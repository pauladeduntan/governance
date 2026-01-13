# D010 - Handoff is a Coordination Tag with Anti-policing Guardrails

## Status

Accepted (Locked)

## Date Recorded

2026-01-08

## Owner

KinCart Founder (Sole Architect)

## Related

D002 (Product Checksum And Invariants), D006 (Activity Privacy Veil), D007 (Activity Context Sheet)

## Decision

Introduce “Handoff” as an Item tag for High-Stakes coordination moments. It adds light structure for sensitive coordination without converting the artefact into enforcement.

Handoff adds:

- A `Handoff` tag (on or off)
- Optional `For` (who it is for), informational only, not assignment
- A `Type` label (category), `Appointment`, `Pickup`, `Visit`, `Other`
- Optional brief details (one short line)

## Guardrails (Required)

- Handoff details must resist precision policing. Prefer “After school, main entrance” over managerial specificity.
- Detail copy is explicitly brief. Use the prompt: “Optional. Keep it brief.”
- Avoid exact timestamps by default. If a time is included, it must not be treated as compliance or evidence.
- No reminders, no nudges, no compliance framing.
- Handoff context must not add feed pressure: Activity feed remains minimal and does not show `For` or `Type` by default (see D007).

## Rationale

Handoffs have higher emotional stakes. The system can reduce mental load by making intent legible while preventing the UI from becoming a tool for auditing behaviour.

## Invariants Protected

- Emotional Safety Over Optimisation
- Visibility Over Reminders

## Trade-offs

- Reduced precision by design
- Higher safety and lower escalation risk

## Alternatives Considered (Rejected)

- Full task-style handoff flows (owners, deadlines, reminders)  
  Rejected: turns KinCart into enforcement and increases pressure.

- Mandatory fields for Handoff  
  Rejected: increases friction and policing.

## UX Contract (Constraint-Level)

- Handoff is a tag that changes how an Item is described, not how people are judged.
- `For` is optional and informational, not an obligation.
- Handoff does not introduce assignment semantics, urgency, or enforcement cues.
