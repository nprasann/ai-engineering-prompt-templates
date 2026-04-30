# Apply Skills To Task

## Purpose
Help an AI coding assistant choose and apply reusable skill guidance during a focused engineering task.

## When to Use
Use when a task spans a recognizable workflow, such as refactoring, API work, RAG ingestion, testing, documentation, CI/CD, or public-release review.

## Inputs Needed
- `<REPO_URL>`
- `<LOCAL_PATH>`
- `<PROJECT_NAME>`
- `<TECH_STACK>`
- `<TASK>`
- `<CONSTRAINTS>`
- `<FILES_TO_INSPECT>`
- `<OUTPUT_FORMAT>`

## Prompt
You are working on `<PROJECT_NAME>`.

Repository: `<REPO_URL>`

Local path: `<LOCAL_PATH>`

Tech stack: `<TECH_STACK>`

Task: `<TASK>`

Files to inspect first: `<FILES_TO_INSPECT>`

Constraints: `<CONSTRAINTS>`

Select the relevant skill guidance for this task from the available skill files. Use only the skills that materially help the task. Explain which skills you selected and why.

Then:
- Inspect the requested files and any repo instructions.
- Summarize relevant context.
- Create a small plan.
- Apply the selected skill rules while keeping the task bounded.
- Identify validation steps before editing.
- If editing is requested, make minimal changes and run the relevant checks.
- Summarize files changed, checks run, risks, and follow-ups.

Output format: `<OUTPUT_FORMAT>`

## Expected Output
A skill-informed plan or implementation summary that names the selected skills, applies their guidance, and keeps the work focused.

## Quality Rules
- Use skills as guidance, not as permission to expand scope.
- Prefer one to three relevant skills over a long list.
- Keep planning and execution separate for risky or broad work.
- Do not include secrets, production data, private URLs, or proprietary content.
- Review diffs and run tests or explain why checks could not be run.

