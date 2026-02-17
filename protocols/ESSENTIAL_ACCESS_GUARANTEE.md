ESSENTIAL_ACCESS_GUARANTEE.md

File: protocols/ESSENTIAL_ACCESS_GUARANTEE.md
Version: v1.0.0
Applies To: Fin-Co v1.5.0+
Depends On:
	•	ECONOMIC_CONSTITUTION.md
	•	EPHEMERALITY_PROFILE.md
	•	CONSENT_INTEGRITY_LAYER.md
	•	VERSIONING_COVENANT.md

Status: Mandatory Moral + Systemic Constraint

⸻

1. Purpose

This document ensures StegVerse-aligned financial systems cannot create conditions where living beings lose access to necessities for life due to:
	•	Liquidity throttles
	•	Stability guardrails
	•	Network partitions
	•	Panic dynamics
	•	Algorithmic constraints
	•	Governance drift

Discomfort and friction may exist.

Necessity denial must not.

⸻

2. Core Invariant

Baseline access to life-sustaining goods and services MUST be preserved under all systemic stability modes.

This guarantee applies regardless of:
	•	political conditions
	•	market volatility
	•	capital flight
	•	participation level
	•	group membership
	•	opt-out status

⸻

3. Definitions

3.1 Necessities for Life (Essential Categories)

“Essential” is defined as access to:
	1.	Food and potable water
	2.	Medical care and essential prescriptions
	3.	Shelter and basic housing payments
	4.	Energy and heating/cooling necessary for habitation
	5.	Critical transportation required for access to (1–4)

This is a bounded set.

All expansions require major version change.

⸻

3.2 Essential Access Floor (EAF)

The Essential Access Floor is a protocol-defined minimum throughput that must remain available during systemic throttling events.

EAF is expressed as:
	•	A maximum essential spend allowance per user per epoch (floor guarantee)
	•	A maximum essential transaction count per epoch (abuse control)
	•	A settlement priority rule (if settlement exists)

⸻

3.3 Essential Merchant / Provider

An “Essential Provider” is a merchant or service provider that has been classified into an essential category via one of:
	•	Verified provider enrollment (preferred)
	•	Community attestation quorum (fallback)
	•	Emergency provisional classification (strictly time-bounded)

No single party may classify a provider unilaterally.

⸻

4. Guarantee Behavior Under Systemic Guardrails

When systemic stability guardrails activate (reserve depletion, settlement risk, network partition, panic velocity):

4.1 What MAY be throttled
	•	Vault → Pocket issuance rates
	•	Non-essential transaction multipliers
	•	Non-essential incentive payouts
	•	Non-essential settlement priority

4.2 What MUST NOT be throttled below EAF
	•	Essential-provider payments up to the EAF
	•	Essential transaction settlement (where applicable)
	•	Essential-provider receipt verification flow

Essential access is priority-protected.

⸻

5. Essential Channel Mechanics (Non-Discretionary)

5.1 Two-Lane Model

The system MUST implement:
	•	Essential lane (protected floor)
	•	General lane (subject to stability throttles)

No user must request special permission to use the essential lane.

The essential lane applies automatically to essential providers.

⸻

5.2 Essential Lane Funding Source

Essential payments MUST be sourced from:
	•	Pocket balances first
	•	Then emergency pocket top-up within EAF constraints
	•	Then limited vault issuance inside EAF

Under no circumstances should essential access require full vault unlock.

⸻

6. Anti-Abuse Safeguards

Essential access cannot become an exploit channel.

The system MUST include:

6.1 Caps
	•	EAF per user per epoch cap
	•	Essential transaction count cap
	•	Provider-side receipt volume anomaly detection (advisory)

6.2 No Incentive Boosting
	•	Essential-lane transactions MUST NOT receive enhanced distribution multipliers.
	•	Essential-lane transactions MUST NOT be used to qualify for group multiplier increases.

Essential is for survival, not optimization.

6.3 Provider Attestation Integrity

Provider classification MUST require:
	•	Multi-party attestation
	•	Epoch-bound renewal
	•	Revocation by objective criteria (fraud evidence thresholds)

No political or discretionary revocations.

⸻

7. Consent Integrity Alignment

All essential-lane payments MUST still comply with:
	•	Human-readable recipient verification (Consent Layer)
	•	Risk-tier friction (Consent Layer)

However:

Risk friction may not prevent essential payments within EAF.

If Tier 2–3 friction triggers during essential payment:
	•	A minimal “confirm twice” flow may apply
	•	Long delays must not apply if it blocks immediate essential need
	•	Duress mode prompt may appear

This requires careful UX: protect without denying.

⸻

8. Ephemerality Alignment

Essential provider identities must be:
	•	Ephemeral in public reporting
	•	Stable enough for user verification

Requirements:
	•	Providers may have stable local aliases on user device
	•	Public reporting uses banded + delayed metrics
	•	No permanent “essential list” that creates targeting vectors

Essential support must not create a public target registry.

⸻

9. Crisis Mode & Network Partition Behavior

During network outage / partition:
	•	Essential-lane offline payments may proceed within micro-cap limits
	•	Settlement occurs upon reconnection
	•	Offline replay protection remains mandatory (nonces, TTL)

If settlement integrity risk rises:
	•	Essential offline cap may lower
	•	Essential online cap remains at EAF floor

⸻

10. Auditability Without Targeting

Public reporting MUST provide:
	•	Aggregate essential-lane volume bands
	•	Essential-lane event counts
	•	No provider list
	•	No community label linkage across epochs

Auditable systems, opaque targets.

⸻

11. Negative Test Matrix

MUST FAIL
	•	Essential classification by a single admin
	•	Essential lane used to increase incentives
	•	Essential lane used to bypass caps
	•	Public reporting revealing stable essential-provider identities
	•	Throttles denying essential payments below EAF

MUST SUCCEED
	•	Essential payments continue during systemic throttle up to EAF
	•	Essential lane honors recipient verification
	•	Essential lane maintains replay protection
	•	Essential classification is multi-party and epoch-bound
	•	Essential lane does not create new targeting vectors

⸻

12. Anti-Drift Safeguard

Any proposal that:
	•	Removes EAF
	•	Adds discretionary essential approvals
	•	Allows essential-lane incentives
	•	Publishes stable essential-provider lists
	•	Introduces “special permission” for essentials

Requires:
	•	Major version increment
	•	Formal GDR
	•	Public review period

⸻

13. Guiding Doctrine

A system that protects money but denies life is incoherent.

StegVerse financial coherence requires:
	•	Sovereignty without confiscation
	•	Stability without control
	•	Protection without surveillance
	•	Resilience without denial of essentials

⸻

End of Document
ESSENTIAL_ACCESS_GUARANTEE.md v1.0.0
