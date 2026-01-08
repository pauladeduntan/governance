# D013 — Auth is framed as “Save progress” (guest is first-class)

Date: 2026-01-08
Status: Accepted
Owner: System (KinCart)

## Decision
User-facing auth language is framed as "Save progress" rather than "Create account".

- Primary framing: Save progress
- Guest mode remains first-class and visible.
- "Create account" language is avoided on Landing; if present at all, it appears as a small link on the sign-in screen (not a primary CTA).

## Rationale
KinCart is a research-led prototype where pressure to sign up increases friction and undermines emotional safety. Saving progress is the honest utility.

## Invariants Protected
- Reduce mental load
- Avoid conversion pressure mechanics

## Trade-offs
- Slightly less conventional onboarding
- Requires clear explanation that Save progress = sign-in for cross-device continuity

## UX Contract
- Landing offers: Continue as guest (primary path) + Save progress (secondary path).
- Save progress uses provider sign-in (Apple/Google/email) without marketing framing.
