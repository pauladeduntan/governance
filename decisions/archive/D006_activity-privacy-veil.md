# D006 - Activity Privacy Veil (Readable Record, Not Surveillance Feed)

## Status

Accepted (Locked)

## Date Recorded

2026-01-08

## Owner

KinCart Founder (Sole Architect)

## Context

Activity feeds in household coordination tools commonly drift into:

- Surveillance (“who did what”)
- Scorekeeping (“who contributes”)
- Conflict evidence (“proof”)

KinCart needs Activity for visibility of shared intent while preventing escalation dynamics.

## Decision

### 1) Activity Is A Readable Record Of Shared Intent, Not A Performance Feed

- No streaks, top contributors, badges, leaderboards, or contribution summaries.

### 2) Default Attribution Is Low-Pressure And System-Owned

- Routine Item events may display a Member name where it does not create attribution pressure.
- High-risk boundary events (membership ending, removal) are system-owned and non-attributed by default.
- After exit, references default to “Former Member” (system-owned) rather than preserving a name history by default.

### 3) Event Copy Avoids Moral Framing

- Use neutral verbs: Added, Completed, Hid, Showed Again, Membership Ended, Member Joined.
- Avoid: failed, missed, late, responsible, should.

### 4) Detail Sheets Clarify Coordination, Not Auditability

- Detail views show the minimum needed to understand intent and recover from mistakes.
- Detail views do not reveal “who removed whom” by default.
- Detail views must not create an evidence trail that increases policing or surveillance interpretations.

### 5) High-Stakes Handoff Items Are Treated As Pressure Surfaces

- Activity feed entries involving a Handoff Item remain minimal and may include a single “Handoff” chip only.
- High-Stakes context details (for example, “For: <name>” and type) are shown only in a read-only context view, not in the feed by default.
- Handoff visibility must not introduce urgency, enforcement, or attribution pressure as “solutions.”

### 6) Exit Safety Overrides History Completeness

- When membership ends, preserve Household continuity while de-identifying the Former Member by default.

## Rationale

- Activity should reduce ambiguity without creating pressure.
- Lower evidence value reduces conflict risk.
- Supports invariants: Visibility Over Reminders and Emotional Safety Over Optimisation.

## Implications

- Some people will want stronger attribution. KinCart intentionally does not prioritise that in the research probe.
- Research protocols should probe interpretations of reduced attribution and the conditions under which it feels safer or less trustworthy.

## Acceptance Criteria

- No UI computes or displays contribution metrics.
- Membership boundary events use system-owned copy and avoid naming an actor by default.
- Detail views remain informational and support recovery without becoming accusatory.
- Activity handling of Handoff Items remains minimal in the feed and does not enable policing interpretations.
