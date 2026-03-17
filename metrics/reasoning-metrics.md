# Reasoning Metrics

## Purpose
Defines how reasoning quality is measured across truth, logic, verification, and stability.

---

## 1. Contradiction

### Definition
A contradiction occurs when a system produces statements that cannot both be true under the same conditions.

### Examples
- "All metals are magnetic" and later "Some metals are not magnetic"
- conflicting conclusions from identical premises

---

## 2. Hallucination

### Definition
A hallucination is a confident statement that is false or unsupported by known facts.

### Types
- factual hallucination (incorrect information)
- fabricated explanation
- invented sources

---

## 3. Weak Verification

### Definition
A claim made without sufficient supporting reasoning or evidence.

### Indicators
- assertions without explanation
- lack of examples
- unverifiable claims

---

## 4. Logical Failure

### Definition
A breakdown in reasoning where the conclusion does not follow from the premises.

### Examples
- invalid inference
- missing reasoning steps
- circular reasoning

---

## 5. Stability Failure

### Definition
Inconsistency in outputs when the same prompt is repeated.

### Indicators
- different answers for identical inputs
- shifting reasoning across attempts

---

## 6. Scoring Rules

### High Quality (90–100)
- no contradictions
- correct reasoning
- verified claims
- stable outputs

### Medium Quality (70–89)
- mostly correct
- minor inconsistencies
- acceptable reasoning

### Low Quality (50–69)
- noticeable errors
- weak verification
- unstable reasoning

### Failure (<50)
- contradictions present
- hallucinations frequent
- logic breaks down
