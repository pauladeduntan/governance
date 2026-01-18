# D002 - Product Checksum and Non-Negotiable Invariants

## Status

Accepted (Active)

## Product Checksum

“Making every day lighter, together.”

All design decisions must reduce mental load and preserve emotional safety. If a feature, flow, or system increases vigilance, guilt, pressure, or monitoring interpretation, it violates the checksum and must be rejected or redesigned.

## Core Intent

KinCart exists to make shared intent visible, not to measure performance, enforce fairness, or optimise behaviour.

Visibility is for coordination and reassurance, not control.

## Non-Negotiable Invariants

### 1) Visibility Without Enforcement

- The system makes shared intent visible through calm list visibility (active Items and Items hidden from the active list via Complete Item or Hide Item).
- It does not assign blame, rank Members, or evaluate effort.
- No leaderboards, scores, streaks, quotas, or performance metrics.

### 2) Awareness Without Judgement

- Language avoids fairness, accountability, or ownership framing.
- The system never implies failure, lateness, or neglect.
- Absence of action is treated as context, not deficiency.

### 3) Completion Is Lightweight And Reversible

- Complete Item is a reversible visibility action, not a terminal state.
- Items can be completed by any Member and shown again without confrontation.
- Avoid confirmation patterns that increase blame, anxiety, or policing interpretation. Prefer reversible actions and clear context.

### 4) No Surveillance Patterns

- No read receipts, last-seen indicators, or inactivity tracking.
- No “who didn’t do this” views or nudging mechanics.
- Updates are ambient, not interruptive.

### 5) System-Owned Language

- The system uses neutral language (for example, Added, Completed, Updated).
- No language that implies deletion, failure, or neglect.
- Emotional tone must avoid managerial or policing cues.

### 6) Context Before Action

- The active Household context is always explicit and visible before actions are taken.
- Members can belong to multiple Households without implied role hierarchy.
- The system never assumes priority across Households.

### 7) Activity Safety (Read-Only, Non-Amplifying)

- Activity is a calm, read-only record, not a performance feed or notification centre.
- If attribution names are shown for active Members, they are for attribution only and must not be amplified.
- No per-person views, counts, sorting, grouping, filtering, badges, streaks, or export-like summaries.
- After membership ends, identity must dynamically re-render to “Former Member” by default across historical entries and context views.

## Explicit Non-Goals

KinCart is not:

- A task manager.
- A productivity tool.
- A compliance or accountability system.
- A family management or behavioural enforcement app.

## Implications

- Design choices must preserve reversibility, boundary integrity, exit safety, and system-owned language.
- Interface patterns must avoid evaluative checklists and punitive framing.
- Any proposal must explicitly state how it preserves the checksum and which invariant it protects.

## Review and Supersession

This decision may only be changed by a new entry:

- D00X - Product Checksum Revision
