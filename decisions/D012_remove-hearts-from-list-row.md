# D012 - Hearts are Removed from the Main List Row

## Status

Accepted (Locked)

## Date Recorded

2026-01-08

## Owner

KinCart Founder (Sole Architect)

## Related

D008 (Hearts are Item-Scoped, not a Feed Mechanic)

## Decision

Hearts are not a primary action on every Shared Cart list row by default.

- Do not place Hearts as a prominent row action alongside core coordination controls.
- Hearts are accessed only via an intentional entry point, not as a default always-visible row control.
- Hearts must not appear as Activity events or counts.

## Rationale

If Hearts are always visible, the interface trains performative gratitude. That can be read as obligation and comparison, which constrains emotional safety and can amplify **visibility-to-enforcement drift** by converting appreciation into a pressure cue.

## Invariants Protected

- Emotional Safety Over Optimisation
- Shared intent visibility without social currency

## Trade-offs

- An extra step to express appreciation
- Lower risk of gratitude becoming status
- Lower visual clutter on the Shared Cart

## Review and Supersession

This decision can only be changed via a new decision entry:

- D00X - Hearts Placement Update (Supersedes D012)
