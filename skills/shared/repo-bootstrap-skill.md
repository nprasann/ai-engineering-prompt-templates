---
name: repo-bootstrap
description: Use when first entering a repository, recovering context, or preparing a safe implementation session.
---

## When to Use
Use this skill at the start of a new task, after context loss, or when asked to understand `<PROJECT_NAME>` before changing files.

## Context
Repository bootstrap skills help the assistant build a factual picture of the project before planning or editing. They are useful across new repos, existing repos, local prototypes, and public starter templates.

## Instructions
1. Read repository instructions first, such as `AGENTS.md`, `instructions.md`, or contributor docs, when present.
2. Read `README.md`, dependency manifests, build files, and task-relevant docs.
3. Inspect `<FILES_TO_INSPECT>` before broad searching.
4. Identify the likely files to touch, commands to run, and smallest validation path.
5. Check worktree status before editing.
6. State assumptions when repo commands, architecture, or ownership boundaries are unclear.

## Rules
- Keep changes minimal and task-focused.
- Do not rewrite unrelated files.
- Do not introduce secrets, private URLs, or production data.
- Do not rely on chat history for architecture facts.
- Prefer discovered repo commands over guessed commands.

## Validation
- Confirm target files and commands before implementation.
- Use fast search tools such as `rg` when available.
- Run the smallest meaningful check after changes.
- Report any missing dependencies or local services that block validation.

