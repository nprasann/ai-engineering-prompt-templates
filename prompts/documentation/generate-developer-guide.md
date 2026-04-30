# Generate Developer Guide

## Purpose
Create a developer guide for building, testing, and contributing to a project.

## When to Use
Use when README content is too short for detailed development workflows.

## Inputs Needed
- `<PROJECT_NAME>`
- `<TECH_STACK>`
- `<FILES_TO_INSPECT>`
- `<CONSTRAINTS>`
- `<OUTPUT_FORMAT>`

## Prompt
Generate a developer guide for `<PROJECT_NAME>`.

Tech stack: `<TECH_STACK>`

Files to inspect: `<FILES_TO_INSPECT>`

Constraints: `<CONSTRAINTS>`

Include local setup, architecture orientation, development commands, test strategy, debugging, code style, contribution flow, and safe handling of configuration.

Output format: `<OUTPUT_FORMAT>`

## Expected Output
A developer guide suitable for `docs/developer-guide.md`.

## Quality Rules
- Prefer discovered commands over guesses.
- Mark unknowns.
- Avoid secrets and private data.
- Include verification steps.

