CRISIS_COMMUNICATIONS_PROTOCOL.md

File: protocols/CRISIS_COMMUNICATIONS_PROTOCOL.md
Version: v1.0.0
Status: Mandatory Trust Layer

⸻

1. Purpose

Defines how system state is communicated during:
	•	DSM activation
	•	ARP guardrail triggers
	•	Settlement stress
	•	Misinformation attacks

Goal:

Transparency without panic amplification.

⸻

2. Signed State Verification

All official communications must:
	•	Be cryptographically signed
	•	Be verifiable locally
	•	Never require external link navigation

Users must never be directed to:
	•	“Migration portals”
	•	“Emergency transfers”
	•	External wallet redirects

⸻

3. Three-Tier Transparency Model

Tier 1 — Immediate UX Notice

Displayed when guardrails activate:

“System guardrail active. Essentials protected. Review underway.”

No sensitive details.

⸻

Tier 2 — Public Review Announcement

Within defined window:
	•	Trigger category (not raw metric)
	•	Duration expectation
	•	Confirmation essential access unaffected

⸻

Tier 3 — Outcome Summary

After review:
	•	Activation duration
	•	Impact band
	•	Lessons learned
	•	Parameter adjustments (if any)

⸻

4. Anti-Misinformation Safeguards

4.1 In-App Truth Anchor

Dedicated, signed “System Status” page.

4.2 Scam Inoculation UX

Users periodically reminded:
	•	Never follow external emergency instructions
	•	Never share recovery credentials
	•	Verify signatures locally

4.3 Alert Fatigue Controls
	•	Risk-tier prioritization
	•	Suppress low-confidence alerts
	•	Escalate only high-certainty threats

⸻

5. Offline Verification

Users must be able to:
	•	Verify system signature status offline
	•	Confirm last known valid state
	•	Validate that no unauthorized protocol change occurred

⸻

6. Guiding Principle

Communication must:

Reduce fear.
Increase clarity.
Never amplify rumor.
Never require blind trust.

⸻

End of Document

⸻
