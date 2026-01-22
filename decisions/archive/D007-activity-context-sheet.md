# D007 - Activity Context Sheet for Handoff (Locked)

## Status

Accepted (Locked)

## Date Recorded

2026-01-05

## Context

Households need “For: <name>” as basic Handoff Item clarity. Showing “For: <name>” directly in the Activity feed risks responsibility signalling and performance-feed dynamics (FM4).

This decision constrains **visibility-to-enforcement drift** by keeping High-Stakes context available on demand without turning the feed into responsibility signalling.

This decision keeps:

- Shared Cart high-clarity (Handoff Item context visible where coordination decisions happen)
- Activity calm (readable record, not a coordination ledger)

## Decision

Activity remains minimal by default. For Handoff-related Activity entries, additional context is revealed on demand via a read-only bottom sheet titled “Activity Context”.

## User-Facing Behaviour (Locked)

### Activity Feed (Default)

- Event line example: `Chioma Added “Dentist”`
- Optional chip: `Handoff` only

The Activity feed must not include:

- `For: <name>` chips
- Handoff type chips (`Pickup`, `Appointment`, `Visit`, `Other`)
- Any additional Handoff descriptor text beyond the `Handoff` chip
- Hearts events or counts

### Activity Context Sheet (Read-only)

Trigger: tap a Handoff-related Activity row.

Contents:

- Title: `Activity Context`
- Item name (primary)
- Chips: `Handoff`, `For: <name>`, `<type>` (`Pickup`, `Appointment`, `Visit`, `Other`)

Exit safety:

- If the “For” person is not an active Member, show `Former Member` (system-owned) instead of their name.

Constraints:

- Read-only only (no edit actions)
- The Activity Context sheet shows only the minimum context needed for interpretation.
- Longer Item details, if present elsewhere, belong to the Item Details surface, not the Activity Context sheet.

## Review and Supersession

This decision can only be changed via a new decision entry:

- D00X - Activity Context Sheet For Handoff Update (Supersedes D007)
