Decision D006: Activity privacy veil (readable record, not surveillance feed)

Status: Accepted (LOCKED)  
Date recorded: 2026-01-08  
Owner: KinCart system (sole architect)

Context

Activity feeds in household apps commonly drift into:
⦁	surveillance (“who did what”)
⦁	scorekeeping (“who contributes”)
⦁	conflict evidence (“proof”)
KinCart needs Activity for visibility of shared intent, while preventing escalation dynamics.

Decision

1.	Activity is a readable record of shared intent, not a performance feed.
⦁	No “streaks”, “top contributors”, badges, or leaderboards.
2.	Default attribution is low-pressure.
⦁	Routine item actions may show a name (Member display name).
⦁	High-risk events (membership changes, removals) are system-owned and non-attributed by default.
3.	Event copy avoids moral framing.
⦁	Use neutral verbs: added, completed, showed again, hidden, membership ended, member joined.
⦁	Avoid “failed”, “missed”, “late”, “responsible”, “should”.
4.	Detail sheets exist to clarify coordination—not to increase auditability.
⦁	Details show the minimum needed to understand the intent and reverse mistakes.
⦁	Details never reveal actor attribution for removals by default.
5.	Exit safety overrides “history completeness”.
⦁	When membership ends, preserve Household continuity while de-identifying the former member.

Rationale

⦁	Activity should reduce ambiguity without creating pressure.
⦁	Lower “evidence value” reduces conflict risk.
⦁	Supports invariant: visibility > reminders and emotional safety > optimisation.

Implications

⦁	Some users will want stronger attribution; KinCart intentionally does not prioritize that in the probe.
⦁	Research protocols should explicitly probe how people react to reduced attribution.

Acceptance criteria

⦁	No UI computes or displays “contribution” metrics.
⦁	Membership events show system-owned copy and avoid naming the actor who removed someone.
⦁	Detail sheets are informational and reversible, not accusatory.
