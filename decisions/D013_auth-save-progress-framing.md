# D013 - Auth is Framed as “Save Progress” (Guest is First-Class)

## Status

Accepted (Locked)

## Date Recorded

2026-01-08

## Owner

KinCart Founder (Sole Architect)

## Decision

User-facing auth language is framed as “Save Progress” rather than “Create Account”.

- Primary framing: Save Progress
- Guest entry remains first-class and visible.
- “Create Account” language is avoided on Entry. If it appears at all, it is a small link on the sign-in screen, not a primary call to action.

## Rationale

KinCart is a research artefact. Sign-up pressure can be read as conversion intent and can invite surveillance and “gated access” interpretations that conflict with emotional safety. “Save Progress” communicates the utility: optional persistence. This constraint also constrains **visibility-to-enforcement drift** by preventing onboarding from becoming a pressure surface.

## Invariants Protected

- Emotional Safety Over Optimisation
- Visibility Over Reminders
- Avoid pressure and conversion framing

## Trade-offs

- Slightly less conventional onboarding
- Requires clear explanation that Save Progress enables cross-device continuity and persistence

## UX Contract (Constraint-Level)

- Entry offers: Continue As Guest (primary path) and Save Progress (secondary path).
- Save Progress uses neutral sign-in options without marketing framing or urgency cues.

## Review and Supersession

This decision can only be changed via a new decision entry:

- D00X - Auth Framing Update (Supersedes D013)
