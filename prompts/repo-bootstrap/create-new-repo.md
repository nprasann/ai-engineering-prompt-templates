# Create New Repo

## Purpose
Create a plan and initial file structure for a new software repository.

## When to Use
Use when starting a new repository from an idea, feature brief, or technical goal.

## Inputs Needed
- `<PROJECT_NAME>`
- `<TECH_STACK>`
- `<TASK>`
- `<CONSTRAINTS>`
- `<OUTPUT_FORMAT>`

## Prompt
You are helping create a new repository named `<PROJECT_NAME>`.

Goal: `<TASK>`

Technology stack: `<TECH_STACK>`

Constraints: `<CONSTRAINTS>`

Produce a vendor-neutral repository bootstrap plan. Include:
- Proposed folder structure.
- Initial files to create.
- README outline.
- Development setup commands.
- Testing approach.
- Security and secret-handling notes.
- First implementation milestones.

If information is missing, state assumptions clearly. Keep the plan generic enough to publish and avoid private or sensitive details.

Output format: `<OUTPUT_FORMAT>`

## Expected Output
A repo creation plan with structure, file list, setup steps, test strategy, and first milestones.

## Quality Rules
- Do not include real credentials, production data, or private system names.
- Prefer small, incremental milestones.
- Include tests and verification from the start.
- Keep generated examples generic.
- Recommend human review before committing generated code.

