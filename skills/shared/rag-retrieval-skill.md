---
name: rag-retrieval
description: Use when changing retrieval, search, ranking, context assembly, grounding, or citations for a RAG system.
---

## When to Use
Use this skill when work touches vector queries, keyword search, hybrid retrieval, ranking, filters, context windows, citation handling, or answer grounding.

## Context
Retrieval should return relevant source context, preserve citation metadata, and avoid unsupported generated answers.

## Instructions
1. Inspect the path from user query to retrieved context to generated answer.
2. Confirm request shape, filters, top-k defaults, scoring, and response payloads.
3. Keep query embedding logic aligned with ingestion embedding configuration.
4. Preserve citation fields from source payloads through final responses.
5. Prefer small ranking or filtering changes over broad retrieval rewrites.
6. Handle empty or weak results with a grounded fallback.

## Rules
- Do not fabricate source content or citations.
- Do not drop audit, authorization, tenant, or user attribution behavior where present.
- Do not silently change retrieval defaults with broad product impact.
- Do not expose private source text in public examples.

## Validation
- Query a known non-sensitive sample document.
- Verify retrieved chunks include source, score, and citation metadata.
- Verify final answers cite retrieved context.
- Run focused retrieval tests or smoke checks.

