# System Flow

## Purpose
Defines how all components of the Ralone Recursive Framework (RRF) interact in a complete evaluation cycle.

---

## Step 1 — Input

A prompt or task is given to the system.

---

## Step 2 — Model Output

The system produces a response.

---

## Step 3 — RTS (Truth Evaluation)

- checks factual correctness
- detects hallucinations
- evaluates confidence vs truth

---

## Step 4 — RLGE (Logic Evaluation)

- validates reasoning structure
- detects contradictions
- checks inference validity

---

## Step 5 — RVE (Verification)

- checks supporting evidence
- validates claims
- evaluates traceability

---

## Step 6 — Metrics Application

Apply defined metrics:
- contradiction
- hallucination
- verification strength
- stability

---

## Step 7 — Benchmark Mapping

Compare output to benchmark tasks:
- reasoning tests
- verification tests
- stability tests

---

## Step 8 — Scoring

Compute scores:
- RTS score
- RLGE score
- RVE score
- Stability score

---

## Step 9 — Composite Score

ORS = average of all scores

---

## Step 10 — Interpretation

Classify result:

- 90–100 → strong reasoning integrity  
- 75–89 → usable but imperfect  
- 50–74 → unstable  
- <50 → failure  

---

## Output

Final evaluation result:
- score
- strengths
- weaknesses
- risk level
