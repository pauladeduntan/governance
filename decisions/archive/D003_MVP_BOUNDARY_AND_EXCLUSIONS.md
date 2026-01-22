# D003 - Current Research Prototype Boundary and Explicit Exclusions

## Status

Accepted (Active)

## Purpose

This decision defines the explicit boundary of the current KinCart research prototype. Anything not listed as in scope is intentionally excluded, even if it appears technically simple or commonly expected.

This protects focus, emotional safety, and research integrity.

## Current Research Prototype Scope (Inclusions)

The current research prototype includes only:

### 1) Household Context Resolution

- Members can belong to one or more Households.
- A Household is selected explicitly before viewing Shared Cart or Activity.
- No hierarchy, roles, or permissions beyond active membership.
- System-owned membership transitions exist as safety semantics (Leave Household, Remove Member), even where the prototype UI does not foreground administrative control.

### 2) Shared Cart (Single Default Cart)

- A Household has a single Shared Cart (Default Cart).
- The Shared Cart contains Items representing shared intent.
- The Shared Cart is a coordination surface, not a project plan.

### 3) Items as Soft State

- Items can be added by any Member.
- Items can be completed by any Member.
- Complete Item hides Items without deleting them.
- Items can be shown again without friction (reversible).

### 4) Handoff Item (High-Stakes Probe Surface)

- Handoff Item is an optional High-Stakes coordination stress surface used to amplify breakdown and repair dynamics without introducing enforcement.
- Handoff context is minimal in the Activity feed (event line plus optional Handoff chip).
- Additional Handoff context (For, Type, optional details) is revealed on demand in a read-only Activity context view.

### 5) Ambient Activity Visibility

- The system records a neutral Activity record of Shared Cart actions (for example, Added, Completed, Hid, Showed Again) and system-owned Household boundary events (for example, Household Name Updated, Household Members Updated), with details kept in read-only context views.
- Activity is calm, read-only, and non-evaluative.
- Activity is not a performance feed and must not become a notification centre.
- Attribution names may be shown for active Members as attribution only, without amplification (no per-person views, counts, sorting, grouping, filtering, badges, streaks, or export-like summaries).
- After membership ends, identity must dynamically re-render to “Former Member” by default across historical entries and context views.

### 6) Guest and Optional Sign-in

- Members may explore as guests.
- Sign-in is optional and framed as Save Progress.
- Sign-in enables persistence, not privilege.

### 7) Hearts (Constrained Gratitude)

- Hearts, if present, are item-scoped and must not function as a feed mechanic.
- Hearts must not appear as counts or reactions in Activity.

## Phenomenon Anchor

This scope boundary constrains **visibility-to-enforcement drift** by excluding common coordination mechanisms that can be interpreted as obligation, surveillance, or performance management under breakdown and repair.

## Explicit Exclusions (Non-negotiable for the Current Research Prototype)

The current research prototype will not include:

### A) Assignment and Ownership

- No Item assignment to individuals.
- No “who is responsible” designation.
- No acceptance, claiming, or delegation flows.

### B) Reminders and Nudging

- No notifications, reminders, or follow-ups.
- No “you haven’t done this” or “don’t forget” mechanics.

### C) Fairness or Contribution Metrics

- No tracking of who did more or less.
- No statistics, charts, or summaries of contribution.
- No gamification or streaks.

### D) Social Feedback in Activity or Feed Form

- No reactions in Activity.
- No reaction counts in Activity.
- No comments or discussion threads in Activity.

### E) Event Orchestration

- No timelines, deadlines, or schedules.
- No event-specific cart surfaces.
- Event examples may exist only as illustrative concepts for research discussion.

### F) Administrative Controls

- No admin dashboards.
- No moderation, approvals, or controls.
- No audit or compliance views.

## Rationale

Each excluded category introduces one or more of the following costs:

- Surveillance risk
- Emotional pressure
- Implicit judgement
- Increased mental load

These costs outweigh short-term completeness gains for the current research prototype.

## Implications

- Requests outside this boundary are deferred.
- “Easy to add later” is not a justification for inclusion.
- Success is assessed by clarity and calm, not completeness.

## Review and Supersession

This decision may only be changed by a new entry:

- D00X - Current Research Prototype Boundary Revision (Supersedes D003)
