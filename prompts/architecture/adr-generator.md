# ADR Generator

## Purpose
Generate an Architecture Decision Record for a specific decision.

## When to Use
Use when documenting a technology, design, or process choice.

## Inputs Needed
- `<PROJECT_NAME>`
- `<TECH_STACK>`
- `<TASK>`
- `<CONSTRAINTS>`
- `<OUTPUT_FORMAT>`

## Prompt
Generate an ADR for `<PROJECT_NAME>`.

Decision topic: `<TASK>`

Tech stack: `<TECH_STACK>`

Constraints: `<CONSTRAINTS>`

Include status, context, decision, options considered, consequences, risks, and follow-up review date.

Output format: `<OUTPUT_FORMAT>`

## Expected Output
A complete ADR suitable for a docs or `adr/` folder.

## Quality Rules
- State assumptions.
- Include tradeoffs, not just benefits.
- Avoid private details.
- Keep the decision reviewable.

