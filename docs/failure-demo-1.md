# Failure Demonstration 1 — Hidden Contradiction

## Test Used

Hard Test 1 — Hidden Contradiction

---

## Prompt

All engineers in a company are highly trained.
Some highly trained people make critical mistakes.

Does it follow that some engineers make critical mistakes?

---

## Model Output (Weak)

Yes, because engineers are highly trained and some highly trained people make mistakes, so some engineers must make mistakes.

---

## Evaluation

### RTS — Truth Scale

* not necessarily true
* assumes overlap without proof
* introduces unsupported conclusion

Score: 40

---

### RLGE — Logic Grounding Engine

* logical error: assumes subset overlap
* invalid inference (does not necessarily follow)
* reasoning chain is flawed

Score: 30

---

### RVE — Verification Engine

* no evidence that engineers are part of the "some" group
* claim is not verifiable from premises

Score: 35

---

## Composite Score

RRF Score = (40 + 30 + 35) / 3 = 35

---

## Correct Reasoning

The conclusion does NOT necessarily follow.

Reason:

* engineers are a subset of highly trained people
* but we are not told that the engineers are part of the group that makes mistakes

---

## Result

This output fails due to invalid logical inference and assumption of overlap without evidence.
