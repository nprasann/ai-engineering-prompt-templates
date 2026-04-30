# Generate Unit Tests

## Purpose
Generate unit tests for a specific component or behavior.

## When to Use
Use when adding coverage for pure logic, small modules, or isolated behavior.

## Inputs Needed
- `<PROJECT_NAME>`
- `<TECH_STACK>`
- `<TASK>`
- `<FILES_TO_INSPECT>`
- `<CONSTRAINTS>`
- `<OUTPUT_FORMAT>`

## Prompt
Generate unit tests for `<TASK>` in `<PROJECT_NAME>`.

Tech stack: `<TECH_STACK>`

Files to inspect: `<FILES_TO_INSPECT>`

Constraints: `<CONSTRAINTS>`

Inspect the implementation and existing test style first. Add tests that match existing patterns. Include normal cases, edge cases, and failure cases.

Output format: `<OUTPUT_FORMAT>`

## Expected Output
Unit tests plus a summary of what behavior they cover.

## Quality Rules
- Follow existing test conventions.
- Avoid brittle tests that depend on internals unnecessarily.
- Do not use production data.
- Run or describe relevant test commands.

