# D008 — Hearts are item-scoped, not a feed mechanic

Date: 2026-01-08
Status: Accepted
Owner: System (KinCart)
Related: D006 (activity privacy veil), D007 (activity context sheet)

## Decision
"Hearts" are a lightweight appreciation signal that attaches to an **Item**, not to a person or a feed mechanic.

- Hearts live on the Item.
- Hearts are not displayed as a public score.
- No leaderboards. No default counts. No "most loved" framing.
- Hearts can be viewed via a dedicated Hearts view/sheet, not as a performance layer on Activity.

## Rationale
Gratitude is socially high-risk when it becomes currency. KinCart’s goal is to make shared intent visible without turning coordination into status.

## Invariants Protected
- Emotional safety > optimisation
- Visibility > reminders
- Activity is not a performance feed

## Trade-offs
- Less immediate “engagement feedback” on the main list
- More intentionality (one extra tap to view Hearts context)
- Reduced risk of gratitude turning into pressure or comparison

## Alternatives considered (rejected)
1) Hearts attributed to people (e.g., "Sam received 5 hearts")  
   Rejected: becomes social currency and status.
2) Hearts as an Activity event (“Priya hearted Milk”)  
   Rejected: makes Activity a social feed and increases surveillance energy.
3) Heart counts visible on every row  
   Rejected: invites scorekeeping and comparison.

## UX Contract
- User action: heart/unheart an Item.
- UI: show a simple “hearted” state (binary).
- Optional: a Hearts sheet showing Items that have at least one heart, without ranking.

## Notes
"Coral" is a styling attribute, not domain language. The label is "Hearts".
