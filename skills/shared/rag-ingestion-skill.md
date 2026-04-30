---
name: rag-ingestion
description: Use when adding or changing document ingestion, chunking, metadata, embeddings, or vector writes for a RAG system.
---

## When to Use
Use this skill when work touches source loading, text extraction, chunking, embedding generation, metadata capture, or writing vectors to a store.

## Context
RAG ingestion should preserve citation metadata, produce deterministic chunks, and keep embedding configuration aligned with retrieval.

## Instructions
1. Inspect ingestion inputs, supported file types, metadata fields, chunking strategy, embedding provider, and vector store configuration.
2. Preserve source metadata such as source name, section, page, URL, timestamp, and stable chunk identifiers where available.
3. Keep chunking deterministic and meaningful; avoid fragments that lose context.
4. Confirm embedding dimensions and vector collection configuration before changing embeddings.
5. Make ingestion idempotent where practical.
6. Keep examples based on sample documents or placeholders.

## Rules
- Do not mix embedding models in one collection without an explicit migration.
- Do not remove citation metadata from stored payloads.
- Do not ingest private documents into public examples.
- Do not hardcode provider credentials.

## Validation
- Run ingestion against a non-sensitive sample file.
- Confirm vectors and metadata are written to the expected collection or index.
- Run a retrieval query and verify returned chunks include usable citations.
- Run focused ingestion tests if available.

