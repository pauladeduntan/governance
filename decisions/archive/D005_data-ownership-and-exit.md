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

This decision constrains **visibility-to-enforcement drift** by treating exit and identity rendering as safety properties rather than accountability features.

## Decision

### 1) Household Membership is an Access Boundary

- Leaving or being removed ends access immediately.
- Former Members cannot access Shared Cart, Activity, Members, or Invites for that Household.

### 2) Activity is Append-only and Non-narrative

- Activity records shared intent changes as a readable record, not a judgement surface.
- Household boundary events may appear in Activity as system-owned feed lines without individual attribution by default (for example, Household Name Updated, Household Members Updated, A Former Member No Longer Has Access).
- Any clarifying detail for Household boundary events is kept in read-only context views.
- Boundary visibility remains bounded: it must not introduce blame, “who removed whom,” or audit-style interpretation by default.

### 3) Former Member Identity is De-identified by Default

- After membership ends, Activity references the actor as “Former Member” (system-owned label).
- No persistent display-name history is presented as a story or attribution trail by default.

### 4) Coordination Artefacts are Household-Scoped, not Person-Scoped

- Shared Cart Items and Activity belong to the Household boundary.
- Personal profile identity must not become a global reputation layer or a scorekeeping substrate.

### 5) Deletion is not a Front-door Affordance in the Current Research Prototype

- Use safe hiding and reversibility patterns for Items (see D011 and the Invariants).
- Any deletion or erasure requests are treated as an off-surface privacy process, not a user-facing flow in public research materials.

## Rationale

- Constrains coercion and surveillance interpretations.
- Supports exit safety so participation does not increase interpersonal risk.
- Keeps the probe aligned with the invariant: Emotional Safety Over Optimisation.

## Implications

- Some accountability detail is intentionally unavailable.
- Systems that require audit trails for enforcement are out of scope.
- UI copy must reflect boundaries without blame (for example, “Access Ended Immediately”).

## Non-goals

- Dispute resolution, moderation, or enforcement tooling.
- Permanent attribution histories.

## Acceptance Criteria

- A removed or departed Member cannot access any Household data.
- Activity entries referencing a Former Member show “Former Member”, not their prior name, by default.
- No UI exposes “who removed whom” by default.

## Review and Supersession

This decision can only be changed via a new decision entry:

- D00X - Data Ownership And Exit Safety Update (Supersedes D005)
