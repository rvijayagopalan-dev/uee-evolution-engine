# Doctoral Research Proposal

**Working title:** *A Domain-Invariant Maturity Model of Adaptive Capability:
Cross-Domain Transfer and Predictive Validity*

**Candidate:** _[name]_ · **Proposed supervisor:** _[name]_ · **Date:** _[date]_

> Synthesis document for prospective supervisors. Draws together the drafts in this
> repository: [theory](../02-theoretical-framework/theoretical-framework.md),
> [review protocol](../01-literature-review/lit-review-protocol.md),
> [rubric](../../docs/evaluation/maturity-rubric.md),
> [survey](../03-methodology/maturity-survey-instrument.md),
> [datasets](../05-data/candidate-datasets.md), and [roadmap](../phd-roadmap.md).

---

## 1. Abstract

Organizations and managed socio-technical systems are routinely described as
"evolving" from raw data toward intelligent, self-adapting behavior, yet the stages
of that progression are defined ad hoc and per industry. Maturity models such as
CMMI and data-maturity frameworks each capture a fragment, but none is shown to be
**domain-invariant, empirically validated, and predictive of outcomes**. This
research develops and tests an 11-level maturity meta-model of *adaptive capability*
(Reality → Observation → Data → Knowledge → Intelligence → Wisdom → Purpose →
Action → Learning → Adaptation → Evolution), grounded in the DIKW hierarchy and the
cybernetic/organizational-learning control loop. Across three unrelated domains
(agriculture, supply chain, clinical pathways) it asks whether one fixed structure
both *transfers* and *predicts adaptation outcomes* — and it is designed to be
proven wrong.

## 2. Background & motivation

The idea originates from a domain-grounded validation exercise (the UEEOS rice-
cultivation case study, `docs/evaluation/`), whose early versions describe a
coherent maturity ladder for agriculture. This proposal extracts that grounded core
and subjects it to the test the original never applied: **does it generalize, and
can it fail?** The metaphysical extensions of the source material are explicitly
out of scope.

## 3. Problem & gap

Existing maturity models are predominantly **single-domain, conceptually derived,
and descriptive**. A systematic review (Study 1) will test the gap hypothesis: that
the cell *"cross-domain + empirically validated + predictive"* is **empty**. If a
model already occupies it, the project pivots — a decision deliberately front-loaded.

## 4. Research questions

> **RQ1 (primary).** Can adaptive capability be represented as a domain-invariant
> hierarchical construct that predicts adaptive outcomes across multiple domains —
> **without per-domain modification**?

Decomposed into four supporting questions, each a falsifiable wall of the primary
claim (canonical statement: [`research-questions.md`](./research-questions.md);
motivating gaps: [`research-gaps.md`](./research-gaps.md)):

- **RQ2** Can adaptive capability be measured reliably and validly? *(P1, P4)*
- **RQ3 (H1)** Does the structure remain invariant across ≥3 unrelated domains? *(P2)*
- **RQ4 (H2)** Does adaptive capability predict adaptation outcomes better than a
  domain-specific baseline? *(P3)*
- **RQ5** Does it provide explanatory power beyond existing maturity (CMMI) and
  dynamic-capability frameworks? *(P5)*

RQ1 holds **iff** RQ2 ∧ RQ3 ∧ RQ4 ∧ RQ5 hold. The systematic review (Study 1)
establishes the gap these questions target.

## 5. Theoretical framework (summary)

The ladder fuses two established literatures: **DIKW** (levels 2–5) and the
**cybernetics → organizational-learning → dynamic-capabilities** adaptive loop
(levels 0–1, 6–10). Levels form a **logical dependency chain** (each presupposes the
prior), and L8→L9→L10 maps onto **single-loop → double-loop → deutero-learning**.
Four formal propositions follow: orderability, domain invariance (H1), predictive
validity (H2), construct distinctness. Full detail:
[`theoretical-framework.md`](../02-theoretical-framework/theoretical-framework.md).

## 6. Methodology

Mixed methods, pre-registered, PRISMA-based review:

- **Instrument:** the 11-level [rubric (v1.1)](../../docs/evaluation/maturity-rubric.md)
  for rater scoring + a [self-report survey](../03-methodology/maturity-survey-instrument.md)
  for the maturity (independent) variable.
- **Outcomes:** adaptation measures from secondary data
  ([candidate datasets](../05-data/candidate-datasets.md)); unit of analysis is the
  **system/organization over time**.
- **Validity:** inter-rater reliability (κ/α ≥ 0.7), construct validity (factor
  analysis), pre-registered hypotheses, reproducible analysis.

## 7. Study plan

| Study | Question | Method | Output |
|------|----------|--------|--------|
| S1 | Gap & framework | Systematic review + synthesis | Review paper |
| S2 | Measurable & reliable? (RQ2) | Rubric + survey; κ; construct validity | Methods paper *(pilot done)* |
| S3 | Invariant? (RQ3/H1) | Score ≥3 domains, no structural change | Empirical paper |
| S4 | Predict & distinct? (RQ4/H2, RQ5) | Maturity vs. outcome vs. baseline; incremental validity | Empirical paper |

## 8. Expected contribution

1. A **domain-invariant, validated, predictive** maturity meta-model (if H1/H2 hold).
2. A reusable, reliability-tested **measurement instrument**.
3. Empirical evidence — **including a documented null** if the model fails to
   generalize, which is itself a contribution.

## 9. Feasibility & preliminary work

A working instrument (rubric v1.1), a two-domain pilot
([worked example](../../docs/evaluation/worked-example.md)), a theory draft, a review
protocol, and a dataset scan already exist — de-risking years 1–2.

## 10. Ethics

Organizational surveys and the clinical domain require **ethics/IRB approval, informed
consent, and data-use agreements**; patient-level sources need credentialing. Ethics
work starts early (Phase 3) to avoid bottlenecks.

## 11. Indicative timeline (full-time ~4 yr)

| Year | Focus |
|------|-------|
| 1 | Admission, review (S1), theory, ethics |
| 2 | Methodology, instrument validation (S2), data partnerships |
| 3 | Cross-domain transfer (S3), predictive validity (S4) |
| 4 | Synthesis, publications, thesis, viva |

## 12. Risks

Novelty vs. CMMI (mitigated by §3 review), unfalsifiability (pre-registered H0),
data access (partnerships secured early), ethics delays (started early), scope creep
into metaphysics (v20 boundary enforced). Detail in
[`../phd-roadmap.md`](../phd-roadmap.md).

## References

_[To be completed in Phase 1 — DIKW, Ashby, Simon, Argyris & Schön, Nelson & Winter,
Teece, Holland, Maturana & Varela, CMMI/CMM, DAMA-DMM, PRISMA 2020, and the review
corpus.]_

---

_Status: proposal draft v0.1 — fill bracketed fields, add references, tailor to the
target program/supervisor before submission._
