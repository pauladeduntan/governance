# D015 - Membership Changes are Access-boundary Events, not Narratives

## Status

Accepted (Locked)

## Date Recorded

2026-01-08

## Owner

KinCart Founder (Sole Architect)

## Context

Membership changes can become evidence in household conflict if framed as blame, attribution, or narrative. KinCart treats membership as an access boundary, not a social storyline.

## Decision

Membership changes are represented, when shown, as system-owned access-boundary events with minimal, neutral copy.

A membership boundary detail sheet, if presented, must include:

- Title: `Membership Ended` or `Member Joined`
- Body line: `Access Ended Immediately.`
- Fields:
  - Member: `Former Member` (system-owned)
  - Change Type: `Left` or `Removed` (system-owned), with no actor attribution
  - When: a coarse time marker only (not forensic)

Default visibility constraint:

- Membership boundary events must not be presented in the Activity feed by default.
- If membership boundary events are ever introduced into Activity surfaces, it requires an explicit new decision that preserves low evidence value and exit safety.

## Rationale

This preserves exit safety and reduces escalation risk by preventing “who did what to whom” narratives from forming around access changes.

## Trade-offs

- Less accountability detail for people seeking enforcement
- Stronger emotional safety and neutrality

## Guardrails

- Never imply the system removes people abruptly as a moral action. Removal is a boundary change, not punishment.
- Never reveal “who removed whom” by default.
- Do not present membership history as a storyline or attribution trail.
