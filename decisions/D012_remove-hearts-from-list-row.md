# D012 — Hearts are removed from the main list row

Date: 2026-01-08
Status: Accepted
Owner: System (KinCart)
Related: D008 (hearts item-scoped)

## Decision
Hearts are not a primary action on every Shared Cart list row by default.

- Do not place Hearts as a prominent row action alongside core coordination controls.
- Access Hearts via an intentional entry point (e.g., a Hearts sheet / menu).

## Rationale
If Hearts are always visible, the UI implicitly trains users to perform gratitude. That creates pressure and distracts from intent visibility.

## Invariants Protected
- Emotional safety > optimisation
- Shared intent visibility without social currency

## Trade-offs
- One extra step to express appreciation
- Lower risk of gratitude-as-status and lower visual clutter
