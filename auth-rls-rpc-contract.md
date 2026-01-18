# Access Boundary Contract (Drift Guardrail)

## Non-Negotiable

Access boundary enforcement and privileged action semantics must never drift. If they drift, we create correctness and security rework and erode emotional safety through boundary violations and exit safety failures.

## Rules

1) Privileged Household-scoped actions must always verify the actor from the current session, not from client input:
   - Actor identity is derived from the current session.
   - The system never accepts an actor identifier supplied by the client as an authority value.
   - The system verifies active membership for the target Household boundary.
   - The system fails closed on any mismatch.

2) Client-provided identifiers are never trusted by default:
   - Household and object identifiers may be passed for routing.
   - The system re-derives the owning Household boundary from authoritative relationships.
   - The system re-checks active membership before accepting any read or change.

3) Normalization is system-owned:
   - The system computes normalization used for equivalence and deduplication.
   - The client never supplies normalization values as authoritative inputs.

4) Boundary enforcement is always enabled in any environment with real participant data:
   - No permissive access exceptions are allowed in environments where any real participant data exists.
   - Any temporary relaxation for private development must never be used in public demos, shared environments, or participant-facing study contexts.
   - Enforcement semantics must match the same membership, boundary integrity, and exit safety rules across the system.

5) Exit safety includes identity rendering constraints:
   - When membership ends, access is revoked immediately.
   - Identity display is system-owned and must dynamically re-render historical Activity and context views to “Former Member” by default after membership ends.

## Required Semantics (Household-Scoped Actions)

Every Household-scoped privileged action must follow the same semantic order:

- derive actor identity from the current session
- re-derive the owning Household boundary from authoritative relationships
- verify active membership for that boundary
- execute the intended behaviour

This describes semantic requirements, not a code template.

## Verification Gate

No change is treated as complete unless verification confirms:

- boundary enforcement is enabled in the target environment(s) used for study or review
- privileged actions consistently verify active membership and fail closed
- boundary integrity and exit safety behaviours match the Blueprint constraints
- identity rendering after exit matches the “Former Member” default
