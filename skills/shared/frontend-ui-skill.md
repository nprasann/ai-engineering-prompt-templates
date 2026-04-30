---
name: frontend-ui
description: Use when building or changing frontend UI, routes, components, forms, state, or user workflows.
---

## When to Use
Use this skill when `<TECH_STACK>` includes a frontend framework or the task touches UI behavior, accessibility, layout, or client-side state.

## Context
Frontend changes should fit the existing design system, preserve common workflows, and be verified visually when possible.

## Instructions
1. Inspect existing routes, components, styles, design tokens, and state-management patterns.
2. Keep UI changes consistent with the current product tone and interaction patterns.
3. Prefer accessible native controls and semantic markup.
4. Handle loading, empty, error, and success states.
5. Keep examples generic and avoid real customer data.
6. Update focused tests or visual checks when behavior changes.

## Rules
- Do not add a new design system unless requested.
- Do not hardcode private URLs, user data, or analytics identifiers.
- Do not make broad layout rewrites for a small task.
- Do not let text overflow or overlap in common viewport sizes.

## Validation
- Run relevant frontend tests, linting, or type checks.
- Manually inspect changed screens when possible.
- Verify keyboard navigation and basic accessibility for interactive elements.

