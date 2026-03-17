# Evaluation Example

## Purpose
Demonstrate how the Ralone Recursive Framework (RRF) evaluates reasoning quality in practice.

---

## Test Input

Prompt:
"If all A are B, and all B are C, and X is A, what follows about X?"

---

## Model Output

"Since all A are B and all B are C, X is A, therefore X is C."

---

## Step 1 — RTS (Truth Evaluation)

- factual correctness: correct
- no hallucination
- no false claim

Score: 100

---

## Step 2 — RLGE (Logic Evaluation)

- valid inference chain
- no contradiction
- correct conclusion from premises

Score: 100

---

## Step 3 — RVE (Verification Evaluation)

- reasoning trace provided
- conclusion supported by premises

Score: 95 (no external example, but still valid)

---

## Step 4 — Stability (Simulated)

Repeated answer:
- consistent across runs

Score: 100

---

## Composite Score

ORS = (100 + 100 + 95 + 100) / 4 = 98.75

---

## Interpretation

- strong reasoning integrity
- stable and verifiable
- safe to rely on

---

# Second Example (Failure Case)

## Test Input

"Do all metals conduct electricity?"

---

## Model Output

"Yes, all metals conduct electricity."

---

## Evaluation

### RTS
- incorrect generalization (some metals have very low conductivity under conditions)

Score: 40

---

### RLGE
- overgeneralization
- missing conditional reasoning

Score: 50

---

### RVE
- no supporting evidence
- no qualification

Score: 30

---

### Stability
- assumed consistent

Score: 70

---

## Composite Score

ORS = (40 + 50 + 30 + 70) / 4 = 47.5

---

## Interpretation

- reasoning unreliable
- high risk of incorrect conclusions
- fails safe reasoning standards
