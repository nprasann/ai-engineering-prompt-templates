---
name: ci-cd
description: Use when changing CI workflows, release automation, build scripts, or deployment checks.
---

## When to Use
Use this skill when `<TASK>` touches GitHub Actions, other CI systems, build scripts, release checklists, artifacts, packaging, or deployment validation.

## Context
CI/CD changes should be minimal, reproducible, and safe for public repositories.

## Instructions
1. Inspect existing workflow files, build scripts, package manifests, and release docs.
2. Preserve current triggers and required checks unless the task asks to change them.
3. Use least-privilege permissions in workflows.
4. Keep secrets referenced by environment names, not literal values.
5. Cache dependencies only when it is safe and understandable.
6. Update README or release docs when commands change.

## Rules
- Do not commit tokens, deploy keys, or secret values.
- Do not broaden workflow permissions casually.
- Do not add deployment steps that target real infrastructure without placeholders.
- Do not hide failing tests by weakening checks.

## Validation
- Run local build/test commands when possible.
- Validate workflow syntax where tooling exists.
- Summarize expected CI behavior and any manual checks still required.

