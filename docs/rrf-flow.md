# RRF Evaluation Flow

## Overview

The Ralone Recursive Framework evaluates reasoning through three layers:

Prompt → Output → Evaluation → Score

---

## Flow

```text
INPUT (Prompt)
        ↓
MODEL OUTPUT
        ↓
-------------------------
|   RRF EVALUATION      |
-------------------------
   ↓        ↓        ↓
  RTS      RLGE     RVE
 (Truth)  (Logic) (Verify)
   ↓        ↓        ↓
   --------AGGREGATE--------
              ↓
        FINAL SCORE
              ↓
        PASS / FAIL
```

---

## Description

### RTS — Truth Layer

Checks:

* factual correctness
* hallucinations
* misuse of certainty

---

### RLGE — Logic Layer

Checks:

* reasoning validity
* inference structure
* contradictions

---

### RVE — Verification Layer

Checks:

* evidence support
* real-world consistency
* traceability

---

## Output

Final result:

* numerical score
* reasoning quality classification
