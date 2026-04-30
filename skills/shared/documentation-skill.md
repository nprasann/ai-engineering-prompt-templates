---
name: documentation
description: Use when creating or updating README files, developer guides, runbooks, architecture docs, ADRs, or release notes.
---

## When to Use
Use this skill when `<TASK>` is primarily documentation or when code changes require nearby docs updates.

## Context
Good engineering docs should be accurate, scannable, public-safe, and tied to commands or workflows that actually exist.

## Instructions
1. Inspect existing docs and source files before writing.
2. Prefer discovered commands over guessed commands.
3. Mark assumptions and unknowns clearly.
4. Keep examples generic and placeholder-based.
5. Include setup, run, test, and troubleshooting guidance when relevant.
6. Keep docs concise enough for maintainers to keep current.

## Rules
- Do not include private URLs, internal hostnames, credentials, or production data.
- Do not invent unsupported features or commands.
- Do not paste large proprietary snippets.
- Do not duplicate content unnecessarily across many docs.

## Validation
- Check links and referenced file paths where practical.
- Verify commands when local dependencies are available.
- Review docs for public-release safety.

