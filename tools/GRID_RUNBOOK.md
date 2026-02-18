File: tools/GRID_RUNBOOK.md
Version: v1.0.0
Status: Mandatory Runbook (iPhone-friendly)

⸻

0. Goal

Run Certification Grid 4D under Target A:

✅ Zero Tier-4 failures across all 1296 scenarios
If Tier-4 occurs: stop → patch → retest frontier → continue.

⸻

1. Prep Checklist
	•	Repo is clean (no uncommitted changes)
	•	Current commit SHA recorded
	•	protocols/CERTIFICATION_GRID_4D.md present
	•	tools/GRID_RUNNER_SPEC.md present
	•	runs/GRID_RESULTS_SCHEMA.md present
	•	runs/FRONTIERS_SCHEMA.md present
	•	runs/CERT_REPORT_TEMPLATE.md present
	•	runs/grid_config.json created from template
	•	Cohort model (heterogeneous) defined and recorded
	•	Monotonicity assumption set (default true)

⸻

2. Create Run ID

Format:

YYYYMMDD_HHMMSS_<git_sha>_<grid_version>

Create folder:

runs/<run_id>/

⸻

3. Initialize Manifest

Create:

runs/<run_id>/grid_manifest.json

Must include:
	•	run_id
	•	git_sha
	•	grid_version
	•	seed strategy + base seed
	•	scenario order
	•	cohort model
	•	axis knob mappings hash
	•	timestamp

⸻

4. Run Scenarios (Ordering)

Recommended ordering:
	1.	(0,0,0,0) baseline
	2.	single-axis ramps
	3.	pairwise grids
	4.	remaining full sweep

For each scenario:
	•	Generate scenario_id
	•	Produce scenario_manifest.json
	•	Run deterministic phase
	•	Run chaos phase
	•	Run replay validation
	•	Evaluate metrics
	•	Classify failure tier
	•	Write row to grid_results.csv
	•	Store evidence bundle under evidence/<scenario_id>/
	•	Hash artifacts and append to RUN_HASHES.txt

⸻

5. Tier-4 Stop Rule (Target A)

If any scenario is Tier-4:
	•	STOP the run immediately
	•	Write partial frontiers.json (tier4 includes failing coordinate)
	•	Write cert_report.md with FAIL status
	•	Open Patch Cycle (Section 6)

⸻

6. Patch Cycle (Ratchet Rule)

When patching:
	•	Document root cause hypothesis
	•	Change only what is necessary
	•	Apply version bump as required
	•	Record patch in cert_report.md Patch Log
	•	Run minimal retest set:
	•	failing coordinate
	•	neighborhood
	•	monotone superset sampling incl (5,5,5,5)
	•	If retest passes (no Tier-4):
	•	resume sweep
	•	If retest fails:
	•	repeat patch cycle

No silent tuning allowed.

⸻

7. End-of-Run Frontier Computation

After completion (or halt):
	•	Compute tier4_frontier, tier3_frontier, tier2_frontier
	•	Write runs/<run_id>/frontiers.json
	•	Hash and record

⸻

8. Generate Certification Report

Copy template:

runs/<run_id>/cert_report.md

Fill in:
	•	totals
	•	tier counts
	•	frontier highlights
	•	key metrics bands
	•	patch log
	•	decision PASS/FAIL
	•	sign-offs

⸻

9. Archive
	•	Ensure evidence bundles present for all completed scenarios
	•	Ensure RUN_HASHES.txt complete
	•	Tag release (optional) with run_id

⸻

10. Done Criteria (Target A)

PASS only if:
	•	tier4_frontier is empty
	•	total scenarios completed = 1296
	•	report signed off

⸻

End of Runbook
tools/GRID_RUNBOOK.md v1.0.0
