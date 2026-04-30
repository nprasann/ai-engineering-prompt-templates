# Create Sessions.md

## Purpose
Create a session log file for tracking AI-assisted engineering work.

## When to Use
Use when a project needs lightweight records of assistant sessions, decisions, changes, tests, and follow-ups.

## Inputs Needed
- `<PROJECT_NAME>`
- `<TASK>`
- `<CONSTRAINTS>`
- `<OUTPUT_FORMAT>`

## Prompt
Create a `sessions.md` file for `<PROJECT_NAME>`.

Current task focus: `<TASK>`

Constraints: `<CONSTRAINTS>`

The file should include:
- A short purpose statement.
- A reusable session entry template.
- Fields for date, assistant/tool, task, files inspected, changes made, tests run, decisions, risks, and follow-ups.
- A privacy reminder to avoid secrets, customer data, private logs, or proprietary details not meant for the repo.

Output format: `<OUTPUT_FORMAT>`

## Expected Output
A reusable `sessions.md` template ready to track AI-assisted work.

## Quality Rules
- Keep session entries concise.
- Record verification, not just edits.
- Avoid sensitive details.
- Make follow-ups actionable.

