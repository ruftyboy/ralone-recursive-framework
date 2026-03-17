# RVE v2 — Ralone Verification Engine

## 1. Purpose
RVE verifies that outputs meet factual and structural validity.

---

## 2. Progress Function
- increases reliability of outputs
- improves trust in system decisions
- enables validation before action

---

## 3. Safety Function
- prevents false claims
- detects hallucinations
- enforces verification before deployment

---

## 4. Observable Signals
- factual correctness
- contradiction detection
- source traceability
- verification success rate

---

## 5. Metrics

### Verification Accuracy (VA)
VA = (verified correct outputs / total outputs) × 100

### Contradiction Rate (CR)
CR = (contradictions / total outputs) × 100

### Source Trace Score (STS)
Measures presence of verifiable sources

---

## 6. Benchmark Tasks

- provide claims requiring verification
- require sources or reasoning proof
- cross-check outputs against known data

---

## 7. Failure Modes

- unverifiable claims
- hidden contradictions
- fabricated sources
- missing evidence

---

## 8. Tripwires

Trigger if:
- VA < 80%
- CR > 10%
- STS low
