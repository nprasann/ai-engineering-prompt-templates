# Generate README

## Purpose
Create or improve a project README for developers and users.

## When to Use
Use when a repo needs clear setup, usage, development, testing, and contribution guidance.

## Inputs Needed
- `<REPO_URL>`
- `<LOCAL_PATH>`
- `<PROJECT_NAME>`
- `<TECH_STACK>`
- `<TASK>`
- `<CONSTRAINTS>`
- `<FILES_TO_INSPECT>`
- `<OUTPUT_FORMAT>`

## Prompt
Generate a README for `<PROJECT_NAME>`.

Repository: `<REPO_URL>`

Local path: `<LOCAL_PATH>`

Tech stack: `<TECH_STACK>`

Documentation goal: `<TASK>`

Files to inspect: `<FILES_TO_INSPECT>`

Constraints: `<CONSTRAINTS>`

Inspect existing docs, dependency files, source layout, scripts, tests, and configuration. Then create or revise a README with:
- Project overview.
- Features or scope.
- Requirements.
- Setup instructions.
- Run commands.
- Test commands.
- Configuration guidance without secrets.
- Project structure.
- Development workflow.
- Troubleshooting notes.
- Security and secret-handling reminder.

Use generic examples only. Mark unknown commands or assumptions clearly.

Output format: `<OUTPUT_FORMAT>`

## Expected Output
A README draft or patch that accurately reflects the repository.

## Quality Rules
- Do not invent unsupported commands.
- Do not include credentials, private URLs, or production data.
- Keep instructions testable.
- Prefer concise, scannable sections.
- Include human verification reminders.

