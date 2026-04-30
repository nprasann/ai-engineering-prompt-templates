# Tradeoff Analysis

## Purpose
Compare engineering options and recommend a practical path.

## When to Use
Use when choosing between architectures, libraries, patterns, or delivery approaches.

## Inputs Needed
- `<PROJECT_NAME>`
- `<TECH_STACK>`
- `<TASK>`
- `<CONSTRAINTS>`
- `<OUTPUT_FORMAT>`

## Prompt
Analyze tradeoffs for `<TASK>` in `<PROJECT_NAME>`.

Tech stack: `<TECH_STACK>`

Constraints: `<CONSTRAINTS>`

Compare viable options across complexity, maintainability, cost, security, performance, reliability, testing impact, and migration risk. Recommend one option and explain why.

Output format: `<OUTPUT_FORMAT>`

## Expected Output
A structured tradeoff analysis with a recommendation and risks.

## Quality Rules
- Compare realistic options.
- Include downside and migration cost.
- Prefer reversible decisions when uncertainty is high.
- Avoid unsupported claims.

