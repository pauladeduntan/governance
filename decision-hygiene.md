# Decision Hygiene

## Rule 1: Suggestions are not Truth

Suggestions are inputs. Only committed decisions are truth.

- If it is not written as a Decision Record (and committed), it does not exist.
- If a suggestion conflicts with an invariant, the invariant wins.
- If a suggestion improves speed but increases emotional risk, reject it.
- Public artefacts must not include implementation recipes or roadmap language.

## Rule 2: The 3-Question Filter

Run this before any change is accepted:

1) What is the user-facing behaviour?
2) What is the failure mode if it breaks?
3) What invariant does it protect?

If you cannot answer all three clearly, stop and turn it into a Decision Record or an Open Question, not an accepted change.

## Rule 3: Activity Drift Check

Any change that touches Activity or identity display must explicitly answer:

- Does this increase performance-feed interpretation risk (per-person views, counts, sorting, grouping, filtering, badges, streaks, or similar)?
- Does this increase identity exposure risk after exit, or break dynamic redaction to “Former Member” by default?
