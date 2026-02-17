Consent Integrity Layer — Human Decision Protection Framework

Version: v1.0.0
Applies To: Fin-Co v1.5.0+
Status: Mandatory Protective Constraint
Scope: User consent, transfer authorization, coercion resistance, social engineering defense

⸻

1. Purpose

The Consent Integrity Layer protects users from:
	•	Coercion
	•	Social engineering
	•	Deepfake impersonation
	•	Fraud manipulation
	•	Panic-driven misjudgment
	•	High-pressure transfer scenarios

Cryptographic security protects keys.
Consent integrity protects decisions.

⸻

2. Core Principle

Authorization must be intentional, legible, reversible (when safe), and resistant to psychological manipulation.

The system MUST protect human judgment without replacing it.

AI may advise.
AI may not override.

⸻

3. Consent Protection Objectives

The system MUST:
	•	Reduce irreversible harm from manipulated consent.
	•	Introduce friction proportional to risk.
	•	Preserve user agency.
	•	Avoid paternalistic blocking.
	•	Maintain dignity under stress.
	•	Avoid creating surveillance scoring regimes.

⸻

4. Risk-Tiered Transfer Friction Model

All transfers MUST be classified into risk tiers.

4.1 Risk Factors (Non-Exhaustive)
	•	Transfer size relative to balance
	•	Vault-to-pocket movement
	•	First-time recipient
	•	Recently changed recipient address
	•	Cross-epoch unfamiliar pattern
	•	Time-of-day anomaly
	•	Rapid successive transfers
	•	External flagged scam patterns (federated alerts)

No single factor triggers blocking.

⸻

4.2 Risk Tiers

Tier 0 — Routine
	•	Small pocket transaction
	•	Frequent recipient
	•	Low anomaly

Friction:
	•	Standard confirmation only

⸻

Tier 1 — Elevated
	•	Moderate amount
	•	New recipient
	•	Slight anomaly

Friction:
	•	Human-readable recipient verification
	•	Explicit “why this is elevated” explanation
	•	5–15 second reflection delay

⸻

Tier 2 — High Risk
	•	Large % of vault
	•	First-time vault drain
	•	Pattern matches known scam template

Friction:
	•	Mandatory reflection delay (configurable 1–24 hours)
	•	AI advisory explanation
	•	Optional “delay by default” toggle

AI must explain:
“Large transfer relative to your history.”

⸻

Tier 3 — Extreme
	•	Near-total vault drain
	•	High anomaly + external scam pattern
	•	Coercion indicators (rapid forced behavior)

Friction:
	•	Time-delay enforced
	•	Optional trusted contact confirmation
	•	Duress mode prompt available

AI must not block.
User may override after delay.

⸻

5. Human-Readable Recipient Verification

All transfers MUST display:
	•	Recipient alias (if exists)
	•	Human-readable fingerprint
	•	Visual confirmation code
	•	Optional QR visual confirmation

This prevents address substitution attacks.

Raw addresses alone are insufficient.

⸻

6. Default Delay for Vault Drains

Vault-to-pocket movements above defined threshold MUST:
	•	Trigger delay
	•	Require second confirmation
	•	Provide risk explanation

Delay window MUST be:
	•	User configurable
	•	Bounded by protocol maximum

Immediate irreversible vault drains are prohibited.

⸻

7. AI Advisory Constraints

AI entity MAY:
	•	Explain risk
	•	Simulate outcomes
	•	Suggest delay
	•	Show historical context
	•	Offer scam education

AI entity MUST NOT:
	•	Block transfer
	•	Modify transfer
	•	Escalate to authority
	•	Assign risk score
	•	Penalize future privileges

No hidden scoring allowed.

⸻

8. Anti-Scam Pattern Layer

Federated learning MAY detect scam patterns.

If pattern detected:
	•	Users receive alert
	•	Alert includes explanation
	•	No identity of reporter disclosed
	•	No centralized reporting authority required

Participation in pattern sharing MUST remain opt-out.

⸻

9. Duress and Coercion Response

9.1 Duress Indicators

System MAY detect:
	•	Rapid sequential attempts
	•	Sudden vault drain attempts
	•	Device biometrics mismatch
	•	Panic interaction patterns

Detection must remain advisory.

⸻

9.2 Duress Mode Trigger

User MAY activate duress mode manually.

Duress mode MUST:
	•	Present decoy wallet
	•	Delay vault access
	•	Not signal activation
	•	Not destroy funds
	•	Require threshold recovery for restoration

⸻

10. Reversibility Principles

If settlement not yet finalized:
	•	User MAY cancel within delay window

If finalized:
	•	No forced reversal authority exists
	•	No admin override
	•	No central freeze

System preserves sovereignty over reversibility convenience.

⸻

11. No Reputation or Behavioral Scoring

The Consent Integrity Layer MUST NOT:
	•	Store user risk scores
	•	Influence multiplier
	•	Influence entropy
	•	Influence buffer eligibility
	•	Affect financial privileges
	•	Rank users
	•	Publicly label risk categories

Protection must never evolve into classification.

⸻

12. Consent Auditability

All high-tier friction events MUST:
	•	Log reason category (not raw telemetry)
	•	Be visible to user locally
	•	Not expose personal patterns publicly
	•	Not create central behavioral archive

User may view:
“Why did I receive this warning?”

⸻

13. Crisis Mode Adaptation

During declared systemic crisis (mechanically triggered):
	•	Risk thresholds MAY temporarily lower
	•	Vault delays MAY extend
	•	AI advisory frequency MAY increase

All adjustments MUST:
	•	Be rule-based
	•	Be time-bound
	•	Be publicly documented
	•	Not require discretionary approval

⸻

14. Prohibited Mechanisms

The following are constitutionally prohibited:
	•	Mandatory AI approval
	•	Automatic transaction blocking
	•	Central fraud override key
	•	Reputation gating
	•	Forced identity exposure
	•	Behavioral risk labeling
	•	Mandatory contact approval for all users

⸻

15. Human Dignity Safeguard

The system MUST:
	•	Avoid moralizing language
	•	Avoid shame-based prompts
	•	Avoid risk-tier labeling
	•	Avoid patronizing tone

Language must remain:

Informational.
Neutral.
Respectful.

⸻

16. Negative Test Matrix

The following MUST fail:
	•	AI blocking transaction unilaterally
	•	Transfer denied due to scoring
	•	Admin reversing transaction
	•	Risk classification affecting multiplier
	•	Coercion trigger revealing itself

The following MUST succeed:
	•	Large transfer triggers delay
	•	Scam pattern prompts appear
	•	User can override after delay
	•	Duress mode hides activation
	•	No permanent behavioral record created

⸻

17. Relationship to Ephemerality Profile

Consent Integrity protects the human layer.

Ephemerality protects the identity layer.

Economic Constitution protects the value layer.

All three operate independently but cohesively.

⸻

18. Guiding Doctrine

Cryptography secures keys.
Ephemerality secures identity.
Consent integrity secures decisions.

No authority overrides sovereignty.
No algorithm replaces agency.
No scoring replaces dignity.

⸻

End of Document
CONSENT_INTEGRITY_LAYER.md v1.0.0
