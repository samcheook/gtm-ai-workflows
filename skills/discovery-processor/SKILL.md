# Discovery Call Processor

Convert raw discovery call notes or transcripts into a structured AE handoff document. Extracts key intel, identifies gaps, and drafts the follow-up email.

## When to use

- Immediately after a discovery call (within 30 minutes)
- When processing a call transcript or recording summary
- When an AE needs a structured handoff brief

## Inputs

- Raw call notes, transcript, or verbal summary
- Attendee names and roles
- Account context (if available from prior research)

## Execution

### Step 1: Extract Structured Data

Parse the input for the following fields. If a field cannot be determined from the notes, mark as "[Not discussed - follow up needed]".

| Field | What to extract |
|-------|----------------|
| Pain points | Specific problems mentioned, quantified where possible |
| Current state | What they're using today, what's working, what isn't |
| Decision process | Who else is involved, what approvals are needed |
| Timeline | When do they want to solve this, any hard deadlines |
| Budget signals | Any mention of budget, contract values, willingness to invest |
| Competition | Other vendors mentioned, other options being evaluated |
| Champion | Who on their side is pushing for this internally |
| Economic buyer | Who signs off on spend |
| Success criteria | What does "good" look like for them |
| Next steps | What was agreed on the call |

### Step 2: Build Contact Map

For each person mentioned or present on the call:
- Name and title
- Role in the decision (buyer, influencer, blocker, champion, user)
- Key quote or position if stated
- Relationship warmth (engaged, neutral, sceptical)

### Step 3: Identify Gaps

List discovery questions that were NOT answered on the call. Prioritise by importance for deal progression. Suggest how to follow up on each gap (email, next call, different contact).

### Step 4: Draft Follow-Up Email

Write a short follow-up email to the primary contact:
- Thank them for their time (one line)
- Recap 2-3 key points discussed (shows you listened)
- Confirm next steps as agreed
- Attach or reference anything promised on the call
- Max 80 words

### Step 5: Generate AE Handoff Brief

Structured one-page document:
```
ACCOUNT: [Company name]
CALL DATE: [Date]
ATTENDEES: [Names + roles]

SUMMARY: [2-3 sentences: what they want, why now, what's next]

PAIN POINTS:
- [Quantified where possible]

DECISION PROCESS:
- [Who, what approvals, timeline]

COMPETITION:
- [What else they're looking at]

CHAMPION: [Name, why they're pushing]
ECONOMIC BUYER: [Name, role]

GAPS (need follow-up):
- [What we still don't know]

RECOMMENDED NEXT STEPS:
- [What the AE should do]

FOLLOW-UP EMAIL: [Draft below]
```

## Output Format

Deliver both the AE handoff brief and the follow-up email draft. Flag any critical gaps that could block deal progression.

## Constraints

- Never invent information not present in the call notes.
- Mark uncertain information as "[Inferred - verify]".
- If the call notes are thin, say so. Don't pad with assumptions.
- The handoff brief should be scannable in 60 seconds by a busy AE.
