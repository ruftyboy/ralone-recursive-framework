# Ralone Recursive Framework (RRF)
![Status](https://img.shields.io/badge/status-active-blue)
![Framework](https://img.shields.io/badge/type-reasoning--evaluation-green)
![License](https://img.shields.io/badge/license-MIT-lightgrey)
![Stage](https://img.shields.io/badge/stage-early--benchmark-orange)
A structured framework for evaluating reasoning quality in AI systems and human cognition.
RRF evaluates not just correctness — but how reasoning is formed, validated, and verified.
---
## Quick Start

Evaluate any reasoning output in 5 steps:

1. Choose a prompt (see `/benchmarks/`)
2. Get a model output
3. Apply:

   * RTS (truth)
   * RLGE (logic)
   * RVE (verification)
4. Score each (0–100)
5. Compute final RRF score

---
## Use Cases

RRF can be used for:

* evaluating AI model reasoning quality
* detecting hallucinations and logical errors
* comparing models beyond surface-level accuracy
* building reasoning benchmarks
* analyzing decision-making systems

---

### Example

Prompt:

> All A are B. Some B are C. Does it follow that some A are C?

Weak Answer:

> Yes, some A must be C.

RRF Evaluation:

* RTS: 40
* RLGE: 30
* RVE: 35

Final Score: 35 → **Fail**

---

## Why This Exists

Modern AI systems often produce outputs that appear correct but contain:

* hidden logical errors
* unsupported claims
* hallucinated facts

RRF provides a structured way to detect and measure these failures.

---

## Core Idea

RRF does not generate intelligence.
It evaluates whether reasoning is:

* correct
* logically consistent
* verifiable

---
## What Makes RRF Different

Most AI evaluations measure:

* fluency
* correctness of final answer

RRF focuses on:

* reasoning quality
* logical validity
* verifiability of claims

---

RRF detects:

* hidden logical errors
* overconfidence
* unsupported conclusions

---

It evaluates not just *what* is said — but *how it is reasoned*.
---
## Core Components

### RTS — Ralone Truth Scale

Separates:

* fact
* inference
* uncertainty

---

### RLGE — Ralone Logic Grounding Engine

Ensures:

* valid reasoning chains
* no contradictions
* correct conclusions

---

### RVE — Ralone Verification Engine

Validates:

* claims against evidence
* real-world consistency
* traceability of reasoning

---

## How It Works

1. Input a prompt
2. Generate output (AI or human)
3. Apply RTS, RLGE, RVE
4. Score each dimension
5. Compute final RRF score

---
## Evaluation Flow

RRF evaluates reasoning through three layers:

* RTS → truth accuracy
* RLGE → logical validity
* RVE → verification

See full flow: `docs/rrf-flow.md`
---
## Example Tests

* **Real Test 1** → pure logical reasoning
* **Real Test 2** → context-sensitive reasoning

See: `/docs/`

---

## Benchmark Results

RRF clearly separates strong vs weak reasoning:

| Test    | Strong Output | Weak Output |
| ------- | ------------- | ----------- |
| Logic   | 100           | 68.3        |
| Context | 100           | 21.6        |

See: `docs/benchmark-results.md`

---

## Model Comparison

RRF can compare reasoning quality across systems:

* detects overconfidence
* identifies logical failure points
* highlights verifiability issues

See: `docs/model-comparison.md`

---
## Project Structure

```
benchmarks/         # test sets (including hard tests)
docs/               # evaluations, comparisons, protocol
core/               # framework definitions
metrics/            # scoring system
```

## Philosophy

RRF does not restrict intelligence.
It ensures intelligence develops with:

* integrity
* stability
* verifiability

---

## Status

Early-stage framework with working evaluation examples and benchmark structure.

---
## Limitations

* small number of test cases (early-stage benchmark)
* partial reliance on manually constructed evaluations
* limited real-model comparisons

Future work includes expanding test coverage and automating evaluation.
---
RRF is designed to move evaluation from output correctness to reasoning integrity.
---
## License

MIT License
