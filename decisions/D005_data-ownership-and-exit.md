Decision D005: Data ownership and exit safety (research-first, household-safe defaults)

Status: Accepted (LOCKED)  
Date recorded: 2026-01-08  
Owner: KinCart system (sole architect)

Context
KinCart is a coordination probe. It must not trap people in a Household, and it must not turn Activity into evidence or leverage during conflict.
This decision sets the minimum safety properties for:
⦁	data ownership (who “owns” what)
⦁	identity exposure (especially after leaving)
⦁	exit/leave/remove semantics (access boundaries)

Decision
1.	Household membership is an access boundary.
⦁	Leaving or being removed ends access immediately.
⦁	Former members cannot read Shared Cart, Activity, Members, or Invites.
2.	Activity is append-only and non-narrative.
⦁	Activity records boundary changes and shared intent changes, not “who is at fault”.
⦁	Membership boundary events are system-owned and non-attributed by default.
3.	Former member identity is de-identified by default.
⦁	After membership ends, Activity references the actor as “Former member” (system-owned label).
⦁	No persistent display-name history is exposed as a “story”.
4.	Data scope is Household-scoped, not person-scoped, for coordination artifacts.
⦁	Shared Cart Items and Activity belong to the Household context.
⦁	Personal profile identity is not used as a “global reputation layer”.
5.	Deletion is not a front-door affordance in MVP/probe.
⦁	Use safe hiding/reversibility patterns for Items (see D011/D014).
⦁	For research pack: treat deletion requests as an administrative/privacy process (not a UI flow).

Rationale
⦁	Prevents coercion and surveillance dynamics.
⦁	Enables “exit safety” so participation does not increase interpersonal risk.
⦁	Keeps the probe aligned with the invariant: emotional safety > optimisation.

Implications
⦁	Some “accountability” detail is intentionally unavailable.
⦁	Systems that require audit trails for enforcement are explicitly out-of-scope.
⦁	UI copy must reflect boundaries without blame (e.g., “Access ended immediately.”).

Non-goals
⦁	Dispute resolution, moderation, or enforcement tooling.
⦁	Permanent attribution histories.

Acceptance criteria
⦁	A removed/left member cannot access any Household data.
⦁	Activity events referencing a former member show “Former member”, not their prior name.
⦁	No UI exposes “who removed whom” by default.
