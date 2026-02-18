File: protocols/FAILURE_ANALYSIS_PLAYBOOK.md
Version: v1.0.0
Status: Mandatory for Certification Cycles

⸻

1. Purpose

Defines how failures discovered during certification are:
	•	Analyzed
	•	Classified
	•	Root-caused
	•	Patched
	•	Retested

Without:
	•	Blame
	•	Narrative protection
	•	Silent tuning
	•	Scope creep
	•	Invariant erosion

⸻

2. Failure Response Rules

Rule 1 — No Defensive Framing

Failures are data.
Never explain them away.
Never reclassify severity to avoid stop conditions.

⸻

Rule 2 — Tier Integrity

If a failure meets Tier-4 criteria under CERTIFICATION_GRID_4D.md, it is Tier-4.

Severity may not be downgraded without:
	•	Documented reasoning
	•	Independent reviewer signoff
	•	Version increment

⸻

Rule 3 — Root Cause Required

Each Tier-3 or Tier-4 failure must produce:
	•	Observable symptom
	•	Invariant implicated
	•	Immediate trigger
	•	Structural cause
	•	Contributing factors
	•	Preventability assessment

⸻

3. Root Cause Template

Each failure must complete:

3.1 Failure Description
	•	Scenario ID
	•	Axis levels
	•	Failure type
	•	Epoch of occurrence

3.2 Trigger Chain

Describe the precise chain:
	•	Input condition →
	•	Guardrail state →
	•	Behavioral amplification →
	•	Final failure

⸻

3.3 Invariant Impact

Which invariant(s) were at risk?
	•	Essential Floor
	•	No Master Key
	•	Bounded Entropy
	•	Expiry Discipline
	•	Identity Blindness
	•	Buffer Floor
	•	Other

⸻

3.4 Structural vs Parametric

Is this:
	•	Parametric weakness (threshold tuning)
	•	Structural flaw (logic gap)
	•	UX-induced vulnerability
	•	Governance drift
	•	Observability failure

Structural flaws require version bump ≥ minor.

⸻

3.5 Patch Strategy Classification

Select one:
	•	Threshold tightening
	•	Additional guardrail
	•	Expiry shortening
	•	UX clarification
	•	Logging enhancement
	•	Architectural change (major version)

⸻

4. Prohibited Responses

The following are not allowed:
	•	Silent parameter tightening
	•	Undocumented emergency extension
	•	Adding admin override
	•	Lowering stress thresholds to avoid failure
	•	Removing scenario from grid

If any occur → automatic Tier-4 under governance failure.

⸻

5. Documentation Discipline

Every failure produces:
	•	failure_report_<scenario_id>.md
	•	Linked to run ID
	•	Linked to patch ID
	•	Cross-referenced in certification report

⸻

6. Learning Log

Maintain cumulative file:

runs/FAILURE_LEARNING_LOG.md

Each entry:
	•	Failure ID
	•	Version
	•	Scenario
	•	Root cause summary
	•	Patch summary
	•	Frontier movement

This builds institutional memory.

⸻

7. Guiding Principle

Failure is permitted.
Invariant erosion is not.

⸻

End of Document
