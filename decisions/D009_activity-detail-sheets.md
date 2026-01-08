# D009 — Activity detail sheets are optional, non-accusatory context

Date: 2026-01-08
Status: Accepted
Owner: System (KinCart)
Related: D006 (activity privacy veil), D007 (activity context sheet)

## Decision
Activity rows may open an optional detail sheet that provides minimal, neutral context — without turning Activity into evidence, blame, or surveillance.

- Detail sheets are optional and non-blocking.
- Detail sheets do not add actor attribution beyond what is already shown by the system.
- Detail sheets avoid moral language and avoid “why” narratives.

## Rationale
Activity must stay readable and safe. When more context is needed, it should be provided without escalating household dynamics.

## Invariants Protected
- Emotional safety > optimisation
- Exit safety
- Activity is not a performance feed

## Trade-offs
- Less “accountability detail”
- More safety in conflict-prone situations

## Detail sheet types (MVP)
1) Item details (for Item-related Activity)
2) Membership change (join / leave / removed)
3) Household name change
4) Display name change

## Copy constraints
- No “who did this to whom” framing.
- Prefer boundary language: access, membership, visibility.
