# Real Test 2 — Context & Truth Evaluation

## Prompt

Water boils at 100°C at standard atmospheric pressure.
At high altitudes, atmospheric pressure is lower.

Does water always boil at exactly 100°C everywhere on Earth?

---

## Model Output A

No. Water boils at 100°C only at standard atmospheric pressure.
At higher altitudes, where pressure is lower, water boils at lower temperatures.

---

## Evaluation

### RTS — Truth Scale

* factually correct
* no hallucination
* correctly applies condition (pressure affects boiling point)

Score: 100

---

### RLGE — Logic Grounding Engine

* correctly connects altitude → pressure → boiling point
* no contradiction
* strong reasoning chain

Score: 100

---

### RVE — Verification Engine

* fully supported by known physics
* claim is verifiable
* no unsupported assumptions

Score: 100

---

## Composite Score

RRF Score = (100 + 100 + 100) / 3 = 100

---

## Result

This output demonstrates correct contextual reasoning and scientific accuracy.

---

## Model Output B

Yes, water always boils at exactly 100°C everywhere on Earth.

---

## Evaluation

### RTS — Truth Scale

* factually incorrect
* ignores pressure variation
* overgeneralization

Score: 20

---

### RLGE — Logic Grounding Engine

* fails to apply given condition (altitude → pressure)
* weak reasoning
* incorrect conclusion

Score: 25

---

### RVE — Verification Engine

* not supported by real-world evidence
* contradicts known physics
* unverifiable claim

Score: 20

---

## Composite Score

RRF Score = (20 + 25 + 20) / 3 = 21.6

---

## Result

This output fails due to incorrect assumptions and lack of contextual reasoning.
