# Analyze Codebase

## Purpose
Analyze a codebase before planning changes.

## When to Use
Use before refactoring, onboarding, estimating work, or documenting architecture.

## Inputs Needed
- `<LOCAL_PATH>`
- `<PROJECT_NAME>`
- `<TECH_STACK>`
- `<FILES_TO_INSPECT>`
- `<OUTPUT_FORMAT>`

## Prompt
Analyze `<PROJECT_NAME>` at `<LOCAL_PATH>`.

Tech stack: `<TECH_STACK>`

Files to inspect: `<FILES_TO_INSPECT>`

Summarize repository structure, main components, build/test commands, data flow, dependencies, risks, and likely improvement areas. Do not edit files.

Output format: `<OUTPUT_FORMAT>`

## Expected Output
A concise codebase analysis with risks, opportunities, and recommended next steps.

## Quality Rules
- Separate facts from assumptions.
- Prefer evidence from files.
- Avoid speculative rewrites.
- Include test and security observations.

