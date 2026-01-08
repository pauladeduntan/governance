# D011 — Removal is “Hide item”, reversible; avoid destructive framing

Date: 2026-01-08
Status: Accepted
Owner: System (KinCart)

## Decision
KinCart does not use “Remove” / “Delete” language for Items in the Shared Cart. The substitute action is "Hide item".

- Action label: "Hide item"
- Confirmation explains reversibility: "You can add it again anytime."
- Hide is treated as non-destructive.

## Rationale
Destructive language increases fear and conflict (“who deleted it?”). Hide reduces escalation and keeps the system psychologically safe.

## Invariants Protected
- Emotional safety > optimisation
- Reversibility as a safety property

## Trade-offs
- Slightly less literal than “delete”
- Requires clear copy so users understand it is reversible

## Alternatives considered (rejected)
- Delete / Remove item
  Rejected: invites blame and permanence anxiety.
- Archive with complex semantics
  Rejected: increases mental load.

## UX Contract
- Hide is reversible via "Add again" (or "Show again") depending on the UI surface.
- Avoid multiple competing reversibility affordances in the same moment; prefer one clear route back.
