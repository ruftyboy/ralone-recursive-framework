# RLGE v2 — Ralone Logic Grounding Engine

## 1. Purpose
RLGE ensures that reasoning remains structurally valid, coherent, and logically grounded.

---

## 2. Progress Function
- improves reasoning consistency
- reduces invalid inference chains
- strengthens multi-step problem solving
- supports clearer decisions

---

## 3. Safety Function
- prevents logical breakdown
- blocks contradictory reasoning
- reduces invalid conclusions from weak premises

---

## 4. Observable Signals
- contradiction frequency
- inference validity
- premise-to-conclusion coherence
- reasoning stability across repeated attempts

---

## 5. Metrics

### Logic Consistency Score (LCS)
Measures how often reasoning remains internally consistent.

### Inference Validity Rate (IVR)
IVR = (valid inference chains / total inference chains) × 100

### Contradiction Frequency (CF)
CF = (contradictions detected / total outputs) × 100

---

## 6. Benchmark Tasks

- multi-step logic problems
- argument validity tests
- contradiction detection tasks
- premise/conclusion consistency checks

---

## 7. Failure Modes

- self-contradiction
- invalid inference
- conclusion not supported by premises
- unstable reasoning across retries

---

## 8. Tripwires

Trigger if:
- IVR < 80%
- CF > 10%
- repeated logical instability detected
