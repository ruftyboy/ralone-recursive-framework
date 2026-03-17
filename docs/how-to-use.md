# How to Use the Ralone Recursive Framework (RRF)

## Overview

RRF is a reasoning evaluation framework designed to:

- improve reasoning accuracy
- reduce hallucinations
- enforce logical consistency
- provide measurable evaluation

---

## Step-by-Step Usage

### 1. Provide Input

Give a reasoning task:

Example:
> Solve: If all A are B, and all B are C, what follows?

---

### 2. Generate Output

Use any model (LLM or human reasoning).

---

### 3. Apply Core Systems

Evaluate using:

- RTS → truth separation (fact vs inference)
- RLGE → logical validity
- RVE → verification of claims

---

### 4. Score with Metrics

Use `metrics/` definitions:

- accuracy score
- logical consistency score
- hallucination rate
- verifiability score

---

### 5. Compare with Benchmarks

Run against:

- `benchmarks/reasoning-tests.md`

Compare:
- baseline vs evaluated output

---

## Output Example

- Accuracy: 92%
- Logical consistency: High
- Hallucination risk: Low
- Verifiability: Confirmed

---

## Goal

RRF does NOT replace intelligence.

It ensures intelligence remains:

- correct
- stable
- verifiable
