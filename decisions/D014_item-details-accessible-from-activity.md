# D014 - Item Details are Accessible from Activity

## Status

Accepted (Locked)

## Date Recorded

2026-01-08

## Owner

KinCart Founder (Sole Architect)

## Related

D007 (Activity Context Sheet for Handoff), D009 (Activity Detail Sheets Are Optional, Neutral Context)

## Decision

Activity rows for Item events may open an “Item Details” sheet.

This is the sanctioned way to:

- Read Item details that do not fit in a one-line preview.
- View Handoff-related context without expanding the Activity feed row into a narrative surface.

## Separation of Concerns

- The Activity feed remains minimal and scannable.
- Handoff-specific chips such as `For: <name>` and `Type` remain governed by D007 and are not shown in the Activity feed by default.
- Item Details may show the Item’s own fields and brief context, but must not introduce assignment, enforcement, or policing cues.

## Rationale

Activity stays scannable, while Item detail stays available on demand. This decision constrains **visibility-to-enforcement drift** by relocating high-risk context away from the feed and into a bounded, read-only sheet that supports interpretation and repair without amplifying blame or surveillance cues.

## Invariants Protected

- Visibility Over Reminders
- Emotional Safety Over Optimisation

## Trade-offs

- An extra tap to see full detail
- Cleaner Activity feed and lower escalation risk

## Copy and Content Guardrails

- Details are optional and brief.
- Avoid moral or managerial language.
- Prefer situational summaries over exact timestamps to resist precision policing (aligned with D010).
- Item Details must not add actor attribution beyond what the system already shows.

## Review and Supersession

This decision can only be changed via a new decision entry:

- D00X - Item Details from Activity Update (Supersedes D014)
