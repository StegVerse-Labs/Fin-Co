File: protocols/PATCH_RATCHET_PROTOCOL.md
Version: v1.0.0
Status: Mandatory Discipline Rule

⸻

1. Purpose

Prevents weakening of invariants under pressure.

Defines how patches:
	•	Move resilience frontier outward
	•	Never shrink guaranteed operating region
	•	Never introduce hidden authority

⸻

2. Ratchet Principle

Every patch must satisfy:

The set of coordinates that pass without Tier-4 must strictly expand or remain unchanged.

It may not contract.

⸻

3. Versioning Rules

Tier-4 structural flaw

→ Minor or Major version bump required.

Invariant change

→ Major version bump required.

Threshold tuning only

→ Minor version bump required.

No patch without version increment.

⸻

4. Minimal Retest Set

After patch:
	•	Re-run failing coordinate
	•	Re-run its Chebyshev-1 neighborhood
	•	Re-run (5,5,5,5)
	•	Re-run any previously Tier-3 frontier coordinates

Only after passing may grid resume.

⸻

5. Invariant Hardening

If Tier-4 relates to invariant breach:
	•	Invariant must be tightened, not loosened.
	•	Loosening requires explicit governance review and major version bump.

⸻

6. No Compensatory Drift

You may not:
	•	Weaken one guardrail to strengthen another.
	•	Increase emergency duration to reduce buffer strain.
	•	Introduce discretionary authority to improve response speed.

Tradeoffs must preserve invariants.

⸻

7. Audit Trail

Each patch must include:
	•	patch_id
	•	pre_patch_frontier
	•	post_patch_frontier
	•	frontier_delta
	•	ratchet_verified: true/false

⸻

8. Stop Condition

If three consecutive patch cycles fail to eliminate a Tier-4 at the same coordinate:

Escalate to:
	•	Architectural redesign review
	•	Invariant review session
	•	External review consideration

⸻

9. Guiding Principle

Resilience must compound.
Authority must not.

⸻

End of Document
