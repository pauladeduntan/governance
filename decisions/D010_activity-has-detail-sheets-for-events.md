# D010 — Activity entries open event-specific detail sheets
Date: 2026-01-08
Status: Accepted

## Context
The Activity feed is a readable record, not a performance log. Some events require extra context without bloating the feed.

## Decision
Activity rows may open a bottom sheet with minimal, event-specific details:
- Item details (for add/complete/hide/show again)
- Membership change (join/leave/remove)
- Household name change
- Display name change

## Rationale
Keeps the feed scannable while allowing “just enough detail” on demand.

## Trade-offs
- Extra UI surface area (sheets) vs reduced feed clutter.
- Must avoid turning sheets into “evidence artifacts” in conflict.

## Guardrails
- No actor attribution by default for sensitive membership changes.
- Copy must remain neutral, system-owned, non-moralizing.
