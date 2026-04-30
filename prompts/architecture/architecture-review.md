# Architecture Review

## Purpose
Review a system or repository architecture and identify practical improvements.

## When to Use
Use before major refactors, scaling work, modernization, or technical planning.

## Inputs Needed
- `<LOCAL_PATH>`
- `<PROJECT_NAME>`
- `<TECH_STACK>`
- `<TASK>`
- `<CONSTRAINTS>`
- `<FILES_TO_INSPECT>`
- `<OUTPUT_FORMAT>`

## Prompt
Perform an architecture review for `<PROJECT_NAME>`.

Local path: `<LOCAL_PATH>`

Tech stack: `<TECH_STACK>`

Review focus: `<TASK>`

Files to inspect: `<FILES_TO_INSPECT>`

Constraints: `<CONSTRAINTS>`

Inspect relevant source, configuration, documentation, tests, deployment files, and dependency manifests. Then produce:
- Executive summary.
- Current architecture overview.
- Main components and responsibilities.
- Data and control flow.
- Coupling, cohesion, and boundary observations.
- Reliability, security, performance, and maintainability risks.
- Testing and observability gaps.
- Recommended improvements by priority.
- Open questions.

Do not make code changes.

Output format: `<OUTPUT_FORMAT>`

## Expected Output
A clear architecture review with prioritized, evidence-based recommendations.

## Quality Rules
- Ground observations in inspected files.
- Separate facts, assumptions, and recommendations.
- Avoid over-engineering.
- Include security and testing considerations.
- Prefer incremental improvement paths.

