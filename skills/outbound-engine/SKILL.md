# Outbound Email Engine

Generate personalised first-touch outbound emails for enterprise prospects. Adapts by persona, account mode, and seniority. Verifies all claims before output.

## When to use

- Generating Day 1 outbound for a new account
- Drafting emails for multiple contacts at the same company
- Adapting messaging for different personas within one account

## Inputs

- Account research brief (or key account context)
- Contact name, role, and seniority level
- Mode selection: A (known relationship) or B (cold/no prior engagement)

## Mode Selection

**Mode A** (relationship exists, contact knows about existing engagement):
- Use account-specific data and metrics
- Loss framing: quantify what they're currently losing, not what they could gain
- Dollar estimates where possible ("$X in failed transactions" not "Y% failure rate")
- Direct, data-led opening

**Mode B** (cold, no visible prior relationship):
- No internal data in the email. Frame around their business problem.
- Industry pain and branded social proof
- "For businesses running [their scale], [common problem] is where the most time gets lost"
- No mention of internal data or existing account information

## Persona Adaptation

| Persona | Max Length | Lead With | Tone |
|---------|-----------|-----------|------|
| C-suite | 60 words | Cost reduction, vendor consolidation | Strategic, sparse |
| Finance/Controller | 80 words | Reconciliation, cash flow, DSO | Metrics, public data OK |
| Technical/Developer | 65 words | Problem first, no fluff | Direct, specific |
| Operations | 80 words | Multi-site complexity, fewer vendors | Practical |
| Payments/Platform Admin | 100 words | Account-specific data (Mode A only) | Peer-to-peer |

## Execution

1. **Determine mode** based on account context. If contact manages the existing relationship directly: Mode A. If contact may not be aware of existing engagement: Mode B.

2. **Select persona** from the table above. Apply length and tone constraints.

3. **Draft email** following structure:
   - Subject line: lowercase, max 5-6 words, looks like an internal forward
   - First sentence: value, news, or their problem (NOT an introduction)
   - Introduction (brief, 1 sentence, paragraph 2)
   - One specific hook (not two products, not three benefits, ONE thing)
   - CTA: low commitment ("15 min would cover it" or "worth a 15-min catch up?")
   - Sign-off: "Talk soon," + sender name

4. **Verify claims**: Every factual statement must trace to a confirmed source (CRM data, public filing, company website, news article). Remove any claim that cannot be sourced.

5. **Preview text check**: First ~35 characters must hook the reader. No "Hi [Name]" opening. Inline the name naturally. Hook about THEM first.

## Output Format

```
Subject: [lowercase, 5-6 words]
Preview score: [estimated engagement based on first 35 chars]

[Email body]

---
Mode: [A/B]
Persona: [type]
Word count: [X]
Claims verified: [list sources]
```

## Constraints

- One hook per email. Not two products, not three benefits. One thing.
- Max 100 words for first-touch emails. Scannable on mobile in 15 seconds.
- Never fabricate metrics, case studies, or social proof.
- Subject lines must look like an internal forward, not a vendor pitch.
- No em dashes. No polished triads. No "leverage", "unlock", "seamless", "holistic."
- Each email must work if forwarded internally. No contradictions between emails to different personas at same company.
