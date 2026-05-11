# Morning Brief

Generate a single prioritised task list for the day by aggregating messages, calendar, email, and outstanding action items.

## When to use

- First thing every morning before starting work
- After returning from leave or OOO
- When context-switching between projects

## Inputs

- Access to: internal messaging (DMs from key stakeholders), calendar (today's events), email inbox (unread/flagged), and active to-do list

## Execution

### Step 1: Check Internal Messages

Scan DMs from key stakeholders (manager, account executives, cross-functional partners) from the last 12 hours. Extract:
- Action items directed at you
- Questions waiting for your response
- Context updates that affect today's priorities
- Meeting prep requests

### Step 2: Check Calendar

Pull today's calendar events. For each meeting:
- What prep is needed (research, docs, agenda)
- Who's attending
- What you need to bring or follow up on after

### Step 3: Check Email

Scan inbox for:
- Prospect replies that need response (high priority)
- Internal requests
- Meeting confirmations or changes
- Anything flagged/starred

### Step 4: Check Active To-Dos

Review outstanding action items from previous days. Flag:
- Overdue items
- Items blocked on someone else (note who)
- Items that can be completed today

### Step 5: Prioritise and Output

Generate a single task list grouped by person or account:

```
## Today's Priorities — [Date]

### Urgent (do first)
- [Task] — [context] — [deadline if any]

### Meetings
- [Time] [Meeting name] — Prep needed: [X]

### Follow-ups
- [Person/account] — [what's needed]

### Can wait
- [Lower priority items]
```

## Output Format

Plain text, scannable in 30 seconds. No fluff. Each item has enough context to act on without clicking into another tool.

## Constraints

- Don't surface noise. Only include items that require action TODAY.
- If nothing urgent exists, say so. Don't invent urgency.
- Group by person/account so related items cluster together.
- Flag anything that's been waiting more than 48 hours.
