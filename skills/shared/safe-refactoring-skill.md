---
name: safe-refactoring
description: Use when improving structure, naming, boundaries, or duplication without intentionally changing behavior.
---

## When to Use
Use this skill when `<TASK>` is a refactor, modernization, cleanup, dependency boundary improvement, or maintainability pass.

## Context
Safe refactoring protects current behavior while making code easier to understand, test, or extend.

## Instructions
1. State the refactoring goal and the behavior that must remain unchanged.
2. Read the smallest set of files needed to understand the current flow.
3. Identify tests or smoke checks before editing.
4. Make one cohesive change at a time.
5. Preserve public API shapes, documented commands, configuration names, and output formats unless `<TASK>` requires changing them.
6. Summarize changed behavior as "none intended" unless behavior actually changed.

## Rules
- Do not combine refactoring with feature work unless explicitly requested.
- Do not remove tests without replacing coverage.
- Do not rename public endpoints, exported functions, or environment variables casually.
- Do not introduce new dependencies unless the benefit is clear and scoped.

## Validation
- Run focused tests for touched code.
- Compare before and after behavior for changed services or public interfaces.
- Run formatting or linting if configured.
- Report any tests not run and why.

