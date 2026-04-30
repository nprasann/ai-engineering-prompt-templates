# Skills

Skills are reusable guidance files that help an AI coding assistant behave consistently for a specific kind of engineering work.

Use a skill when a task needs more workflow detail than a single prompt should carry. A prompt should define the task, inputs, expected output, and quality rules. A skill should define repeatable domain guidance, inspection steps, implementation rules, and validation habits.

## How to Use Skills With Prompts

1. Pick the prompt that matches the task, such as `prompts/refactoring/safe-refactor-plan.md`.
2. Pick one or more relevant skills from `skills/shared/`.
3. Paste the prompt into your AI coding assistant.
4. Add a short instruction such as:

```text
Use these skills while completing the task:
- skills/shared/safe-refactoring-skill.md
- skills/shared/testing-skill.md

Apply the skill guidance only where relevant. Keep the task bounded by the prompt.
```

5. Replace placeholders such as `<PROJECT_NAME>`, `<TECH_STACK>`, `<TASK>`, `<CONSTRAINTS>`, and `<FILES_TO_INSPECT>`.
6. Review the assistant's plan before allowing broad edits.

## Skill Design Principles

- Keep skills generic and reusable.
- Prefer public-safe placeholders over real environment values.
- Keep skills focused on one workflow or domain.
- Include inspection steps before implementation advice.
- Include validation steps and safety rules.
- Do not include secrets, private URLs, customer data, internal system names, or proprietary code.

## Included Shared Skills

- `repo-bootstrap-skill.md`: starting or re-entering a repository.
- `safe-refactoring-skill.md`: behavior-preserving refactors.
- `testing-skill.md`: unit, integration, smoke, and regression testing.
- `api-service-skill.md`: API endpoint and service-layer changes.
- `rag-ingestion-skill.md`: document ingestion for RAG systems.
- `rag-retrieval-skill.md`: retrieval, ranking, grounding, and citations.
- `vector-db-skill.md`: vector collection and payload changes.
- `dotnet-api-skill.md`: .NET API project work.
- `frontend-ui-skill.md`: frontend and UX implementation work.
- `database-migration-skill.md`: schema and data migration planning.
- `ci-cd-skill.md`: CI, release, and automation workflows.
- `documentation-skill.md`: README, guide, runbook, and architecture docs.
- `security-review-skill.md`: security and public-release review.

