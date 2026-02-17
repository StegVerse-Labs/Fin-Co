# Protocol Requirements — Fin-Co

All implementations must enforce invariant constraints programmatically.

---

## PR-01: Survival Rail Isolation
Separate economic rails must prevent speculative contamination.

---

## PR-02: Entropy Enforcement
Capital Entropy mechanisms must remain active at all times, including during GDE.

---

## PR-03: Temporal Buffering
Protected markets must use batch clearing or latency-neutral mechanisms.

---

## PR-04: Agent Mandate Enforcement
AI agents must:
- Operate under signed mandate contracts
- Log value flows
- Remain revocable

---

## PR-05: Emergency Logging
All GDE invocations must emit:
- Public GDR
- Sunset timestamp
- Restoration trigger

Minimal emergency record fallback required if infrastructure fails.

---

## PR-06: Predictive Neutrality
Simulation outputs may not directly alter solvency conditions or market positioning without governance approval.
