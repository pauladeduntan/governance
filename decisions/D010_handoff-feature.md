# D010 — Handoff is a coordination tag with anti-policing guardrails

Date: 2026-01-08
Status: Accepted
Owner: System (KinCart)
Related: D002 (checksum & invariants), D006 (activity privacy veil)

## Decision
Introduce "Handoff" as an Item tag that adds light structure for sensitive coordination moments without converting the system into enforcement.

Handoff adds:
- A Handoff tag (on/off)
- Optional "For" (who it is for) — not a task assignment
- A Handoff label (category, e.g., Appointment / Pickup / Visit / Other)
- Optional brief details (one short line)

## Guardrails (required)
- Handoff details must resist precision policing:
  Prefer "After school · main entrance" over exact timestamps and managerial specificity.
- Detail copy is explicitly brief:
  "Optional. Keep it brief."
- No reminders, no nudges, no compliance framing.

## Rationale
Handoffs have higher emotional stakes. The system can reduce mental load by making intent legible while preventing the UI from becoming a tool for auditing behaviour.

## Invariants Protected
- Emotional safety > optimisation
- Visibility > reminders

## Trade-offs
- Reduced precision (by design)
- Higher safety and lower escalation risk

## Alternatives considered (rejected)
- Full task-style handoff flows (owners, deadlines, reminders)
  Rejected: turns KinCart into enforcement and increases pressure.
- Mandatory fields for handoff
  Rejected: increases friction and policing.

## UX Contract
- Handoff is a tag that changes how an Item is described, not how people are judged.
- "For" is optional and informational, not an obligation.
