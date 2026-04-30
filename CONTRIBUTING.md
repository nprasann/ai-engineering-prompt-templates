# Contributing

Thanks for helping improve this prompt-template library. Keep contributions generic, reusable, and safe to publish.

## Add a New Prompt

1. Choose the most relevant folder under `prompts/`.
2. Create a Markdown file with a concise kebab-case name.
3. Use the required prompt format below.
4. Include consistent placeholders where user-specific details belong.
5. Keep examples generic and free of private data.

## Required Prompt Format

Each prompt file must include:

```markdown
# <Prompt Name>

## Purpose

## When to Use

## Inputs Needed

## Prompt

## Expected Output

## Quality Rules
```

## Safety Checklist

- No secrets, API keys, tokens, passwords, private URLs, or credentials.
- No production data, customer data, employee data, or sensitive logs.
- No proprietary code unless the repository owner explicitly intends to publish it.
- No employer-specific, client-specific, or internal system names.
- Prefer placeholders such as `<PROJECT_NAME>`, `<TECH_STACK>`, and `<TASK>`.
- Prefer generic examples that could apply to many teams.
- Require human review of diffs and test results.

## Prompt Style

- Write for multiple AI coding assistants.
- Keep tasks small enough for one focused session.
- Include clear inputs and expected outputs.
- Ask the assistant to inspect relevant files before editing.
- Include guardrails for security, correctness, testing, and minimal changes.

