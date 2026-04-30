---
name: vector-db
description: Use when changing vector collections, indexes, payloads, dimensions, search filters, or vector database configuration.
---

## When to Use
Use this skill when `<TASK>` touches vector store setup, collection schema, vector dimensions, upserts, search filters, payload fields, or local vector database configuration.

## Context
Vector database changes can affect ingestion, retrieval quality, citations, and migration requirements.

## Instructions
1. Locate vector client setup, collection/index creation, environment examples, and query code.
2. Confirm host, port, collection name, vector size, distance metric, payload structure, and filter fields.
3. Treat collection schema changes as migrations and explain when data must be re-ingested.
4. Keep payload fields stable for citations, filtering, observability, and audit review.
5. Use explicit upsert and search behavior.
6. Keep local defaults easy to run without private infrastructure.

## Rules
- Do not silently change vector dimensions or distance metrics.
- Do not mix embeddings with incompatible dimensions.
- Do not store private source text in public examples.
- Do not hardcode cloud credentials or endpoints.

## Validation
- Start or connect to the local vector store if available.
- Create or inspect the collection/index.
- Ingest sample data and verify payload fields.
- Run vector search and confirm scores and citation metadata.

