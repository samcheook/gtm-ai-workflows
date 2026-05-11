# Account Research Pipeline

Run a full account research brief for an enterprise existing-business account. Outputs a structured brief ready for AE handoff or discovery call prep.

## When to use

- Before outbound to a new account
- Before a discovery call or renewal meeting
- When an AE requests background on an account they're picking up

## Inputs

- Company name or account identifier
- (Optional) Specific focus area (e.g. "payments infrastructure", "expansion markets")

## Execution

### Phase 1: Data Collection

1. **CRM pull**: Query the CRM for account metadata. Extract: annual revenue processed, product activations, contract dates, account owner, segment, support ticket history.

2. **Corporate family mapping**: Search for parent/child entity relationships. Identify subsidiaries, brands, and related accounts. Note which entities are active vs. dormant.

3. **Web research**: Search for recent news (last 90 days). Look for: funding rounds, leadership changes, geographic expansion, product launches, acquisitions, partnerships. Capture source URLs and dates.

4. **Internal messaging search**: Search internal channels for mentions of the company. Extract: prior conversations, known blockers, relationship context, technical notes from solutions teams.

5. **Contact mapping**: Identify key decision-makers and their roles. Group by: economic buyer, technical evaluator, champion, day-to-day operator. Note any prior engagement history.

### Phase 2: Analysis

6. **Revenue estimation**: Based on known data, estimate total addressable revenue from this account. Break down by product category. Identify gaps between current usage and full potential.

7. **Product gap analysis**: Compare active products against the full catalog. Identify products that would be relevant based on the account's industry, size, and current stack. Prioritise by estimated revenue impact.

8. **Competitive landscape**: Note any known competitors in the account. Flag if any products are served by competitors that could be displaced.

### Phase 3: Output

9. **Generate brief** with the following sections:
   - Company overview (what they do, size, market position)
   - Current relationship summary (products active, revenue, contract status)
   - Corporate family map (visual hierarchy of entities)
   - Contact map (names, roles, engagement history)
   - Product gap analysis (what's missing, estimated value)
   - Trigger events (recent news, leadership changes)
   - Recommended positioning (what to lead with, what to avoid)

## Output Format

Structured document with clear section headers. Each finding must cite its source (CRM, web, internal channel). Revenue estimates must show methodology. No unsourced claims.

## Constraints

- Never fabricate data. If a field returns empty, say so.
- Distinguish between: access denied, unavailable field, and empty result set.
- A query with zero rows is NOT a data gap.
- Revenue estimates must be labelled as estimates with methodology shown.
- Do not include internal-only data in any output that might be shared externally.
