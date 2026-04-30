# AI Engineering Prompt Templates

A vendor-neutral prompt-template library for AI-assisted software engineering.

These prompts are designed for GitHub Copilot Chat, Codex, Claude Code, Cursor, local LLM workflows, and similar AI coding assistants. They help developers and technical managers run small, focused AI coding sessions for repo bootstrapping, refactoring, documentation, testing, architecture, and delivery planning.

## What This Repository Covers

- Create new repositories and local projects.
- Convert ideas into implementation-ready repo plans.
- Create `AGENTS.md`, instruction files, and session logs.
- Analyze and refactor existing codebases.
- Review architecture and document design decisions.
- Generate test plans, unit tests, integration tests, and test-gap reports.
- Create README files, developer guides, runbooks, and release checklists.
- Prepare generic public-release sanitization reviews.

## How to Use

1. Pick a prompt from `prompts/`.
2. Copy it into your AI coding assistant.
3. Replace placeholders such as `<PROJECT_NAME>`, `<TECH_STACK>`, and `<TASK>`.
4. Keep each session small and focused.
5. Review the assistant's plan before accepting broad edits.
6. Review diffs, run tests, and inspect generated files before committing.

Never commit secrets, credentials, tokens, customer data, private notes, production data, or proprietary code that is not meant to be shared.

## Placeholder Reference

- `<REPO_URL>`: Repository URL or remote origin.
- `<LOCAL_PATH>`: Local filesystem path for the project.
- `<PROJECT_NAME>`: Project or repository name.
- `<TECH_STACK>`: Languages, frameworks, tools, and runtime.
- `<TASK>`: The specific work to perform.
- `<CONSTRAINTS>`: Scope, safety, style, compatibility, or policy limits.
- `<FILES_TO_INSPECT>`: Files or directories the assistant should read first.
- `<OUTPUT_FORMAT>`: Desired response format, file format, or structure.

## Platform Notes

- GitHub Copilot Chat: best for repo-aware Q&A, small edits, tests, and explanations.
- Codex-style agents: best for multi-file repo tasks and automated edits.
- Claude Code: strong for reasoning-heavy refactors and large context.
- Cursor: strong for IDE-integrated editing.
- Local LLMs: useful for private/offline work but less reliable for large refactors.

## Recommended Session Pattern

Use prompts in short cycles:

1. Ask the assistant to inspect the current state.
2. Ask for a focused plan.
3. Approve or adjust the plan.
4. Let the assistant make bounded edits.
5. Run tests and review diffs.
6. Record the result in a session log.

## Safety Principles

- Prefer minimal, reversible changes.
- Keep generated examples generic.
- Avoid private identifiers, internal project names, secrets, and real production data.
- Ask for tests or verification steps whenever code changes.
- Treat AI output as a draft until reviewed by a human.

## Security Note

Before publishing, forking, or sharing generated content, scan for secrets, credentials, private URLs, internal hostnames, production data, customer data, sensitive logs, and proprietary content. Use placeholders for environment-specific values and verify that `.gitignore` excludes local secret files such as `.env`, `.env.*`, `*.key`, and `*.pem`.

This repository is a prompt-template library only. It should not contain real application secrets, production configuration, customer data, or private implementation details.

## Contributing

Contributions should follow [CONTRIBUTING.md](CONTRIBUTING.md). New prompts must use the standard prompt format, rely on placeholders for project-specific details, and stay generic enough to be reused across teams and AI coding assistants.

## Repository Layout

- `prompts/`: Reusable prompts organized by engineering workflow.
- `templates/`: Markdown templates for common project artifacts.
- `examples/`: Generic example project scenarios showing how prompts can be applied.
