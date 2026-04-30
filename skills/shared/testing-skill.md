---
name: testing
description: Use when adding, updating, or evaluating tests for a project.
---

## When to Use
Use this skill for unit tests, integration tests, smoke tests, regression tests, fixtures, and test-gap analysis.

## Context
Tests should validate important behavior with deterministic inputs and without depending on private services or production data.

## Instructions
1. Inspect existing test layout, naming, dependencies, and commands before adding new conventions.
2. Prefer unit tests for pure logic, parsing, validation, formatting, and service helpers.
3. Use integration tests for API routes, databases, queues, external boundaries, and multi-component behavior.
4. Use smoke checks for local services when full test automation is not available.
5. Use non-sensitive fixtures and deterministic assertions.
6. Keep tests focused on behavior that could regress.

## Rules
- Do not require real credentials for normal tests.
- Do not require network access unless the project already documents it.
- Do not use production data, customer data, or sensitive logs.
- Avoid brittle assertions against unrelated implementation details.

## Validation
- Run the focused test command for changed code.
- If no test runner is configured, document the smallest manual check.
- Include test results in the final summary.

