# D005 - Data Ownership and Exit Safety (Research-First, Household-Safe Defaults)

## Status

Accepted (Locked)

## Date Recorded

2026-01-08

## Owner

KinCart Founder (Sole Architect)

## Context

KinCart is a coordination probe. It must not trap people in a Household, and it must not turn Activity into evidence or leverage during conflict.

This decision sets the minimum safety properties for:

- Data scope and ownership (what belongs to a Household boundary)
- Identity exposure (especially after leaving or removal)
- Exit semantics (leave and remove behavior, and access boundaries)

## Decision

### 1) Household Membership is an Access Boundary

- Leaving or being removed ends access immediately.
- Former Members cannot access Shared Cart, Activity, Members, or Invites for that Household.

### 2) Activity is Append-only and Non-narrative

- Activity records shared intent changes as a readable record, not a judgement surface.
- Membership boundary changes must be system-owned and non-attributed by default.
- Boundary changes must not be presented in the Activity feed by default if they increase surveillance or blame risk.

### 3) Former Member Identity is De-identified by Default

- After membership ends, Activity references the actor as “Former Member” (system-owned label).
- No persistent display-name history is presented as a story or attribution trail by default.

### 4) Coordination Artefacts Are Household-Scoped, Not Person-Scoped

- Shared Cart Items and Activity belong to the Household boundary.
- Personal profile identity must not become a global reputation layer or a scorekeeping substrate.

### 5) Deletion is Not a Front-Door Affordance in the Current Research Prototype

- Use safe hiding and reversibility patterns for Items (see D011 and the Invariants).
- Any deletion or erasure requests are treated as an off-surface privacy process, not a user-facing flow in public research materials.

## Rationale

- Prevents coercion and surveillance dynamics.
- Enables exit safety so participation does not increase interpersonal risk.
- Keeps the probe aligned with the invariant: Emotional Safety Over Optimisation.

## Implications

- Some accountability detail is intentionally unavailable.
- Systems that require audit trails for enforcement are out of scope.
- UI copy must reflect boundaries without blame (for example, “Access Ended Immediately”).

## Non-Goals

- Dispute resolution, moderation, or enforcement tooling.
- Permanent attribution histories.

## Acceptance Criteria

- A removed or departed Member cannot access any Household data.
- Activity entries referencing a Former Member show “Former Member”, not their prior name, by default.
- No UI exposes “who removed whom” by default.
