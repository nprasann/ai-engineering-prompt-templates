---
name: security-review
description: Use when reviewing code, prompts, docs, examples, or releases for security and public-safety issues.
---

## When to Use
Use this skill before making a repo public, publishing examples, changing auth/data access, or handling configuration.

## Context
Security review should find practical risks without reproducing sensitive values in reports.

## Instructions
1. Scan for secrets, tokens, credentials, private keys, connection strings, and `.env` files.
2. Scan for private URLs, internal hostnames, personal contact info, production data, logs, screenshots, and proprietary content.
3. Review auth, authorization, input validation, data access, logging, and error handling when code is involved.
4. Replace environment-specific details with placeholders.
5. Separate blockers from optional hardening ideas.
6. Remind maintainers that git history needs separate review.

## Rules
- Do not paste secret values into findings.
- Do not assume current-file scans prove history is safe.
- Do not remove useful content if placeholder replacement is enough.
- Do not expose private organizational context.

## Validation
- Confirm `.gitignore` excludes common secret files.
- Re-run targeted scans after fixes.
- Summarize files reviewed, findings, fixes, and remaining manual checks.

