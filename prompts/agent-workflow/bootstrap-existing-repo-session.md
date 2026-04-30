# Bootstrap Existing Repo Session

## Purpose
Start an AI-assisted session in an existing repository with safe inspection before edits.

## When to Use
Use at the beginning of a new task in an unfamiliar or partially familiar repo.

## Inputs Needed
- `<REPO_URL>`
- `<LOCAL_PATH>`
- `<PROJECT_NAME>`
- `<TASK>`
- `<CONSTRAINTS>`
- `<FILES_TO_INSPECT>`
- `<OUTPUT_FORMAT>`

## Prompt
Bootstrap an AI-assisted engineering session for `<PROJECT_NAME>`.

Repository: `<REPO_URL>`

Local path: `<LOCAL_PATH>`

Task: `<TASK>`

Files or directories to inspect first: `<FILES_TO_INSPECT>`

Constraints: `<CONSTRAINTS>`

First inspect the repository state, including structure, README or docs, build files, tests, and any existing assistant instruction files. Do not edit files during the inspection phase.

Then produce:
- Repo overview.
- Relevant files and directories.
- Existing build/test commands.
- Risks or missing information.
- Proposed small plan for `<TASK>`.
- Files likely to change.
- Verification steps.

Wait for confirmation before broad or risky changes.

Output format: `<OUTPUT_FORMAT>`

## Expected Output
A session bootstrap summary and focused plan for safe work.

## Quality Rules
- Inspect before editing.
- Do not overwrite user changes.
- Keep changes minimal and task-focused.
- Identify tests before implementation.
- Avoid private or sensitive content in summaries.

