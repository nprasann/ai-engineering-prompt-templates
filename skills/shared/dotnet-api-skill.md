---
name: dotnet-api
description: Use when working on .NET API services, controllers, minimal APIs, middleware, configuration, or tests.
---

## When to Use
Use this skill when `<TECH_STACK>` includes .NET, ASP.NET Core, C#, minimal APIs, controllers, Entity Framework, or xUnit/NUnit/MSTest.

## Context
.NET API work should follow existing project structure, dependency injection patterns, configuration conventions, and test style.

## Instructions
1. Inspect solution files, project files, `Program.cs`, configuration files, controllers/endpoints, services, and tests.
2. Follow existing dependency injection and options/configuration patterns.
3. Keep controllers or endpoints thin and move business logic into services.
4. Use strongly typed models for request and response contracts.
5. Keep configuration environment-driven and placeholder-based.
6. Update tests and README commands when behavior changes.

## Rules
- Do not commit real connection strings or secrets.
- Do not introduce broad framework changes for small tasks.
- Do not change public API routes without calling out compatibility impact.
- Do not bypass authorization, validation, logging, or error handling patterns.

## Validation
- Run `dotnet test` or the focused test project when available.
- Run `dotnet build` when tests are not available.
- Exercise changed endpoints with non-sensitive sample data.

