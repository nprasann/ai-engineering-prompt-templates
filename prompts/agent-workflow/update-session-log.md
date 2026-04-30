# Update Session Log

## Purpose
Update a session log after an AI-assisted coding or documentation task.

## When to Use
Use at the end of a session or after a meaningful checkpoint.

## Inputs Needed
- `<PROJECT_NAME>`
- `<TASK>`
- `<FILES_TO_INSPECT>`
- `<CONSTRAINTS>`
- `<OUTPUT_FORMAT>`

## Prompt
Update the session log for `<PROJECT_NAME>`.

Task: `<TASK>`

Files inspected or changed: `<FILES_TO_INSPECT>`

Constraints: `<CONSTRAINTS>`

Create a concise session entry that includes:
- Date.
- Assistant/tool used.
- Task summary.
- Files inspected.
- Files changed.
- Key decisions.
- Tests or checks run.
- Results.
- Risks or limitations.
- Follow-up tasks.

Do not include secrets, sensitive logs, private data, credentials, or internal-only details.

Output format: `<OUTPUT_FORMAT>`

## Expected Output
A session-log entry that can be pasted into `sessions.md`.

## Quality Rules
- Be factual and concise.
- Include verification status.
- Separate completed work from follow-ups.
- Keep content generic enough to publish when needed.

