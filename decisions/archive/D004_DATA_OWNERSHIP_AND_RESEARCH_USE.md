# D004 - Data Boundaries, Research Use, and Ethical Posture

## Status

Accepted (Active, Non-Negotiable)

## Context

KinCart is a non-commercial research artefact exploring Household coordination in HCI/CSCW. This decision defines data boundaries, research use constraints, and collaboration posture to constrain **visibility-to-enforcement drift** and avoid ambiguity, misrepresentation, and safety drift.

Mental load reduction is treated as a checksum aim, not a reported outcome.

## Decision

### 1) Intellectual Property and Artefact Ownership

- The KinCart founder retains ownership of the artefact’s design work, written materials, and any implementation created by the founder.
- Public repositories contain research governance and public-safe artefacts, not implementation recipes.
- Peer review and collaborative learning contributions do not transfer IP or create ownership, licensing rights, or derivative claims.

### 2) Data Minimisation and Collection Boundaries

- KinCart is designed to minimise collection of sensitive personal data.
- The artefact must not collect or store financial transaction data, precise location data, health data, or legally sensitive identifiers as a research dependency.
- The artefact must not depend on surveillance patterns (for example, inactivity tracking, read receipts, or per-person monitoring).
- Exit safety is a data and identity constraint: when membership ends, access is revoked immediately and identity exposure is minimised (including dynamic re-rendering to “Former Member” by default in Activity and context views).
- Any data captured for research purposes must be the minimum necessary and must be explicitly documented in the Blueprint or a governance decision before collection occurs.

### 3) Research use and Publication Boundaries

- KinCart may be referenced publicly and academically as a research artefact, not as a commercial product or service.
- Research outputs must not publish user-identifiable data.
- Participant contact details, consent forms, recordings, transcripts, and any directly identifying materials must be stored outside public repositories under appropriate access controls.
- Any future study involving participants must follow appropriate ethics and consent processes as required by the host institution or review body.

### 4) Non-commercial Boundary

- KinCart remains non-commercial while under this decision.
- No selling access, monetisation experiments, or commercial contracts.
- Any reframing toward commercial or service delivery posture requires an explicit superseding decision.

### 5) Collaboration Boundary

- Collaborators participate as peer reviewers or for collaborative learning only.
- No milestones, deadlines, output expectations, or employment-like evaluation.
- Collaboration does not change IP ownership or relax data and ethics boundaries.

## Implications

- Public communication defaults to research artefact framing and avoids commercial vocabulary.
- Public artefacts must avoid roadmap and delivery language (for example, MVP, post-MVP, rollout, scaling).
- Any change that expands data capture or study posture requires an explicit decision record that states what is collected, why it is necessary, and how emotional safety and exit safety are protected.
- If a proposal amplifies surveillance interpretation risk, it is rejected or redesigned.

## Related Decisions

- D001 - Project Framing: Research-Led, Non-Commercial Artefact
- D002 - Product Checksum And Non-Negotiable Invariants
- D003 - Current Research Prototype Boundary And Explicit Exclusions

## Review and Supersession

This decision may only be changed by a new entry:

- D00X - Data Boundaries And Research Use Update (Supersedes D004)
