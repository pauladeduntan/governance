# D015 - Membership Changes are Access-Boundary Events, not Narratives

## Status

Accepted (Locked)

## Date Recorded

2026-01-08

## Owner

KinCart Founder (Sole Architect)

## Context

Membership changes can become conflict evidence if framed as blame, attribution, or narrative. KinCart treats membership as an access boundary, not a social storyline.

This decision constrains **visibility-to-enforcement drift** by keeping membership visibility system-owned, low-detail, and low evidence value.

## Decision

Membership changes are represented, when shown, as system-owned access-boundary events with minimal, neutral copy.

### Activity Feed Visibility

- If a membership boundary event is shown in Activity, it uses system-owned, non-attributed wording only (for example, `A Former Member No Longer Has Access`).
- The feed must not show “Left” versus “Removed”, and must not show “who removed whom” or any actor attribution.

### Access Boundary Detail Sheet (Optional, Read-only)

If a detail sheet is presented for a membership boundary event, it remains system-owned and neutral.

It includes:

- Title: `Access Update`
- Body line: `Access Ended Immediately.`
- Fields:
  - Member: `Former Member` (system-owned)
  - When: a coarse time marker only (not forensic)

Constraints:

- No “Left” versus “Removed” distinction in public-facing surfaces by default.
- No actor attribution (no “changed by”).
- Do not present membership history as a storyline or attribution trail.

## Rationale

This preserves exit safety and reduces escalation risk by preventing “who did what to whom” narratives from forming around access changes, while still allowing minimal boundary visibility where confusion would otherwise increase pressure.

## Trade-offs

- Less detail for people seeking enforcement
- Lower conflict evidence value and stronger exit safety defaults

## Guardrails

- Never imply the system removes people abruptly as a moral action. Removal is a boundary change, not punishment.
- Never reveal “who removed whom” by default.
- Do not present membership history as a storyline or attribution trail.

## Review and Supersession

This decision can only be changed via a new decision entry:

- D00X - Membership Boundary Visibility Update (Supersedes D015)
