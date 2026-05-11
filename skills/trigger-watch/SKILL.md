# Trigger Event Monitor

Search for news and trigger events across a book of business. Filter for commercial relevance and produce a digest grouped by account owner.

## When to use

- Weekly cadence (every Monday or Friday)
- Before outbound planning sessions
- When looking for timely reasons to re-engage dormant accounts

## Inputs

- List of target accounts (company names)
- (Optional) Grouped by account owner/AE
- (Optional) Specific trigger types to prioritise

## Trigger Event Categories

| Category | What to look for | Why it matters |
|----------|-----------------|----------------|
| Funding | New funding round, IPO filing, debt raise | Budget unlocked, growth mode |
| Leadership | New CTO, CFO, CIO, VP Payments hire | New decision-maker, fresh eyes |
| Expansion | New market, new office, acquisition | Infrastructure needs scale |
| Product | Product launch, platform migration | Technical window open |
| Partnership | New vendor announced, integration partner | Competitive displacement opportunity |
| Financial | Earnings report, revenue milestone, cost cuts | Budget pressure or growth signal |
| Regulatory | Compliance deadline, industry regulation change | Urgency driver |

## Execution

### Step 1: Search

For each account in the list, search web sources for events from the last 7 days (or configured window):
- News articles
- Press releases
- LinkedIn company posts
- Job postings (hiring signals)
- Regulatory filings

### Step 2: Filter for Relevance

For each event found, assess:
- Is this commercially relevant? (Does it create a reason to reach out?)
- Is this timely? (Happened in the search window?)
- Is this verified? (From a credible source with a URL?)

Discard events that are:
- Not commercially relevant (awards, CSR announcements, generic PR)
- Older than the search window
- From unreliable sources

### Step 3: Score and Prioritise

Rate each trigger event:
- **High**: Creates an immediate reason to reach out (new CTO, funding round, expansion to your market)
- **Medium**: Useful context for a conversation but not urgent (product launch, partnership)
- **Low**: Background intel only (earnings, minor hire)

### Step 4: Output

Generate digest grouped by account owner:

```
## Trigger Events — Week of [Date]

### [AE Name]'s Accounts

**[Company A]** — HIGH
- [Event]: [One-line summary]. Source: [URL]
- Suggested angle: [How to use this in outreach]

**[Company B]** — MEDIUM
- [Event]: [One-line summary]. Source: [URL]

### [AE Name 2]'s Accounts
...

### No Triggers Found
- [Company X], [Company Y] — no relevant events this period
```

## Constraints

- Only include events from credible, linkable sources.
- Never fabricate or speculate about events. If unsure, don't include.
- Keep the digest scannable. One line per event, not paragraphs.
- "No triggers found" is a valid output. Don't force relevance where none exists.
- Suggested angles must be specific to the event, not generic ("I saw you raised a round" is bad, "your Series C likely means scaling payments infrastructure" is better).
