# GTM AI Workflows

Production AI skills built with Claude Code to automate and accelerate Go-To-Market workflows. Used daily for 6 months in enterprise sales operations including account research, outbound generation, and discovery call processing.

## Skills

### Account Research Pipeline
Pulls data from CRM, internal data sources, Slack, and web into a single structured brief. Replaces a half-day manual research process with one command.

**Inputs:** Company name or account ID
**Outputs:** Structured brief with revenue data, product usage, corporate family map, contact map, competitive landscape, and recommended positioning

### Outbound Email Engine
Generates personalised outbound emails with persona adaptation and account-mode selection. Includes mandatory fact-verification against live data sources before any claim enters an email.

**Features:**
- Mode selection (direct relationship vs. cold/platform)
- Persona adaptation (C-suite, Finance, Technical, Operations)
- Preview text optimisation
- Automated verification of all factual claims

### Discovery Call Processor
Converts raw call notes or transcripts into structured AE handoff documentation in under a minute.

**Outputs:** Contact map, pain points, next steps, follow-up email draft, recommended positioning for AE

### Follow-Up Tracker
Scans sent email for outbound messages with no reply after a configurable window. Flags them and drafts short follow-up messages.

### Morning Brief
Aggregates Slack, Gmail, calendar, and CRM data into a single prioritised task list for the day.

### End-of-Day Update
Generates a short summary of what was accomplished, pulled from session activity, calendar, and email.

### Trigger Event Monitor
Searches for news and trigger events across a book of business. Filters for commercial relevance and produces a digest grouped by account owner.

---

## Architecture

Each skill is defined in a `SKILL.md` file containing:
- Purpose and trigger conditions
- Step-by-step execution instructions
- Input/output specifications
- Rules and constraints

Skills are modular and documented for reuse. They can be picked up by any Claude Code user and adapted to their workflow.

## Built With
- [Claude Code](https://claude.ai/code) (Anthropic)
- MCP (Model Context Protocol) for data source integrations
- Structured prompt engineering and agentic workflow design
