# Decision Hygiene

## Rule 1: Suggestions are Not Truth

Suggestions are inputs. Only committed decisions are truth.

- If it is not written as a Decision Record (and committed), it does not exist.
- If a suggestion conflicts with an invariant, the invariant wins.
- If a suggestion improves speed but increases emotional risk, reject it.

## Rule 2: The 3-Question Filter

Run this before any change is accepted:

1) What is the user-facing behaviour?
2) What is the failure mode if it breaks?
3) What invariant does it protect?

If you cannot answer all three clearly, stop and turn it into a decision or an open question, not an accepted change.
