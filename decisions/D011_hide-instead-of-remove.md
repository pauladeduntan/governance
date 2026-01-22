# D011 - Removal is “Hide Item”, Reversible, Avoid Destructive Framing

## Status

Accepted (Locked)

## Date Recorded

2026-01-08

## Owner

KinCart Founder (Sole Architect)

## Decision

KinCart does not use “Remove” or “Delete” language for Items in the Shared Cart. The substitute action is “Hide Item”.

- Action label: “Hide Item”
- Hide Item is non-destructive and reversible.
- The interface communicates reversibility with non-blocking microcopy (for example, “You can show it again anytime.”).

This decision is distinct from “Complete Item”. Both actions hide an Item from the active list, but they must not be framed as deletion, punishment, or a moral outcome.

## Rationale

Destructive language amplifies fear and conflict (“who deleted it?”). This constraint constrains **visibility-to-enforcement drift** by avoiding permanence cues that can be read as blame or policing during breakdown and repair.

## Invariants Protected

- Emotional Safety Over Optimisation
- Reversibility By Default

## Trade-offs

- Slightly less literal than “delete”
- Requires clear microcopy so Members interpret it as reversible

## Alternatives Considered (Rejected)

- Delete or Remove Item  
  Rejected: invites blame and permanence anxiety.

- Archive with complex semantics  
  Rejected: increases mental load.

## UX Contract (Constraint-Level)

- Hide Item is reversible via a single clear affordance, preferably “Show Again”, depending on the surface.
- Avoid multiple competing reversal affordances in the same moment. Prefer one clear route back.
- Hide Item must not introduce attribution pressure or “who did this” cues.

## Review and Supersession

This decision can only be changed via a new decision entry:

- D00X - Hide Item Semantics Update (Supersedes D011)
