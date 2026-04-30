# Implementation Plan

## Purpose
Create a practical implementation plan for a feature, fix, or project.

## When to Use
Use before starting multi-step engineering work.

## Inputs Needed
- `<PROJECT_NAME>`
- `<TECH_STACK>`
- `<TASK>`
- `<CONSTRAINTS>`
- `<FILES_TO_INSPECT>`
- `<OUTPUT_FORMAT>`

## Prompt
Create an implementation plan for `<TASK>` in `<PROJECT_NAME>`.

Tech stack: `<TECH_STACK>`

Files to inspect: `<FILES_TO_INSPECT>`

Constraints: `<CONSTRAINTS>`

Include assumptions, milestones, file-level change plan, tests, docs, risks, dependencies, and release checklist.

Output format: `<OUTPUT_FORMAT>`

## Expected Output
A focused implementation plan ready for review.

## Quality Rules
- Keep milestones small.
- Include tests and rollback.
- Avoid unrelated refactors.
- Mark unknowns clearly.

