# Follow-Up Tracker

Scan sent email for outbound messages that haven't received a reply. Flag stale conversations, prioritise by account value, and draft short follow-up messages.

## When to use

- Daily or every 2-3 days as part of pipeline hygiene
- When you suspect prospects have gone cold
- Before weekly pipeline review meetings

## Inputs

- Access to sent email (last 14 days)
- (Optional) Minimum days without reply (default: 3)
- (Optional) Priority accounts to check first

## Execution

### Step 1: Scan Sent Email

Search sent messages from the last 14 days. For each outbound email to a prospect (not internal):
- Check if a reply has been received
- Calculate days since sent with no response
- Flag any message with no reply after the configured threshold (default: 3 days)

### Step 2: Prioritise

Rank flagged messages by:
1. Account revenue potential (high value first)
2. Days since sent (older = more urgent)
3. Contact seniority (C-suite replies matter more)
4. Sequence position (first touch vs. follow-up)

### Step 3: Draft Follow-Up Messages

For each flagged message, draft a short bump. Rules:
- Max 40 words
- New angle or value add (don't just say "checking in")
- Reference the original email naturally ("the [topic] I mentioned")
- Same thread (reply to original) unless original subject was weak
- One clear CTA

**Follow-up templates by situation:**

| Situation | Approach |
|-----------|----------|
| First touch, no reply (3-5 days) | New thread, case study or social proof angle |
| First touch, no reply (7+ days) | Final attempt, direct and brief |
| Reply went cold mid-conversation | Reference where you left off, re-ask the question |
| Meeting request ignored | Reduce commitment ("even 10 min would work") |

### Step 4: Output

Present a table:

```
| Contact | Company | Days Silent | Original Subject | Priority | Suggested Action |
|---------|---------|-------------|-----------------|----------|-----------------|
```

Followed by draft bump messages for the top 5 priority items.

## Constraints

- Do not follow up more than 3 times on a single thread without a reply.
- If a contact has explicitly said "not interested" or "not now", remove from tracker.
- Never draft a follow-up that contradicts the original email.
- Keep bumps conversational, not corporate.
