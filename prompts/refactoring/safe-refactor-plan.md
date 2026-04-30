# Safe Refactor Plan

## Purpose
Create a low-risk refactoring plan before editing code.

## When to Use
Use when improving structure, reducing duplication, or modernizing code without changing behavior.

## Inputs Needed
- `<LOCAL_PATH>`
- `<PROJECT_NAME>`
- `<TECH_STACK>`
- `<TASK>`
- `<CONSTRAINTS>`
- `<FILES_TO_INSPECT>`
- `<OUTPUT_FORMAT>`

## Prompt
Create a safe refactor plan for `<PROJECT_NAME>`.

Local path: `<LOCAL_PATH>`

Tech stack: `<TECH_STACK>`

Refactor task: `<TASK>`

Files to inspect: `<FILES_TO_INSPECT>`

Constraints: `<CONSTRAINTS>`

First inspect the relevant files and current tests. Then produce a plan with:
- Current behavior to preserve.
- Refactor goals and non-goals.
- Proposed small steps.
- Files likely to change.
- Tests to run before and after.
- Regression risks.
- Rollback strategy.

Do not make code changes unless explicitly asked.

Output format: `<OUTPUT_FORMAT>`

## Expected Output
A step-by-step refactor plan focused on preserving behavior.

## Quality Rules
- Preserve public behavior unless the task says otherwise.
- Prefer small, reviewable changes.
- Identify tests before editing.
- Call out risky assumptions.
- Avoid broad rewrites.

