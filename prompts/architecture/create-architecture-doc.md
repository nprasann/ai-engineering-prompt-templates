# Create Architecture Doc

## Purpose
Create a concise architecture document for a project.

## When to Use
Use when a repo needs a current design overview for maintainers or reviewers.

## Inputs Needed
- `<PROJECT_NAME>`
- `<TECH_STACK>`
- `<FILES_TO_INSPECT>`
- `<CONSTRAINTS>`
- `<OUTPUT_FORMAT>`

## Prompt
Create an architecture document for `<PROJECT_NAME>`.

Tech stack: `<TECH_STACK>`

Files to inspect: `<FILES_TO_INSPECT>`

Constraints: `<CONSTRAINTS>`

Document goals, non-goals, components, data flow, key dependencies, runtime behavior, testing, security, operational concerns, and known tradeoffs.

Output format: `<OUTPUT_FORMAT>`

## Expected Output
A maintainable architecture document with clear sections and assumptions.

## Quality Rules
- Do not invent undiscovered details.
- Mark unknowns clearly.
- Keep language generic and publishable.
- Include verification and security notes.

