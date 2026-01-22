# D009 - Activity Detail Sheets are Optional, Neutral Context

## Status

Accepted (Locked)

## Date Recorded

2026-01-08

## Owner

KinCart Founder (Sole Architect)

## Related

D006 (Activity Privacy Veil), D007 (Activity Context Sheet)

## Decision

Activity rows may open an optional read-only detail sheet that provides minimal, neutral context without turning Activity into evidence, blame, or surveillance.

- Detail sheets are optional and non-blocking.
- Detail sheets do not add actor attribution beyond what is already shown by the system.
- Detail sheets avoid moral language and avoid “why” narratives.

## Rationale

Activity must stay readable and safe. When more context is needed, it should be provided without escalating Household dynamics. This decision constrains **visibility-to-enforcement drift** by keeping additional context bounded, read-only, and non-narrative.

## Invariants Protected

- Emotional Safety Over Optimisation
- Exit Safety
- Activity Is Not A Performance Feed

## Trade-offs

- Less accountability detail
- More safety in conflict-prone situations

## Detail Sheet Scope (Current Research Prototype)

1) Item Details (For Item-related Activity)  
   - Read-only context that helps a Member understand what changed and recover from mistakes where recovery is allowed by design.

2) Activity Context (Handoff Item)  
   - Governed by D007. Handoff context remains minimal in the feed and is revealed only on demand via a read-only context sheet.

Excluded from this decision by default:

- Membership change sheets
- Household name change sheets
- Display name change sheets

If any of the excluded sheet types are ever introduced, they require an explicit new decision and must remain system-owned and non-attributed by default.

## Copy Constraints

- No “who did this to whom” framing.
- Prefer boundary language: access, membership, visibility.
- No moral language, no blame cues, no enforcement framing.

## Review and Supersession

This decision can only be changed via a new decision entry:

- D00X - Activity Detail Sheets Update (Supersedes D009)
