# Public Release Sanitization

## Purpose
Review a repository or document set for content that should not be published.

## When to Use
Use before making a repository public, sharing templates, or publishing docs.

## Inputs Needed
- `<LOCAL_PATH>`
- `<PROJECT_NAME>`
- `<TASK>`
- `<CONSTRAINTS>`
- `<FILES_TO_INSPECT>`
- `<OUTPUT_FORMAT>`

## Prompt
Perform a public-release sanitization review for `<PROJECT_NAME>`.

Local path: `<LOCAL_PATH>`

Release goal: `<TASK>`

Files to inspect: `<FILES_TO_INSPECT>`

Constraints: `<CONSTRAINTS>`

Inspect the requested files for:
- Secrets, keys, tokens, credentials, or connection strings.
- Private URLs, internal hostnames, customer names, employee names, or vendor-sensitive details.
- Production data, logs, screenshots, or traces.
- Proprietary code or policy content not intended for publication.
- License, attribution, and third-party dependency concerns.
- Documentation that exposes sensitive architecture or operational details.

Produce a findings list with file paths, issue type, severity, recommended fix, and whether the content should be removed, generalized, or replaced with a placeholder.

Do not paste sensitive values into the report. Refer to them by type only.

Output format: `<OUTPUT_FORMAT>`

## Expected Output
A sanitization report and prioritized remediation checklist.

## Quality Rules
- Never reproduce secrets or sensitive values.
- Be conservative when publication risk is unclear.
- Recommend generic placeholders.
- Include license and attribution checks.
- Separate blockers from nice-to-have cleanup.

