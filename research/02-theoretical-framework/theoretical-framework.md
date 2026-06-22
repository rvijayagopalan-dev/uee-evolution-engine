# Theoretical Framework

*Justifies the 11-level maturity engine from established theory rather than
intuition, defines its constructs, states its scope conditions, and formalizes the
falsifiable propositions. This is what a reviewer presses on: "why these levels,
why this order, why eleven?"*

---

## 1. Stance

The engine is positioned as a **maturity meta-model**: a domain-invariant ordering
of *adaptive capability*. It is not a new ontology of reality — that framing (the
v21+ tiers) is explicitly excluded. The claim is narrow and testable: **systems that
adapt well exhibit a recurring, orderable set of capabilities**, and that ordering
is the same across domains.

## 2. Theoretical roots of each level

The ladder is a synthesis of four established bodies of theory. The honest position:
**levels 0–8 are well-grounded; levels 9–10 are a defensible extension** that the
empirical work must earn.

| Lvl | Construct | Primary theoretical root |
|----:|-----------|--------------------------|
| 0 | Reality | Systems theory — system boundary & identification (von Bertalanffy) |
| 1 | Observation | Cybernetics — sensing / requisite variety (Ashby, Wiener) |
| 2 | Data | Information theory; the **DIKW hierarchy** (data tier) |
| 3 | Knowledge | DIKW (knowledge tier); knowledge representation / ontologies |
| 4 | Intelligence | Decision theory; bounded rationality (Simon) |
| 5 | Wisdom | DIKW (wisdom tier); multi-criteria & value-based judgment |
| 6 | Purpose | Cybernetics of goals; teleological systems; strategic intent |
| 7 | Action | Control theory — actuation; routines & capabilities (Nelson & Winter) |
| 8 | Learning | Organizational learning (Argyris & Schön: single-/double-loop); absorptive capacity |
| 9 | Adaptation | Complex adaptive systems (Holland); **dynamic capabilities** (Teece) — reconfiguration |
| 10 | Evolution | Double-loop → deutero-learning; autopoiesis (Maturana & Varela); self-organization |

**Why this order:** it follows the **sense → model → decide → act → learn → adapt →
self-transform** control loop, nested. Each level *presupposes* the ones below it
(you cannot learn from outcomes you do not act on, act on decisions you cannot make,
decide without knowledge, etc.). This gives the ladder a **logical dependency
structure**, not just a narrative.

## 3. Two theoretical anchors do most of the work

1. **DIKW hierarchy** (Data → Information → Knowledge → Wisdom) grounds levels 2–5
   — the most established part, also the most critiqued (so engage the critiques).
2. **The viable / adaptive control loop** (cybernetics → organizational learning →
   dynamic capabilities) grounds levels 0–1 and 6–10 — the *adaptation* spine that
   is the thesis's actual contribution.

The novelty is **fusing the epistemic ladder (DIKW) with the adaptive-control loop
into one ordered scale and claiming it is domain-invariant** — a claim neither
literature makes on its own.

## 4. Construct definitions (abridged; full versions feed the rubric)

Each level is defined by *what capability is present*, operationalized in
[`maturity-rubric.md`](../../docs/evaluation/maturity-rubric.md). Critical
boundary definitions (carried from rubric v1.1):

- **Knowledge (L3):** an explicit *relational model* of the domain (graph = highest form).
- **Learning (L8):** outcomes change *decision rules* — Argyris & Schön **single-loop**.
- **Adaptation (L9):** behavior reconfigures within the **current structure**.
- **Evolution (L10):** the **structure itself** changes — **double-loop / deutero-learning**.

The L8→L9→L10 progression maps cleanly onto the **single-loop → double-loop →
deutero-learning** hierarchy, which is its strongest theoretical defense.

## 5. Scope conditions (where the model is claimed to hold)

State these explicitly — a theory without boundaries is unfalsifiable:
- Applies to **purposive, adaptive systems** (organizations, managed socio-technical
  systems) — not arbitrary physical processes.
- Assumes the system has **goals** and operates over **repeated cycles** (so learning
  and adaptation are observable).
- The unit of analysis is the **system/organization**, scored over a bounded period.
- Domain-invariance is claimed for *the level structure*, **not** for the level
  *content* (which is domain-specific by construction).

## 6. Formal propositions (testable)

- **P1 (Orderability / dependency).** Within a system, attainment at level *n*
  rarely exceeds attainment at level *n−1*; the levels form a near-cumulative
  (Guttman-like) scale. *Test:* scalogram / Mokken analysis on rubric scores.
- **P2 (Domain invariance — H1).** The same 11-level structure fits ≥3 unrelated
  domains with no added/removed levels. *Falsifier (H0):* any domain needs a
  structural edit.
- **P3 (Predictive validity — H2).** A system's maturity (Index or Attained Level)
  predicts adaptation outcomes better than a domain-specific baseline. *Test:*
  regression / AUC vs. baseline, pre-registered.
- **P4 (Construct distinctness).** The 11 levels are not collapsible to fewer latent
  factors than theorized. *Test:* factor analysis / dimensionality assessment.
- **P5 (Incremental validity — RQ5).** Maturity explains adaptation-outcome variance
  *beyond* what CMMI and dynamic-capability measures capture. *Test:* hierarchical
  regression — added R² / ΔAUC over the rival predictors, pre-registered.

Propositions map to the research questions in
[`../00-proposal/research-questions.md`](../00-proposal/research-questions.md):
P1/P4→RQ2, P2→RQ3, P3→RQ4, P5→RQ5; RQ1 is the conjunction.

## 7. Known theoretical risks (address head-on)

| Risk | Response |
|------|----------|
| **DIKW is widely critiqued** (esp. data→wisdom as naive) | Use DIKW only for L2–L5; lean on cybernetics/learning theory for the adaptive spine; cite the critiques |
| **"11 levels" looks arbitrary** | Defend via the dependency loop + single/double/deutero-learning, not via the number itself; let factor analysis (P4) check granularity |
| **Overlap with dynamic capabilities** | Frame dynamic capabilities as the *theory of L9–L10*, not a competitor; this strengthens grounding |
| **Reification** (treating a scale as a real "engine") | Keep it a measurement model; avoid the metaphysical framing entirely |

## 8. Outputs
- Theory chapter (this, expanded) → `./`
- Construct table feeding the rubric and survey instrument
- The four propositions → tested in `../04-studies/`

---

_Status: framework draft v0.1 — needs full citations and a deeper DIKW-critique
engagement. See [`../phd-roadmap.md`](../phd-roadmap.md) Phase 2._
