# RRF Test Generator

## Purpose
Generate new reasoning tests systematically for the Ralone Recursive Framework (RRF).

---

## Core Formula

A strong RRF test usually combines:

- premise
- twist
- pressure point
- question

---

## Test Types

### 1. Logic Boundary Test
Tests whether a model overextends a conclusion.

**Template**
- All A are B.
- Some B are C.
- Does it follow that some A are C?

---

### 2. Context Sensitivity Test
Tests whether a model applies conditions correctly.

**Template**
- Statement is true under condition X.
- Condition Y changes the situation.
- Does the statement still hold?

---

### 3. Uncertainty Test
Tests whether a model separates evidence from certainty.

**Template**
- A result happens in many cases.
- A single case is observed.
- Can we conclude causation?

---

### 4. Contradiction Test
Tests whether a model detects internal inconsistency.

**Template**
- Two statements appear plausible.
- They cannot both be true under the same condition.
- Can the model identify the contradiction?

---

### 5. Exception Test
Tests whether a model catches real-world exceptions.

**Template**
- General rule is stated.
- Known exception exists.
- Does the model overgeneralize?

---

## Prompt Construction Rules

### Rule 1
Use simple language with hidden difficulty.

### Rule 2
Only one key reasoning trap per prompt.

### Rule 3
Make the wrong answer tempting.

### Rule 4
The correct answer should be explainable clearly.

---

## Example Generated Tests

### Example A — Logic Boundary
All artists in the room are trained observers.  
Some trained observers miss important details.

Does it follow that some artists in the room miss important details?

---

### Example B — Context Sensitivity
A metal expands when heated under normal conditions.  
In a constrained structure, expansion may be restricted.

Does metal always freely expand whenever it is heated?

---

### Example C — Uncertainty
A treatment helps 80% of patients in a study.  
One patient improved after taking it.

Did the treatment definitely cause the improvement?

---

## Output Template

For each generated test, include:

- prompt
- what it tests
- likely weak answer
- correct reasoning
- scoring notes

---

## Goal
The purpose of the generator is to create many tests while preserving:

- clarity
- difficulty
- evaluability
- repeatability
