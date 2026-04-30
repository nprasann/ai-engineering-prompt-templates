# Create Instructions.md

## Purpose
Create a reusable instructions file for AI-assisted development sessions.

## When to Use
Use when a team wants consistent assistant behavior across tools and projects.

## Inputs Needed
- `<PROJECT_NAME>`
- `<TECH_STACK>`
- `<TASK>`
- `<CONSTRAINTS>`
- `<OUTPUT_FORMAT>`

## Prompt
Create an `instructions.md` file for AI-assisted work on `<PROJECT_NAME>`.

Tech stack: `<TECH_STACK>`

Primary task types: `<TASK>`

Constraints: `<CONSTRAINTS>`

The instructions should cover:
- How the assistant should inspect the repo.
- How it should propose and execute changes.
- How it should handle tests and validation.
- How it should summarize work.
- Security and privacy requirements.
- Rules for avoiding broad refactors unless requested.

Keep the file platform-agnostic so it works with GitHub Copilot Chat, Codex, Claude Code, Cursor, and similar tools.

Output format: `<OUTPUT_FORMAT>`

## Expected Output
A clean `instructions.md` draft with practical, reusable assistant guidance.

## Quality Rules
- Keep instructions generic and publishable.
- Include no credentials, private URLs, or internal names.
- Prefer specific verification behavior.
- Emphasize small focused sessions.

