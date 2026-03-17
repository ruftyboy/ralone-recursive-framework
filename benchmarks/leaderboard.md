# RRF Leaderboard — Reasoning Evaluation

## Purpose

Rank models based on reasoning quality using the Ralone Recursive Framework (RRF).

---

## Methodology

Each model is evaluated across multiple tests using:

* RTS (Truth Scale)
* RLGE (Logic Grounding Engine)
* RVE (Verification Engine)

Final score = average across all tests.

---

## Current Leaderboard

| Rank | Model                  | Logic Test | Context Test | Failure Test | Avg Score |
| ---- | ---------------------- | ---------- | ------------ | ------------ | --------- |
| 1    | ChatGPT (baseline)     | 100        | 100          | 35           | 78.3      |
| 2    | Weak Model (simulated) | 68.3       | 21.6         | 35           | 41.6      |

---

## Interpretation

### ChatGPT (baseline)

* strong logical reasoning
* handles context correctly
* still fails under hidden contradiction

---

### Weak Model

* inconsistent reasoning
* fails context-sensitive tasks
* prone to incorrect generalization

---

## Key Insight

Even strong models can fail under:

* hidden logical traps
* ambiguous reasoning conditions
* incomplete information

---

## Status

Early benchmark with limited tests.
Planned expansion:

* more test categories
* more models
* automated evaluation pipeline
