Consent Integrity Layer — Human Decision Protection Framework

Version: v1.1.0
Applies To: Fin-Co v1.5.0+
Depends On:
	•	EPHEMERALITY_PROFILE.md
	•	ECONOMIC_CONSTITUTION.md
	•	VERSIONING_COVENANT.md

Status: Mandatory Protective Constraint

⸻

1. Purpose

The Consent Integrity Layer protects user decision-making in high-friction environments where:
	•	Coercion is plausible
	•	Social engineering is advanced
	•	Deepfake impersonation exists
	•	Device compromise is possible
	•	Panic behavior can cause systemic instability

Cryptographic custody (Economic Constitution) protects value.
Ephemerality (Ephemerality Profile) protects identity.
Consent Integrity protects human judgment.

All three layers are required for system coherence.

⸻

2. Layer Interdependence

This document MUST be interpreted in coordination with:

2.1 Ephemerality Profile
	•	Spend authorizations are ephemeral.
	•	Identity linkage decays.
	•	Telemetry is minimized.
	•	No master override exists.

Consent Integrity must never introduce mechanisms that undermine ephemerality.

⸻

2.2 Economic Constitution
	•	No discretionary override.
	•	Entropy rules remain mechanical.
	•	Backstop triggers are automatic.
	•	No scoring systems permitted.

Consent friction must not alter economic invariants.

⸻

3. Core Principle

Authorization must be intentional, legible, reversible (where safe), and resistant to psychological manipulation.

AI may advise.
AI may not execute, block, or override.

No decision authority may migrate from user to system.

⸻

4. Risk-Tiered Transfer Model (Aligned with Ephemeral Authorization)

All transfers operate within the Ephemeral Authorization constraints defined in EPHEMERALITY_PROFILE.md.

Consent Integrity operates on top of that layer.

⸻

4.1 Risk Factors (Non-Exhaustive)

Risk signals MAY include:
	•	Transfer amount relative to balance
	•	Vault-to-pocket movement
	•	First-time recipient
	•	Address mutation
	•	High anomaly pattern
	•	Federated scam pattern match
	•	Rapid sequential attempts
	•	Cross-epoch unfamiliar behavior (without permanent linkage)

No single signal may cause automatic denial.

⸻

4.2 Risk Tiers

Tier 0 — Routine
	•	Small pocket transaction
	•	Known recipient
	•	No anomaly

Friction:
	•	Standard confirmation

⸻

Tier 1 — Elevated
	•	Moderate anomaly
	•	New recipient
	•	Higher % of pocket

Friction:
	•	Human-readable verification
	•	Explicit explanation
	•	Short reflection delay

⸻

Tier 2 — High Risk
	•	Significant vault drain
	•	Large % of holdings
	•	Scam-pattern correlation

Friction:
	•	Mandatory delay
	•	AI explanation
	•	Optional delay extension
	•	Vault authorization still bound by TTL and cap (Ephemerality Profile §6)

⸻

Tier 3 — Extreme
	•	Near-total vault drain
	•	Multi-signal anomaly
	•	Coercion indicators

Friction:
	•	Enforced time-delay
	•	Duress mode prompt (see §7)
	•	Optional trusted contact confirmation (user-controlled)

AI must not block.
User override remains possible after delay.

⸻

5. Alignment With Ephemeral Authorization

The following MUST remain true:
	•	All spend authority is time-bound (Ephemerality §6).
	•	Consent friction cannot extend beyond authorization TTL.
	•	Delays cannot become de facto permanent freezes.
	•	No consent layer mechanism may require centralized review.

Consent Integrity must not mutate into control authority.

⸻

6. Human-Readable Recipient Verification

To prevent substitution attacks:
	•	Recipient alias or visual fingerprint required
	•	QR visual match recommended
	•	No raw address-only confirmation
	•	Confirmation UX must be stable across epochs

Ephemeral identity rotation must not reduce clarity of recipient verification.

⸻

7. Duress Mode (Cross-Referenced With Ephemerality)

See EPHEMERALITY_PROFILE.md §7.

Consent Integrity requirements:
	•	Duress mode must not reveal activation.
	•	Duress mode must not alter entropy or multiplier.
	•	Duress mode must not create a behavioral record.
	•	Recovery must require threshold keys.

Consent Integrity may prompt duress mode but never auto-activate.

⸻

8. Federated Scam Detection (Privacy-Constrained)

Pattern alerts may be generated via federated learning.

Requirements:
	•	No raw transaction export
	•	No central behavioral scoring
	•	No identity aggregation
	•	Opt-out participation allowed
	•	Alerts must be explanatory

Federated learning must comply with Ephemerality telemetry constraints.

⸻

9. No Reputation, Credit, or Behavioral Scoring

The Consent Integrity Layer MUST NOT:
	•	Store persistent risk profiles
	•	Influence entropy rates
	•	Influence backstop access
	•	Influence multiplier eligibility
	•	Influence group verification
	•	Rank users
	•	Penalize opt-out participants

Protection must never evolve into stratification.

⸻

10. Crisis Mode Adaptation (Mechanical Only)

In declared crisis (see Economic Constitution):
	•	Risk thresholds MAY temporarily lower.
	•	Vault delay windows MAY extend.
	•	Reflection delays MAY increase.

All adjustments MUST:
	•	Be rule-triggered
	•	Be time-bound
	•	Be publicly documented
	•	Not require discretionary review

No “temporary emergency override” may introduce centralized authority.

⸻

11. Consent Auditability (User-Level Only)

Users MUST be able to see:
	•	Why a prompt occurred
	•	Which risk category triggered it
	•	That no score was assigned
	•	That no permanent record was created

System MUST NOT create central consent logs that allow long-term behavior tracking.

⸻

12. Negative Test Matrix (Integrated With Ephemerality)

The following MUST fail:
	•	AI blocking transfer
	•	Admin reversal
	•	Behavioral scoring persistence
	•	Risk tier affecting multiplier
	•	Coercion trigger exposing duress activation
	•	Central authority freezing funds

The following MUST succeed:
	•	Large vault drain triggers delay
	•	Scam pattern prompts appear
	•	User override works after delay
	•	Duress hides itself
	•	No persistent behavior profile exists

⸻

13. Anti-Drift Safeguard

Any proposal that:
	•	Introduces mandatory AI approval
	•	Centralizes risk telemetry
	•	Adds behavior-based privilege
	•	Weakens ephemeral authorization caps
	•	Adds admin freeze capability

Requires:
	•	MAJOR version increment
	•	Formal GDR
	•	Public audit period

No silent modification permitted.

⸻

14. Guiding Doctrine

Cryptography secures keys.
Ephemerality secures identity.
Consent integrity secures decisions.
Entropy secures circulation.
Hybrid buffers secure stability.

No layer may absorb authority from another.

⸻

15. System Coherence Statement

This layer exists to prevent:

Security from becoming coercion.
Protection from becoming classification.
Advisory from becoming authority.

Consent remains human.
Execution remains mechanical.
Identity remains ephemeral.

⸻

End of Document
CONSENT_INTEGRITY_LAYER.md v1.1.0
