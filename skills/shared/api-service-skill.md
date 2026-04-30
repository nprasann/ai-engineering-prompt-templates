---
name: api-service
description: Use when adding or changing API endpoints, request models, response models, or service-layer behavior.
---

## When to Use
Use this skill when `<TASK>` touches HTTP APIs, RPC endpoints, route handlers, controllers, service wiring, health checks, or request/response contracts.

## Context
API work should preserve contracts, validate inputs, keep route handlers thin, and make behavior easy to test.

## Instructions
1. Read existing route/controller setup, request models, response models, and service-layer patterns.
2. Follow the current framework and project layout.
3. Keep endpoint contracts explicit and JSON-friendly when applicable.
4. Validate inputs before calling databases, filesystems, model providers, queues, or external services.
5. Preserve authentication, authorization, audit, and correlation behavior where present.
6. Update nearby docs or examples when endpoint behavior changes.

## Rules
- Do not expose unrestricted database, filesystem, shell, or network access.
- Do not make breaking contract changes without calling them out.
- Do not add external hosted-service calls unless explicitly configured.
- Do not hardcode secrets, tenants, URLs, or environment names.

## Validation
- Run focused API tests if present.
- Exercise changed endpoints with non-sensitive sample data.
- Verify health or readiness checks where available.
- Confirm error responses for invalid input.

