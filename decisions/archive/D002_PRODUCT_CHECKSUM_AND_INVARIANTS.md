# D002 — Product Checksum and Non-Negotiable Invariants

## Status
Accepted (active)

## Product Checksum
**“Making every day lighter, together.”**

All product decisions must reduce mental load and preserve emotional safety.
If a feature, flow, or system increases vigilance, guilt, pressure, or monitoring,
it violates the checksum and must be rejected or redesigned.

## Core Intent
KinCart exists to make **shared intent visible**, not to measure performance,
enforce fairness, or optimise behaviour.

Visibility is for coordination and reassurance — not control.

## Non-Negotiable Invariants

### 1. Visibility without enforcement
- The system shows what is intended, in progress, or completed.
- It does not assign blame, rank contributors, or evaluate effort.
- No leaderboards, scores, streaks, quotas, or performance metrics.

### 2. Awareness without judgement
- Language avoids “fairness”, “accountability”, or “ownership”.
- The system never implies failure, lateness, or neglect.
- Absence of action is treated as context, not deficiency.

### 3. Completion is lightweight and reversible
- Completing an item is a soft signal, not a terminal state.
- Items can be completed by anyone and re-added without friction.
- No confirmations, warnings, or “are you sure?” friction in MVP.

### 4. No surveillance patterns
- No read receipts, last-seen indicators, or inactivity tracking.
- No “who didn’t do this” views or nudging mechanics.
- Updates are ambient, not interruptive.

### 5. System-owned language
- The system uses neutral language (“completed”, “added”, “updated”).
- No language that implies deletion, failure, or neglect.
- Emotional tone must feel supportive, not managerial.

### 6. Context before action
- Household context is always resolved before showing items.
- Users can belong to multiple households without role conflict.
- The system never assumes priority across households.

## Explicit Non-Goals
KinCart is not:
- A task manager
- A productivity tool
- A compliance or accountability system
- A family management or behavioural enforcement app

## Implications for Design and Engineering
- Schema decisions favour append-only logs and soft state.
- UI avoids checklists that feel evaluative or punitive.
- Features that optimise “efficiency” at emotional cost are rejected.
- Any future feature proposal must explicitly state how it preserves the checksum.

## Review / Supersession
This decision may only be changed by a new entry:
- D00X — Product Checksum Revision

