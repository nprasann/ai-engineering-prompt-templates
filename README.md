# AI Engineering Prompt Templates

A vendor-neutral prompt-template library for AI-assisted software engineering. Prompts are reusable software engineering artifacts.

These prompts are designed for GitHub Copilot Chat, Codex, Claude Code, Cursor, local LLM workflows, and similar AI coding assistants. They help developers and technical managers run small, focused AI coding sessions for repo bootstrapping, refactoring, documentation, testing, architecture, and delivery planning.

## What This Repo Is For

Use this repository when you want repeatable prompts for common software engineering workflows:

- Repo bootstrapping and local project creation.
- `AGENTS.md`, instruction files, and session logs.
- Codebase analysis and behavior-preserving refactors.
- Architecture reviews, architecture docs, ADRs, and tradeoff analysis.
- Test plans, unit tests, integration tests, and test-gap analysis.
- README files, developer guides, runbooks, and release checklists.
- Public-release sanitization and documentation cleanup.
- Reusable skill guidance for recurring workflows such as API work, RAG ingestion, testing, documentation, CI/CD, and security review.

Small focused prompts are usually better than large generic prompts. Planning and execution should usually be separate sessions: first ask the assistant to inspect and plan, then ask it to make bounded changes after you review the plan.

## 2-Minute Quick Start

1. Pick a prompt from `prompts/`.
2. Optionally pick a skill from `skills/shared/` when the task needs reusable workflow guidance.
3. Copy the prompt into GitHub Copilot Chat, Codex, Claude Code, Cursor, or another coding assistant.
4. Replace placeholders such as `<PROJECT_NAME>`, `<TECH_STACK>`, `<TASK>`, and `<CONSTRAINTS>`.
5. Ask the assistant to inspect relevant files before editing.
6. Review the plan, then run a separate focused execution prompt if changes are needed.
7. Review diffs, run tests, and inspect generated files before committing.

## How to Use

1. Pick a prompt from `prompts/`.
2. Add one to three relevant skills from `skills/shared/` when reusable workflow guidance would help.
3. Copy the prompt and skill instruction into your AI coding assistant.
4. Replace placeholders such as `<PROJECT_NAME>`, `<TECH_STACK>`, and `<TASK>`.
5. Keep each session small and focused.
6. Review the assistant's plan before accepting broad edits.
7. Review diffs, run tests, and inspect generated files before committing.

Never commit secrets, credentials, tokens, customer data, private notes, production data, or proprietary code that is not meant to be shared.

## Folder Structure

```text
.
├── prompts/      # Reusable prompt templates organized by workflow
├── skills/       # Reusable workflow guidance for common engineering tasks
├── templates/    # Markdown artifact templates for repo docs and workflows
├── examples/     # Generic example scenarios showing prompt usage
├── README.md
├── CONTRIBUTING.md
└── LICENSE
```

## Placeholder Reference

- `<REPO_URL>`: Repository URL or remote origin.
- `<LOCAL_PATH>`: Local filesystem path for the project.
- `<PROJECT_NAME>`: Project or repository name.
- `<TECH_STACK>`: Languages, frameworks, tools, and runtime.
- `<TASK>`: The specific work to perform.
- `<CONSTRAINTS>`: Scope, safety, style, compatibility, or policy limits.
- `<FILES_TO_INSPECT>`: Files or directories the assistant should read first.
- `<OUTPUT_FORMAT>`: Desired response format, file format, or structure.

## How to Use Skills in Prompts

Skills are reusable guidance artifacts that describe how an assistant should approach a recurring engineering workflow. Use them with prompts when the task benefits from domain-specific rules but should still stay bounded.

Example instruction to add beneath a prompt:

```text
Use these skills while completing the task:
- skills/shared/repo-bootstrap-skill.md
- skills/shared/safe-refactoring-skill.md
- skills/shared/testing-skill.md

Apply the skill guidance only where relevant. Keep the task bounded by <TASK> and <CONSTRAINTS>.
```

Recommended pattern:

1. Use a prompt to define the task and expected output.
2. Add one to three relevant skills for workflow guidance.
3. Ask the assistant to explain which skills it is using and why.
4. Keep planning and execution separate for risky changes.
5. Review diffs and run validation before committing.

Skill examples in this repo include RAG ingestion, RAG retrieval, vector DB work, API services, .NET APIs, frontend UI, database migrations, CI/CD, testing, documentation, refactoring, and security review.

## Platform Notes

- GitHub Copilot Chat: best for repo-aware Q&A, small edits, tests, and explanations inside a GitHub or IDE workflow.
- Codex / agent-based tools: best for multi-file repo tasks, automated edits, inspection-to-implementation loops, and verification summaries.
- Claude Code: strong for reasoning-heavy refactors and large context.
- Cursor: strong for IDE-integrated editing.
- Local LLMs: useful for private/offline work but less reliable for large refactors.

## Prompt Design Principles

- Make the prompt specific to one outcome.
- Separate planning prompts from execution prompts when risk or scope is meaningful.
- Tell the assistant what files to inspect first.
- Include required inputs and expected output.
- Ask for tests, verification, and a concise change summary.
- Prefer placeholders over hardcoded project details.
- Keep prompts vendor-neutral unless a tool-specific workflow is intentional.
- Use skills to add reusable workflow rules without bloating the prompt itself.

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
- Avoid proprietary code, private organizational context, customer data, internal URLs, and personal contact information.
- Ask for tests or verification steps whenever code changes.
- Treat AI output as a draft until reviewed by a human.

## Security Note

Before publishing, forking, or sharing generated content, scan for secrets, credentials, private URLs, internal hostnames, production data, customer data, sensitive logs, and proprietary content. Use placeholders for environment-specific values and verify that `.gitignore` excludes local secret files such as `.env`, `.env.*`, `*.key`, and `*.pem`.

This repository is a prompt-template library only. It should not contain real application secrets, production configuration, customer data, or private implementation details.

## Contributing

Contributions should follow [CONTRIBUTING.md](CONTRIBUTING.md). New prompts must use the standard prompt format, rely on placeholders for project-specific details, and stay generic enough to be reused across teams and AI coding assistants.

## Public-Release Safety Checklist

Before publishing a prompt, template, example, or generated artifact, confirm:

- No secrets, tokens, credentials, private keys, or passwords.
- No `.env` files or environment-specific config values.
- No real production data, customer data, logs, traces, or screenshots.
- No internal URLs, private hostnames, or organization-specific systems.
- No personal email addresses, phone numbers, or private contact details.
- No proprietary code or documentation not intended for publication.
- Examples use placeholders or generic sample values.
