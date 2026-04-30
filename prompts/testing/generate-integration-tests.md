# Generate Integration Tests

## Purpose
Generate integration tests across components or external boundaries.

## When to Use
Use when behavior depends on multiple modules, APIs, databases, queues, or file systems.

## Inputs Needed
- `<PROJECT_NAME>`
- `<TECH_STACK>`
- `<TASK>`
- `<FILES_TO_INSPECT>`
- `<CONSTRAINTS>`
- `<OUTPUT_FORMAT>`

## Prompt
Generate integration tests for `<TASK>` in `<PROJECT_NAME>`.

Tech stack: `<TECH_STACK>`

Files to inspect: `<FILES_TO_INSPECT>`

Constraints: `<CONSTRAINTS>`

Inspect existing integration test patterns. Add tests that validate realistic interactions while using safe local fixtures, mocks, containers, or test doubles as appropriate.

Output format: `<OUTPUT_FORMAT>`

## Expected Output
Integration tests and verification instructions.

## Quality Rules
- Avoid real credentials and production services.
- Prefer deterministic local test data.
- Clean up resources created by tests.
- Keep tests focused on externally visible behavior.

