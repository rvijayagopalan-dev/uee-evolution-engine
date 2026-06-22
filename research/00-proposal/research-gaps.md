# Research Gaps

*The literature gaps that motivate each research question. Pairs one-to-one with
[`research-questions.md`](./research-questions.md): RQ1 is the overarching gap;
RQ2–RQ5 are the four independent ways it could fail to exist.*

---

## The overarching gap — the empty cell

Existing maturity models — CMM/CMMI, DAMA-DMM, data-maturity ladders, digital-twin
frameworks — each occupy a *weak* region of the maturity-model landscape. Placed on a
2×2 of **scope** (single-domain vs. cross-domain) × **use** (descriptive vs.
predictive), with a third axis for **validation** (conceptual vs. empirical), every
established model lands in:

- **single-domain**, and/or
- **conceptually derived** (not empirically validated), and/or
- **descriptive** (not predictive).

The cell *"cross-domain + empirically validated + predictive"* is **empty**. The
thesis claims that cell can be filled by a single construct — the 11-level maturity
meta-model of adaptive capability. Confirming Study 1 (systematic review) tests the
gap hypothesis directly: if a model already occupies the cell, the project pivots — a
decision deliberately front-loaded.

---

## Gap 1 — The fragmentation gap (motivates RQ1)

Adaptive capability is theorized in pieces that never join:

- **DIKW** gives an *epistemic* ladder (Data → Information → Knowledge → Wisdom) but
  is silent on action, learning, and adaptation — and is itself heavily critiqued.
- **Cybernetics → organizational learning → dynamic capabilities** gives an
  *adaptive control loop* but no ordered, measurable scale.

No literature **fuses the epistemic ladder with the adaptive-control loop into one
ordered, domain-invariant construct**. RQ1 asks whether that fused construct is real,
transferable, and predictive — rather than a per-industry narrative. The fusion is the
thesis's core novelty; neither parent literature makes the claim alone.

## Gap 2 — The measurement gap (motivates RQ2)

Existing maturity models are conceptually derived and rarely ship with a
reliability-tested instrument; level assignment is typically subjective and
retrofittable. **Without objective per-level indicators and demonstrated
inter-rater reliability and construct validity, adaptive capability is not a
measurable construct** — and RQ1 is unanswerable, because an unmeasurable scale can
be fitted to anything. RQ2 closes this with a rubric-based instrument, κ/α ≥ 0.7, and
factor-analytic evidence that the levels do not collapse.

## Gap 3 — The generalizability gap (motivates RQ3)

The construct's source material (the UEEOS rice-cultivation case study) demonstrated
the ladder on **one** domain and **never allowed it to fail**. More broadly, "every
industry has its own maturity model" is the status quo precisely because none has
been shown to transfer unchanged. **No model has been tested for structural
invariance across unrelated domains with a pre-registered way to be refuted.** RQ3
closes this by instantiating the structure in ≥3 unrelated domains with no structural
edits, and a pre-registered null (H0) that any required edit refutes invariance.

## Gap 4 — The predictive gap (motivates RQ4)

Maturity models are overwhelmingly **descriptive**: they label a current state but
do not forecast outcomes, and are seldom benchmarked against a baseline. **There is
little evidence that maturity level predicts adaptation performance at all, let alone
better than a domain-specific baseline.** A level that predicts nothing is a
vocabulary, not a science. RQ4 closes this by testing predictive validity against a
baseline with pre-registered, significance-tested hypotheses.

## Gap 5 — The distinctness gap (motivates RQ5)

The model's nearest rivals are **CMMI** (the incumbent maturity standard) and
**dynamic capabilities** (Teece, the leading theory of organizational adaptation).
A reviewer's sharpest challenge: *"isn't this just CMMI relabeled, or dynamic
capabilities with extra steps?"* **No work has shown that a unified DIKW-plus-adaptive
ladder explains outcome variance beyond what these frameworks already capture.** RQ5
closes this by testing the full ordered ladder's *incremental* explanatory power over
both rivals. The framework treats dynamic capabilities as the *theory of levels 9–10*
rather than a competitor, so RQ5's burden is to show the **whole** ladder adds value.

---

## Gap → question → test map

| Gap | Closes | Failure mode if gap is real & unaddressed | Test |
|-----|--------|-------------------------------------------|------|
| 1 — Fragmentation | RQ1 | Construct is just a per-industry narrative | Conjunction of RQ2–RQ5 |
| 2 — Measurement | RQ2 | Scale unmeasurable / collapses to few factors | κ/α, factor analysis (P1, P4) |
| 3 — Generalizability | RQ3 | Domain needs structural edits (H0) | Cross-domain instantiation (P2/H1) |
| 4 — Predictive | RQ4 | Level predicts nothing beyond baseline | Regression/AUC vs. baseline (P3/H2) |
| 5 — Distinctness | RQ5 | No variance beyond CMMI / dynamic capabilities | Incremental validity (P5) |

A result that **disconfirms** any gap-closing claim is a publishable finding, not a
failure — the program is designed to be proven wrong (pre-registered H0).

---

_Status: research gaps v1.0 — pairs with [`research-questions.md`](./research-questions.md).
Gap 1's emptiness claim is tested empirically in Study 1 (systematic review); see
[`../01-literature-review/lit-review-protocol.md`](../01-literature-review/lit-review-protocol.md)._
