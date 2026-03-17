# Ralone Recursive Framework (RRF)

A structured framework for evaluating reasoning quality in AI systems and human cognition.

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

## License

MIT License
