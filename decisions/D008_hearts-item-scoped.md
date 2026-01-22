# D008 - Hearts are Item-Scoped, not a Feed Mechanic

## Status

Accepted (Locked)

## Date Recorded

2026-01-08

## Owner

KinCart Founder (Sole Architect)

## Related

D006 (Activity Privacy Veil), D007 (Activity Context Sheet)

## Decision

“Hearts” are a lightweight appreciation signal that attaches to an Item. Hearts must not attach to a person and must not become a feed mechanic.

- Hearts live on the Item within the Shared Cart surface.
- Hearts are not displayed as a public score.
- No leaderboards, no ranking, no “most loved” framing.
- No default Heart counts on list rows.
- Hearts must not appear as Activity events and must not introduce social-feed dynamics into Activity.

If Hearts are surfaced beyond the Item, they appear only in an intentional, separate view that lists hearted Items without ranking.

## Rationale

Gratitude is socially high-risk when it becomes currency. This constraint set limits status signalling and constrains **visibility-to-enforcement drift** by preventing appreciation from becoming comparison, obligation, or monitoring interpretation.

## Invariants Protected

- Emotional Safety Over Optimisation
- Visibility Over Reminders
- Activity Is Not A Performance Feed

## Trade-offs

- Less immediate feedback on the main list
- More intentionality (an extra step to view Hearts context)
- Reduced risk of gratitude turning into comparison or obligation

## Alternatives Considered (Rejected)

1) Hearts attributed to people (for example, “Sam received 5 Hearts”)  
   Rejected: becomes social currency and status.

2) Hearts as an Activity event (for example, “Priya hearted Milk”)  
   Rejected: turns Activity into a social feed and amplifies surveillance interpretation.

3) Heart counts visible on every row by default  
   Rejected: invites scorekeeping and comparison.

## UX Contract (Constraint-Level)

- Action: a Member can heart or unheart an Item.
- Representation: a simple hearted state is allowed, but counts must not be shown by default on list rows.
- If a Hearts view exists, it lists hearted Items without ranking.

## Notes

“Coral” is a styling attribute, not domain language. The label is “Hearts”.

## Review and Supersession

This decision can only be changed via a new decision entry:

- D00X - Hearts Constraint Update (Supersedes D008)
