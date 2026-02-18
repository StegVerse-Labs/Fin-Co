Resilience Certification Report
	•	Run ID: <run_id>
	•	Grid Version: <grid_version>
	•	Repo / Commit: <repo_url_or_name> / <git_sha>
	•	Certification Target: A (Zero Tier-4 across 1296 scenarios)
	•	Monotonicity Assumption: <true|false>
	•	Scenario Order: <ordering_strategy>
	•	Seed Strategy: <strategy> (base: <base_seed>)

⸻

1. Executive Summary
	•	Total Scenarios Expected: 1296
	•	Total Scenarios Completed: <n_completed>
	•	Tier-4 Count: <tier4_count>
	•	Tier-3 Count: <tier3_count>
	•	Tier-2 Count: <tier2_count>
	•	PASS Target A: <true|false>

First Tier-4 (if any)
	•	Scenario: <scenario_id> (S1=<a>, S2=<b>, S3=<c>, S4=<d>)
	•	Failure Type: <first_failure_type>
	•	Time to Failure (epochs): <t>

⸻

2. System Build & Configuration

2.1 Grid Config
	•	runs/grid_config.json hash: <sha256>
	•	Notes on knob mappings (if any deviation from template):
	•	<bullet list>

2.2 Cohort Model
	•	Archetype mix: <A% / B% / C% / D% / E%>
	•	Regions simulated: <count>
	•	Notes: <short>

⸻

3. Evidence Artifacts
	•	grid_manifest.json hash: <sha256>
	•	grid_results.csv hash: <sha256>
	•	frontiers.json hash: <sha256>
	•	Evidence root: runs/<run_id>/evidence/
	•	Overall hashes: RUN_HASHES.txt hash: <sha256>

⸻

4. Frontier Summary

4.1 Tier-4 Frontier (must be empty to pass Target A)
	•	Count: <n>
	•	Coordinates (if any):
	•	<scenario_id> — <failure_type> — t=<epochs>
	•	…

4.2 Tier-3 Frontier
	•	Count: <n>
	•	Key patterns:
	•	<pattern 1>
	•	<pattern 2>

4.3 Tier-2 Frontier
	•	Count: <n>
	•	Key patterns:
	•	<pattern 1>
	•	<pattern 2>

⸻

5. Key Metrics Highlights (Banded)
	•	Min Buffer Reserve Ratio: <band>
	•	Peak Vault→Pocket Velocity: <band>
	•	Max Essential Provider Concentration: <band>
	•	Crisis Signature Verification Rate: <band>
	•	Panic Propagation (B←C): <band>
	•	ARP Review Notice Compliance: <% compliant>
	•	ARP Outcome Publication Compliance: <% compliant>

⸻

6. Findings

6.1 Tier-4 Findings (if any)

For each Tier-4 failure:
	•	Scenario: <scenario_id>
	•	Failure Type: <type>
	•	Root Cause Hypothesis: <short>
	•	Required Patch Category: <protocol|ux|threshold|logging|other>
	•	Ratchet Rule Applied: <yes|no>
	•	Minimal Retest Set Executed: <yes|no>

6.2 Tier-3 Findings
	•	<bullets>

6.3 Tier-2 Findings
	•	<bullets>

⸻

7. Patch Log (If Applied)

Each patch must list:
	•	Patch ID: <id>
	•	Files changed: <paths>
	•	Version bump: <x.y.z>
	•	Rationale: <short>
	•	Frontier moved: <yes/no>
	•	Retest set: <list of scenario_ids>
	•	Outcome: <pass/fail>

⸻

8. Certification Decision
	•	Decision: <PASS|FAIL>
	•	Justification:
	•	<one paragraph>
	•	Next Action:
	•	If FAIL: patch + rerun minimal set + resume sweep
	•	If PASS: proceed to Certification Round 2 (larger cohort / observers)

⸻

9. Sign-Off
	•	Certification Lead: <name> — <date>
	•	Mechanical Auditor: <name> — <date>
	•	Governance Integrity Auditor: <name> — <date>
	•	Red-Team Coordinator: <name> — <date>

Signature (optional): <detached signature or hash>

⸻

End of Template
runs/CERT_REPORT_TEMPLATE.md v1.0.0
