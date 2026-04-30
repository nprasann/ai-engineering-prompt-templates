# Test Gap Analysis

## Purpose
Identify missing test coverage and prioritize new tests.

## When to Use
Use before refactors, releases, or reliability improvements.

## Inputs Needed
- `<PROJECT_NAME>`
- `<TECH_STACK>`
- `<TASK>`
- `<FILES_TO_INSPECT>`
- `<OUTPUT_FORMAT>`

## Prompt
Analyze test gaps for `<PROJECT_NAME>`.

Tech stack: `<TECH_STACK>`

Focus: `<TASK>`

Files to inspect: `<FILES_TO_INSPECT>`

Review current tests and identify important behavior that is untested or weakly tested. Prioritize gaps by risk and suggest specific test cases.

Output format: `<OUTPUT_FORMAT>`

## Expected Output
A prioritized test-gap report with recommended test cases.

## Quality Rules
- Focus on meaningful behavior, not coverage vanity.
- Include regression-prone areas.
- Note missing test infrastructure.
- Avoid using sensitive test data.

