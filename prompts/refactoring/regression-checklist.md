# Regression Checklist

## Purpose
Create a checklist for validating behavior after code changes.

## When to Use
Use before merging refactors, upgrades, or multi-file edits.

## Inputs Needed
- `<PROJECT_NAME>`
- `<TECH_STACK>`
- `<TASK>`
- `<CONSTRAINTS>`
- `<OUTPUT_FORMAT>`

## Prompt
Create a regression checklist for `<PROJECT_NAME>`.

Tech stack: `<TECH_STACK>`

Change being validated: `<TASK>`

Constraints: `<CONSTRAINTS>`

Include automated tests, manual checks, edge cases, security checks, performance concerns, rollback signals, and documentation updates.

Output format: `<OUTPUT_FORMAT>`

## Expected Output
A practical validation checklist for reviewers and maintainers.

## Quality Rules
- Focus on changed behavior.
- Include negative and edge cases.
- Include security and data-handling checks.
- Keep checklist actionable.

