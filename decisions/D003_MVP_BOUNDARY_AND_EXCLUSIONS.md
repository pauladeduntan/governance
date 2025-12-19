# D003 — MVP Boundary and Explicit Exclusions

## Status
Accepted (active)

## Purpose
This decision defines the **explicit boundary of the KinCart MVP**.
Anything not listed as “in scope” is intentionally excluded, even if it appears
technically simple or commonly expected.

This protects focus, emotional safety, and research integrity.

## MVP Scope (Inclusions)

The MVP includes only:

### 1. Household context resolution
- Users can belong to one or more households.
- A household must be selected before viewing carts or items.
- No hierarchy, roles, or permissions beyond active membership.

### 2. Shared carts
- A household has one or more carts.
- Carts contain items representing shared intent.
- Carts are simple containers, not projects or plans.

### 3. Items as soft state
- Items can be added by any household member.
- Items can be completed by any household member.
- Completion hides items without deleting them.
- Completed items can be re-added without friction.

### 4. Ambient activity visibility
- The system records neutral activity events (added, completed).
- Activity is append-only and non-evaluative.
- No reactions, comments, or acknowledgements in MVP.

### 5. Guest and authenticated access
- Users may explore as guests.
- Authentication enables persistence, not privilege.

## Explicit Exclusions (Non-Negotiable for MVP)

The MVP will NOT include:

### A. Assignment and ownership
- No item assignment to individuals.
- No “who is responsible” designation.
- No acceptance, claiming, or delegation flows.

### B. Reminders and nudging
- No notifications, reminders, or follow-ups.
- No “you haven’t done this” or “don’t forget” mechanics.

### C. Fairness or contribution metrics
- No tracking of who did more or less.
- No statistics, charts, or summaries of contribution.
- No gamification or streaks.

### D. Social feedback
- No reactions (likes, hearts).
- No comments or discussion threads.
- No praise or acknowledgement mechanics.

### E. Event orchestration
- No timelines, deadlines, or schedules.
- No event-specific flows in MVP.
- Event examples may exist only as illustrative concepts.

### F. Administrative controls
- No admin dashboards.
- No moderation, approvals, or controls.
- No audit or compliance views.

## Rationale
Each excluded feature introduces:
- Surveillance risk
- Emotional pressure
- Implicit judgement
- Increased mental load

These costs outweigh short-term usability gains in MVP.

## Implications
- Feature requests that fall outside this boundary are deferred.
- “Easy to add later” is not a justification for inclusion.
- MVP success is measured by **clarity and calm**, not completeness.

## Review / Supersession
This decision may only be changed by a new entry:
- D00X — MVP Boundary Revision
