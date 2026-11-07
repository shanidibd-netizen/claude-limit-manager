---
description: "Use when implementing or reviewing Claude Code plan limits, session limits, quota status, limit data sources, or related refresh behavior in this app."
---
# Claude Code Session Limits

## Confirmed Scope
- This app concerns Claude Code plan and session limits.
- Anthropic API usage, rate limits, and billing are out of scope unless a task explicitly expands the product scope.

## Rules and Data Sources
- No concrete limit rules, data formats, or data sources are documented in the repository yet. Treat these as unknown, not as permission to guess.
- Before changing limit calculations or status behavior, trace the existing implementation and its tests. Identify where the data comes from, when it is refreshed, and how unavailable or stale data is represented.
- Prefer documented, authoritative Claude Code behavior and existing project evidence. Distinguish observed behavior from assumptions, and ask for clarification when the source or rule cannot be verified.
- Keep source-specific parsing separate from limit interpretation where the existing architecture allows it; do not silently substitute API billing data for Claude Code plan/session data.
- Add or update focused tests for verified limit rules, refresh behavior, and missing or stale data states.
