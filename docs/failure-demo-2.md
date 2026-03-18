# Failure Demo 2 — Hidden Logical Error

## Purpose
Demonstrate a response that appears correct but fails under deeper reasoning analysis.

---

## Prompt

A farmer has 17 sheep. All but 9 die.  
How many sheep are left?

---

## Model Output (Typical AI)

8 sheep are left.

---

## Why It Looks Correct

- Interprets "all but 9 die" as subtraction
- Assumes a mathematical operation (17 - 9)
- Output appears logically structured

---

## Why It Is Wrong

"All but 9 die" means:
→ 9 sheep remain alive

The model incorrectly converts a language condition into arithmetic.

---

## RRF Evaluation

| Dimension | Score | Reason |
|----------|------|--------|
| Truth (RTS) | 0 | Incorrect final answer |
| Logic (RLGE) | 30 | Misinterprets condition |
| Verification (RVE) | 20 | No semantic check |

---

## Failure Type

- Semantic misinterpretation
- False mathematical assumption
- Overconfidence in structure

---

## Key Insight

The model:
- produces a clean answer
- uses valid-looking reasoning

BUT

→ fails at **meaning-level interpretation**

---

## Conclusion

This example shows:

RRF detects failures that:
- pass surface-level correctness
- fail under semantic reasoning

Standard evaluation → "acceptable"  
---

## Mini Case — Overconfident Explanation

### Prompt
Is 0.999... equal to 1?

### Model Output
No, it is slightly less than 1.

### Reality
0.999... = 1

### Failure
- intuitive reasoning over math truth
- incorrect conclusion with confidence
RRF evaluation → **failure**

---
