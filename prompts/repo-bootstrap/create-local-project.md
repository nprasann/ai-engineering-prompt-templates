# Create Local Project

## Purpose
Guide an assistant through creating a local project folder and initial working files.

## When to Use
Use when building a new local prototype, utility, app, or service before publishing it.

## Inputs Needed
- `<LOCAL_PATH>`
- `<PROJECT_NAME>`
- `<TECH_STACK>`
- `<TASK>`
- `<CONSTRAINTS>`
- `<OUTPUT_FORMAT>`

## Prompt
Create a local project at `<LOCAL_PATH>` named `<PROJECT_NAME>`.

Task: `<TASK>`

Tech stack: `<TECH_STACK>`

Constraints: `<CONSTRAINTS>`

First inspect whether `<LOCAL_PATH>` already exists. If it exists, summarize current contents before changing anything. Then create a minimal, working project with:
- Source files.
- Dependency or environment files.
- README with setup and run instructions.
- Tests or a clear test scaffold.
- `.gitignore` appropriate for `<TECH_STACK>`.

Keep the implementation simple and runnable. Do not add secrets, private endpoints, or production data. Show the commands needed to run and test the project.

Output format: `<OUTPUT_FORMAT>`

## Expected Output
A created or planned local project with clear run commands, tests, and a concise summary of files changed.

## Quality Rules
- Inspect before editing.
- Avoid overwriting existing work without confirmation.
- Keep dependencies minimal and conventional.
- Include verification steps.
- Avoid private or sensitive content.

