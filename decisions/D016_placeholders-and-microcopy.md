# D016 - Placeholder Rules and Anti-policing Microcopy Consistency

## Status

Accepted (Locked)

## Date Recorded

2026-01-08

## Owner

KinCart Founder (Sole Architect)

## Decision

Placeholders and microcopy must be consistent and must not encourage policing, surveillance, or compliance framing.

### Item Name Placeholder Rules

- Items:
  - Placeholder examples are simple groceries and household Items (for example, “e.g. Milk” or “e.g. Rice”).

- Handoff Items:
  - Placeholder examples may include non-grocery coordination nouns only when `Handoff` is enabled (for example, “e.g. Appointment” or “e.g. School pickup”).

### Item Details Placeholder Rules

If an Item details field exists on an Item surface:

- Placeholder is descriptive but brief (for example, “e.g. 1kg bag” or “e.g. small bottle”).
- Microcopy prompt: “Optional. Keep It Brief.”

### Handoff Detail Style Guide

- Prefer situational summaries (for example, “After school, main entrance”).
- Avoid exact timestamps and compliance language by default.
- Do not write instructions that read like auditing or enforcement.

## Rationale

Members copy what the interface suggests. Placeholders are behavioural design. They must support coordination without becoming audit text.

## Invariants Protected

- Emotional Safety Over Optimisation
- Reduce mental load
- Visibility Over Reminders

## Trade-offs

- Less precision by design
- Lower conflict risk and better tone integrity
