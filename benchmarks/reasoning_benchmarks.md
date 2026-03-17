# Reasoning Benchmark Tests

## Purpose
This benchmark evaluates whether a system can reason with truth integrity, logical consistency, verification discipline, and stability across repeated attempts.

It maps primarily to:
- RTS
- RVE
- RLGE

---

## Test 1 — Multi-Step Logic

### Goal
Measure whether the system can complete a multi-step reasoning chain without contradiction or invalid inference.

### Example Prompt
If all A are B, and all B are C, and X is A, what follows about X?

### Expected Answer
X is C.

### Measured Dimensions
- logical consistency
- inference validity
- contradiction rate

### Scoring
- 100 = fully correct, no contradiction, valid reasoning
- 70 = correct answer, weak or incomplete reasoning
- 40 = partial reasoning, unstable logic
- 0 = invalid conclusion

---

## Test 2 — Truth vs Inference

### Goal
Measure whether the system separates fact from inference from uncertainty.

### Example Prompt
Water boils at 100°C at standard atmospheric pressure. Does water always boil at exactly 100°C everywhere on Earth?

### Expected Answer
No. That is true only under standard atmospheric pressure; boiling point changes with altitude and pressure.

### Measured Dimensions
- truth accuracy
- inference labeling
- uncertainty awareness
- hallucination resistance

### Scoring
- 100 = correct answer with correct qualification
- 75 = mostly correct answer, limited qualification
- 40 = answer partly correct but overconfident
- 0 = false certainty or hallucinated claim

---

## Test 3 — Verification Required

### Goal
Measure whether the system can justify a claim rather than only assert it.

### Example Prompt
Why is the statement “all metals are magnetic” false?

### Expected Answer
Because not all metals are magnetic; for example, copper and aluminum are not ferromagnetic.

### Measured Dimensions
- verification quality
- factual support
- explanation traceability

### Scoring
- 100 = correct answer with valid supporting example
- 70 = correct answer with weak support
- 30 = unsupported assertion
- 0 = false answer

---

## Test 4 — Stability Test

### Goal
Measure whether repeated answers remain stable across retries.

### Example Prompt
Ask the same logic question three times in separate runs.

### Measured Dimensions
- answer consistency
- reasoning stability
- contradiction drift

### Scoring
- 100 = stable across all runs
- 70 = same answer, minor wording drift
- 40 = partial inconsistency
- 0 = major contradiction between runs

---

## Composite Scoring

Overall Reasoning Score (ORS):

ORS = average of:
- Logic Score
- Truth Score
- Verification Score
- Stability Score

Range: 0–100

---

## Interpretation

- 90–100 = strong reasoning integrity
- 75–89 = usable but imperfect
- 50–74 = unstable reasoning quality
- below 50 = high reasoning failure risk
