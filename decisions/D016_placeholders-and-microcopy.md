# D016 — Placeholder rules + anti-policing microcopy consistency

Date: 2026-01-08
Status: Accepted
Owner: System (KinCart)

## Decision
Placeholders and microcopy must be consistent and must not encourage policing.

### Item name placeholder rules
- Normal Items:
  - Placeholder examples are simple groceries/household items (e.g., "e.g., Milk" / "e.g., Rice")
- Handoff Items:
  - Placeholder examples may include non-grocery coordination nouns only when Handoff is enabled (e.g., "e.g., Dentist" / "e.g., Pharmacy")

### Details placeholder rules
If Details exists:
- Placeholder is descriptive but brief (e.g., "e.g., 1kg bag" / "e.g., small bottle")
- Microcopy: "Optional. Keep it brief."

### Handoff detail style guide
- Prefer: "After school · main entrance"
- Avoid: exact times and compliance language by default

## Rationale
Users copy what the UI suggests. Placeholders are behavioural design; they must support coordination without turning into audit text.

## Invariants Protected
- Emotional safety > optimisation
- Reduce mental load

## Trade-offs
- Less precision
- Lower conflict risk and better tone integrity
