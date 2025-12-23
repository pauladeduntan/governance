# Auth/RLS/RPC Contract (Drift Guardrail)

## Non-negotiable
Membership checks, RLS policies, and RPC semantics must never drift.
If they drift, we create correctness/security rework and erode emotional safety.

## Rules
1) Any SECURITY DEFINER RPC that reads/writes household data MUST:
   - derive user_id from auth.uid() (never accept user_id from client)
   - verify membership via household_members (is_active = true)
   - fail closed (raise exception / return forbidden) on any mismatch

2) Client-provided identifiers are never trusted by default:
   - household_id, cart_id, item_id may be passed for routing,
     but every RPC MUST re-derive the owning household and re-check membership.

3) Canonicalization is server-owned:
   - the server computes canonical keys (e.g., lower(trim(text)))
   - the client never supplies canonical_key as an authority value

4) RLS stays enabled:
   - RLS is ON for all tables
   - “temporary permissive policies” are allowed only in private dev, never in public/shared environments
   - production policies must match the same membership semantics as RPCs

## Required Pattern (RPC)
Every household-scoped RPC must start with:
- v_user_id := auth.uid()
- lookup household_id from cart/item if needed
- membership EXISTS check
- then the business logic

## Verification Gate
No schema change is “done” unless verification SQL passes and confirms:
- RLS enabled on all tables
- expected policies exist
- RPCs are present and enforce membership checks
