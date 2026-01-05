# D007 — Activity context sheet for Handoff (LOCKED)

Status: Committed
Date: YYYY-MM-DD

## Context
Large households need “For: <name>” as basic handoff clarity. Showing “For: <name>” directly in the Activity feed risks responsibility/ownership signalling and performance-feed dynamics (FM4).

This decision keeps:
- Shared Cart high-clarity (handoff context visible where decisions happen)
- Activity calm (structural log; not a coordination ledger)

## Decision
Activity remains minimal by default.
For Handoff-related Activity entries, additional context is revealed on demand via a read-only bottom sheet titled “Activity context”.

## User-facing behaviour (LOCKED)

### Activity feed (default)
- Event line example: `Chioma added “Dentist”`
- Optional chip: `Handoff` only

The Activity feed must NOT include:
- `For: <name>` chips
- Handoff type chips (Pickup/Appointment/Visit/Other)
- Handoff label text
- Hearts events or counts
- “Household name updated”
- “Household members updated”

### Activity context sheet (read-only)
Trigger: tap a Handoff-related Activity row.

Contents:
- Title: `Activity context`
- Item name (primary)
- Chips: `Handoff`, `For: <name>`, `<type>` (Pickup/Appointment/Visit/Other)

Exit safety:
- If the “For” person is not an active member, show `Former member` (system-owned) instead of their name.

Constraints:
- Read-only only (no edit actions)
- No narrative notes field

## Non-goals (LOCKED)
- No assignment semantics (“assigned to”, “owner”, “responsible”)
- No reminders, urgency, due dates
- No hearts in Activity

## Failure modes defended
- FM4: Activity becomes a performance feed
- FM3: Identity exposure after exit (mask “Former member”)
- FM1: Wrong-household context errors (sheet must reflect active Household)

## Invariants protected
Emotional safety over optimisation; Visibility over reminders; No judgement/scoring;
System-owned language; Exit safety; Minimum identity exposure.
