# Access Boundary Contract (Drift Guardrail)

## Non-Negotiable

Access boundary enforcement and privileged action semantics must never drift. If they drift, we create correctness and security rework and erode emotional safety through boundary violations and exit safety failures.

## Rules

1) Privileged household-scoped actions must always verify the actor from the session, not from client input:
   - the actor identity is derived from the current session
   - the system never accepts an actor identifier supplied by the client as an authority value
   - the system verifies active membership for the target Household boundary
   - the system fails closed on any mismatch

2) Client-provided identifiers are never trusted by default:
   - Household and object identifiers may be passed for routing
   - the system must re-derive the owning Household boundary from authoritative relationships
   - the system must re-check active membership before accepting any read or change

3) Normalization is system-owned:
   - the system computes normalization used for equivalence and deduplication
   - the client never supplies normalization values as authoritative inputs

4) Boundary enforcement is always enabled in any shared environment:
   - no permissive access exceptions are allowed in environments where any real participant data exists
   - any temporary relaxation for private development must never be used in public, shared, or participant-facing contexts
   - enforcement semantics must match the same membership, boundary integrity, and exit safety rules across the system

## Required Pattern (Household-Scoped Actions)

Every household-scoped privileged action must start by:

- deriving the actor identity from the current session
- re-deriving the owning Household boundary from authoritative relationships
- verifying active membership for that boundary
- then executing the intended behavior

## Verification Gate

No change is treated as complete unless verification confirms:

- boundary enforcement is enabled in the target environment
- privileged actions consistently verify active membership and fail closed
- boundary integrity and exit safety behaviors match the Blueprint constraints
