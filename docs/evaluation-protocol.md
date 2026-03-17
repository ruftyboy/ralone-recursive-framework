# RRF Evaluation Protocol

## Purpose

Define a consistent process for evaluating reasoning outputs using the Ralone Recursive Framework (RRF).

---

## Evaluation Steps

### Step 1 — Read the Prompt Carefully

* identify key conditions
* identify hidden constraints
* identify potential traps

---

### Step 2 — Analyze the Output

* what is the claim?
* what assumptions are made?
* what is concluded?

---

### Step 3 — Apply RTS (Truth Scale)

Evaluate:

* factual correctness
* hallucination presence
* misuse of certainty

Scoring Guide:

* 90–100 → fully correct
* 70–89 → mostly correct with minor issues
* 40–69 → partially correct but flawed
* 0–39 → incorrect or misleading

---

### Step 4 — Apply RLGE (Logic Grounding Engine)

Evaluate:

* validity of reasoning chain
* presence of logical errors
* correct use of premises

Scoring Guide:

* 90–100 → logically sound
* 70–89 → mostly valid with small gaps
* 40–69 → weak reasoning
* 0–39 → invalid logic

---

### Step 5 — Apply RVE (Verification Engine)

Evaluate:

* claim support from premises
* consistency with known facts
* traceability of reasoning

Scoring Guide:

* 90–100 → fully verifiable
* 70–89 → mostly supported
* 40–69 → weak support
* 0–39 → unsupported or contradictory

---

### Step 6 — Compute Final Score

RRF Score = (RTS + RLGE + RVE) / 3

---

## Evaluation Rules

### Rule 1

Do not assume information not given in the prompt.

### Rule 2

Do not reward confident but incorrect answers.

### Rule 3

Penalize overgeneralization.

### Rule 4

Reward precise reasoning.

---

## Failure Indicators

Common failure patterns:

* assumption of overlap without evidence
* ignoring conditions
* confusing correlation with causation
* overconfident incorrect conclusions

---

## Goal

Ensure that different evaluators produce:

* consistent scores
* comparable results
* reliable reasoning assessments
