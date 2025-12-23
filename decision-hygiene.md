# Decision Hygiene

## Rule 1: Suggestions are not truth
Suggestions are inputs; only committed decisions are truth.

- If it is not written as a decision (and committed), it does not exist.
- If a suggestion conflicts with an invariant, the invariant wins.
- If a suggestion improves speed but increases emotional risk, reject it.

## Rule 2: The 3-question filter (run before every build step)
Before implementing anything, answer:

1) What is the user-facing behaviour?
2) What is the failure mode if it breaks?
3) What invariant does it protect?

If you can’t answer all three clearly, stop and turn it into a decision or a question—not a build step.
