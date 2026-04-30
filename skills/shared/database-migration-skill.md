---
name: database-migration
description: Use when changing schemas, migrations, seed data, indexes, or data access behavior.
---

## When to Use
Use this skill when `<TASK>` touches database schema, migrations, indexes, stored procedures, ORM models, seed data, or data access boundaries.

## Context
Database changes should be explicit, reversible where practical, and validated against realistic non-sensitive fixtures.

## Instructions
1. Inspect existing migration tooling, schema files, ORM models, and data access patterns.
2. Identify whether the change is backward-compatible.
3. Separate schema changes from data backfills when possible.
4. Use placeholder or synthetic sample data only.
5. Document rollback or mitigation steps for risky changes.
6. Update tests and docs for changed data contracts.

## Rules
- Do not include production data in migrations or fixtures.
- Do not hardcode database credentials or connection strings.
- Do not make destructive changes without an explicit migration plan.
- Do not bypass existing data access controls.

## Validation
- Run migration tests or apply migrations to a local/test database.
- Run focused data access tests.
- Verify indexes, constraints, and rollback notes where relevant.

