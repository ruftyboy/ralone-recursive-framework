# Evaluation — Batch 3

## Overview

This batch tests advanced reasoning failures including:
- hidden contradictions
- conditional traps
- ambiguity handling
- logical generalization
- multi-step inference

---

## Results

| Test | Type | RTS | RLGE | RVE | Notes |
|------|------|-----|------|-----|------|
| 1 | Contradiction | 60 | 55 | 50 | partial logic failure |
| 2 | Conditional | 50 | 45 | 40 | assumes causation |
| 3 | Ambiguity | 40 | 35 | 30 | fails to detect ambiguity |
| 4 | Generalization | 55 | 50 | 45 | context leakage |
| 5 | Multi-step | 85 | 80 | 75 | mostly correct |

---

## Analysis

### Common Failures

- assumes unstated conditions  
- ignores ambiguity  
- overgeneralizes  
- treats implication as causation  

---

## Key Insight

Even when models perform well on structured logic:

they fail when:
- conditions are incomplete  
- multiple interpretations exist  
- reasoning requires restraint  

---

## Conclusion

Batch 3 reveals:

RRF is effective at detecting:
- reasoning shortcuts  
- hidden assumptions  
- fragile logic chains  

---
