# Generate Runbook

## Purpose
Create an operational runbook for common maintenance tasks.

## When to Use
Use for services, jobs, apps, or tools that need repeatable operational procedures.

## Inputs Needed
- `<PROJECT_NAME>`
- `<TECH_STACK>`
- `<TASK>`
- `<CONSTRAINTS>`
- `<OUTPUT_FORMAT>`

## Prompt
Generate a runbook for `<PROJECT_NAME>`.

Tech stack: `<TECH_STACK>`

Operational focus: `<TASK>`

Constraints: `<CONSTRAINTS>`

Include purpose, prerequisites, local commands, deployment or release notes if applicable, monitoring signals, troubleshooting steps, rollback guidance, and escalation placeholders.

Output format: `<OUTPUT_FORMAT>`

## Expected Output
A generic runbook draft that avoids environment-specific secrets.

## Quality Rules
- Use placeholders for sensitive endpoints.
- Avoid private incident details.
- Include rollback and verification.
- Keep steps actionable.

