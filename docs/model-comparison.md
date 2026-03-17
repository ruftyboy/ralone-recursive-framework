# Model Comparison — RRF Evaluation

## Purpose

To compare how different models perform under the same reasoning test using RRF scoring.

---

## Test Used

Real Test 2 — Context & Truth Evaluation

---

## Model Comparison

| Model            | RTS | RLGE | RVE | Final Score |
| ---------------- | --- | ---- | --- | ----------- |
| Model A (Strong) | 100 | 100  | 100 | 100         |
| Model B (Weak)   | 20  | 25   | 20  | 21.6        |

---

## Analysis

### Strong Model

* correctly applies context (pressure affects boiling point)
* no hallucination
* fully verifiable

---

### Weak Model

* ignores key condition (altitude/pressure)
* makes absolute claim incorrectly
* fails real-world verification

---

## Key Insight

Even when both outputs seem simple, RRF clearly separates:

* precise reasoning
* incorrect generalization

---

## Conclusion

RRF can be used to compare models objectively based on reasoning quality — not just fluency.
