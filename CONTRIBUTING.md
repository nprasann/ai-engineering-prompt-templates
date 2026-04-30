# Contributing

Thanks for helping improve this prompt-template library. Keep contributions generic, reusable, and safe to publish.

## Add a New Prompt

1. Choose the most relevant folder under `prompts/`.
2. Create a Markdown file with a concise kebab-case name.
3. Use the required prompt format below.
4. Include consistent placeholders where user-specific details belong.
5. Keep the prompt focused on one engineering outcome.
6. Keep examples generic and free of private data.

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
- No `.env` files or environment-specific configuration values.
- No production data, customer data, employee data, or sensitive logs.
- No proprietary code unless the repository owner explicitly intends to publish it.
- No employer-specific, client-specific, or internal system names.
- No personal email addresses, phone numbers, or private contact details.
- Prefer placeholders such as `<REPO_URL>`, `<LOCAL_PATH>`, `<PROJECT_NAME>`, `<TECH_STACK>`, `<TASK>`, `<CONSTRAINTS>`, `<FILES_TO_INSPECT>`, and `<OUTPUT_FORMAT>`.
- Prefer generic examples that could apply to many teams.
- Require human review of diffs and test results.

## Prompt Quality Checklist

- Write for multiple AI coding assistants.
- Keep tasks small enough for one focused session.
- Separate planning and execution when the task is risky or broad.
- Include clear inputs and expected outputs.
- Ask the assistant to inspect relevant files before editing.
- Include guardrails for security, correctness, testing, and minimal changes.
- Prefer minimal changes over broad rewrites.
- Include verification expectations such as tests, linting, or manual checks.

## Contributor Workflow

1. Create or update the prompt, template, or example.
2. Check that all content is generic and public-safe.
3. Verify prompt files include every required section.
4. Review diffs for accidental private details.
5. Run any relevant formatting or link checks if your editor provides them.
6. Open a pull request with a short summary of the use case and safety review.

## Add a New Skill

Use skills for reusable workflow guidance that would make an individual prompt too long. A skill should describe how to approach a class of work, not one private project.

1. Add the skill under `skills/shared/` unless it is intentionally scoped elsewhere.
2. Start from `templates/skill.template.md`.
3. Use a generic kebab-case filename such as `database-migration-skill.md`.
4. Include when to use it, context, instructions, rules, and validation.
5. Use placeholders such as `<PROJECT_NAME>`, `<TECH_STACK>`, `<TASK>`, `<CONSTRAINTS>`, `<FILES_TO_INSPECT>`, and `<OUTPUT_FORMAT>`.
6. Keep examples public-safe and avoid real environment details.

Skills should complement prompts. They should not override the prompt's task, constraints, or output format.
