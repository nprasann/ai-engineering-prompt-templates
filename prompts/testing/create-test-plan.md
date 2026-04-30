# Create Test Plan

## Purpose
Create a focused test plan for a feature, fix, or refactor.

## When to Use
Use before implementing or reviewing a change that needs validation.

## Inputs Needed
- `<PROJECT_NAME>`
- `<TECH_STACK>`
- `<TASK>`
- `<CONSTRAINTS>`
- `<OUTPUT_FORMAT>`

## Prompt
Create a test plan for `<TASK>` in `<PROJECT_NAME>`.

Tech stack: `<TECH_STACK>`

Constraints: `<CONSTRAINTS>`

Include unit, integration, end-to-end or manual checks where relevant, plus edge cases, negative cases, test data guidance, and commands to run.

Output format: `<OUTPUT_FORMAT>`

## Expected Output
A practical test plan that can guide implementation and review.

## Quality Rules
- Cover expected, edge, and failure paths.
- Avoid real production data.
- Include automation where practical.
- Keep scope proportional to risk.

