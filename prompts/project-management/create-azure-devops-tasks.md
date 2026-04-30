# Create Azure DevOps Tasks

## Purpose
Create generic task breakdowns suitable for Azure DevOps or similar trackers.

## When to Use
Use when converting a plan into implementation tasks.

## Inputs Needed
- `<PROJECT_NAME>`
- `<TASK>`
- `<TECH_STACK>`
- `<CONSTRAINTS>`
- `<OUTPUT_FORMAT>`

## Prompt
Create implementation tasks for `<TASK>` in `<PROJECT_NAME>`.

Tech stack: `<TECH_STACK>`

Constraints: `<CONSTRAINTS>`

Break work into task titles, descriptions, acceptance criteria, estimates, dependencies, and validation steps.

Output format: `<OUTPUT_FORMAT>`

## Expected Output
A tracker-ready task list.

## Quality Rules
- Keep tasks small and testable.
- Include validation steps.
- Avoid proprietary details.
- Note blockers and assumptions.

