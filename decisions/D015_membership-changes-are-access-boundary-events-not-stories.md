# D015 — Membership changes are access-boundary events, not narratives

Date: 2026-01-08
Status: Accepted

## Context
Membership events can become “evidence” in household conflict if framed as blame or attribution.

## Decision
Membership detail sheet must include:
- Title: “Membership ended” (or “Member joined”)
- Body line: “Access ended immediately.”
- Fields:
  - Member: “Former member” (system-owned)
  - Change type: Left / Removed (no actor attribution)
  - When: …

## Rationale
Preserves exit safety and reduces social escalation risk.

## Trade-offs
- Less “accountability detail” for admins.
- Stronger emotional safety and neutrality.

## Guardrails
Never imply the system removes people “abruptly”; removal is a boundary change, not a moral action.
