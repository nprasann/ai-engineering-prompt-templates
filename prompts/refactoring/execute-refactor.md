# Execute Refactor

## Purpose
Carry out a planned refactor with minimal behavior change.

## When to Use
Use after a refactor plan has been reviewed or when the task is clearly bounded.

## Inputs Needed
- `<LOCAL_PATH>`
- `<PROJECT_NAME>`
- `<TECH_STACK>`
- `<TASK>`
- `<CONSTRAINTS>`
- `<FILES_TO_INSPECT>`
- `<OUTPUT_FORMAT>`

## Prompt
Execute this refactor for `<PROJECT_NAME>`.

Local path: `<LOCAL_PATH>`

Tech stack: `<TECH_STACK>`

Task: `<TASK>`

Files to inspect or change: `<FILES_TO_INSPECT>`

Constraints: `<CONSTRAINTS>`

Before editing, inspect the target files and summarize the intended changes. Then make the smallest reasonable changes to complete the task while preserving behavior.

After editing:
- Run relevant formatting, linting, and tests when available.
- Summarize files changed.
- Explain behavior preserved.
- Report any tests not run and why.
- List follow-ups separately.

Output format: `<OUTPUT_FORMAT>`

## Expected Output
Completed refactor, verification results, and a concise change summary.

## Quality Rules
- Keep changes focused on `<TASK>`.
- Do not silently change public APIs.
- Do not remove tests without replacing coverage.
- Avoid unrelated cleanup.
- Never introduce secrets or private data.

