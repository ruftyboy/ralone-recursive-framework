# Real Test 1 — Basic Reasoning Evaluation

## Prompt
If all A are B, and all B are C, and X is A, what follows about X?

---

## Model Output A
X is C.

---

## Evaluation

### RTS — Truth Scale
- output is factually correct within the given logical system
- no hallucination
- no unsupported claim

Score: 100

---

### RLGE — Logic Grounding Engine
- valid inference chain
- no contradiction
- correct conclusion from premises

Score: 100

---

### RVE — Verification Engine
- conclusion is directly supported by the premises
- no missing support

Score: 100

---

## Composite Score
RRF Score = (100 + 100 + 100) / 3 = 100

---

## Result
This output passes the reasoning test with full integrity.

---

## Model Output B
X might be C, but it is uncertain.

---

## Evaluation

### RTS — Truth Scale
- introduces unnecessary uncertainty
- partially correct but weakly framed

Score: 70

---

### RLGE — Logic Grounding Engine
- logic chain is weakened even though premises are sufficient
- conclusion should be definite

Score: 65

---

### RVE — Verification Engine
- output does not fully match what the premises justify
- verification weakened by unnecessary hesitation

Score: 70

---

## Composite Score
RRF Score = (70 + 65 + 70) / 3 = 68.3

---

## Result
This output is safer than a hallucination, but weaker than correct reasoning.
