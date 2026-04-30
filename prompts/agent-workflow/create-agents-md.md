# Create AGENTS.md

## Purpose
Generate an `AGENTS.md` file that gives AI coding assistants clear repo-specific working instructions.

## When to Use
Use when onboarding AI agents to a repository or standardizing how assistants should inspect, edit, test, and summarize work.

## Inputs Needed
- `<REPO_URL>`
- `<LOCAL_PATH>`
- `<PROJECT_NAME>`
- `<TECH_STACK>`
- `<CONSTRAINTS>`
- `<FILES_TO_INSPECT>`
- `<OUTPUT_FORMAT>`

## Prompt
Create an `AGENTS.md` for `<PROJECT_NAME>`.

Repository: `<REPO_URL>`

Local path: `<LOCAL_PATH>`

Tech stack: `<TECH_STACK>`

Files to inspect first: `<FILES_TO_INSPECT>`

Constraints: `<CONSTRAINTS>`

The `AGENTS.md` should tell AI coding assistants how to work safely in this repo. Include:
- Project overview.
- Repository layout.
- Build, test, lint, and run commands.
- Coding conventions.
- Testing expectations.
- Security and secret-handling rules.
- Instructions for minimal, reviewable changes.
- Session summary expectations.
- A rule to avoid committing secrets or private data.

If commands or conventions are unknown, include placeholders and mark them as needing confirmation.

Output format: `<OUTPUT_FORMAT>`

## Expected Output
A complete, generic `AGENTS.md` draft ready for human review.

## Quality Rules
- Do not invent private details.
- Clearly mark assumptions.
- Prefer repo-discovered commands over guesses.
- Keep instructions concise and actionable.
- Require tests or verification for code changes.

