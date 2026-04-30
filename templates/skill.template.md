---
name: <SKILL_NAME>
description: Use when <TASK> requires repeatable guidance for <TECH_STACK> or a specific engineering workflow.
---

## When to Use
Use this skill when `<TASK>` involves <WORKFLOW_OR_DOMAIN>.

## Context
Describe the reusable engineering context for `<PROJECT_NAME>` without private details.

## Instructions
1. Inspect `<FILES_TO_INSPECT>` and existing repo instructions before editing.
2. Identify assumptions, risks, and the smallest useful validation path.
3. Keep the work bounded by `<CONSTRAINTS>`.
4. Prefer existing project patterns over new abstractions.
5. Use placeholders for environment-specific values.

## Rules
- Do not include secrets, production data, private URLs, or proprietary content.
- Do not rewrite unrelated files.
- Do not broaden scope beyond `<TASK>`.

## Validation
- Run relevant tests, linting, build checks, or smoke checks.
- Report any checks that could not be run.
- Produce the result in `<OUTPUT_FORMAT>` when requested.

