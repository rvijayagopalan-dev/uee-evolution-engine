# Maturity Survey Instrument (Self-Report)

*Primary-data instrument that operationalizes
[`maturity-rubric.md`](../../docs/evaluation/maturity-rubric.md) v1.1 as a
respondent-facing questionnaire. Fills the gap identified in
[`../05-data/candidate-datasets.md`](../05-data/candidate-datasets.md): public data
gives outcomes but not maturity scores (esp. Levels 5–10).*

> **Domain-invariant by design.** The same 11 question blocks apply to any domain;
> only the bracketed `[examples]` change. Keeping wording fixed across domains is
> what makes the H1 transfer test fair.

---

## Section A — Respondent & unit of analysis

| Field | Note |
|-------|------|
| A1. Organization / system name (or code) | The **unit of analysis** — must be a system, not a person |
| A2. Domain | Agriculture / Supply chain / Clinical / Other |
| A3. Respondent role & tenure | For source-credibility weighting |
| A4. Reporting period | Anchor all answers to one period (e.g., last 12 months) |
| A5. Respondent's basis of knowledge | Direct / partial / secondhand |

> Collect **≥2 respondents per unit** where possible, to estimate self-report reliability.

## Section B — Maturity blocks (Levels 0–10)

Each level uses the **same 0–3 anchors** as the rubric. Respondent selects the
statement that best matches the reporting period. (Optional free-text "evidence"
box per block to support later rater verification.)

> Scale: **0** Absent · **1** Ad hoc / manual / inconsistent · **2** Systematic /
> repeatable · **3** Optimized / automated / continuously improved.

### L0 — Reality
*Are the system's entities, actors, inputs and outputs explicitly identified?*
- 0: No documented inventory.
- 1: Informal/partial knowledge, not written down.
- 2: A maintained inventory of `[entities/actors/inputs/outputs]` exists.
- 3: Inventory is complete, owned, and kept current.

### L1 — Observation
*Are signals captured from the real system?*
- 0: No systematic data capture.
- 1: Occasional/manual readings of `[key variables]`.
- 2: Routine capture of most key variables at a set cadence.
- 3: Comprehensive, automated capture with monitored coverage.

### L2 — Data
*Is what you observe stored with structure and governance?*
- 0: Scattered/unstored.
- 1: Spreadsheets/local files, no standards.
- 2: Structured store with schema and basic governance.
- 3: Governed, quality-monitored, with metadata/lineage.

### L3 — Knowledge
*Are relationships and rules made explicit?* *(v1.1: 2 = relational model, 3 = formal graph)*
- 0: Relationships exist only in people's heads.
- 1: Some documented rules of thumb.
- 2: An explicit relational model linking `[entities]`.
- 3: A formal knowledge graph / ontology.

### L4 — Intelligence
*Does the system produce recommendations?*
- 0: None.
- 1: Occasional expert/manual recommendations.
- 2: Systematic recommendations for `[decisions]`, accuracy tracked.
- 3: Validated, continuously improved recommendation models.

### L5 — Wisdom
*Are trade-offs reasoned about explicitly?*
- 0: Trade-offs not considered.
- 1: Considered informally, case by case.
- 2: Documented multi-criteria trade-offs (e.g., `[X vs. Y]`).
- 3: Trade-offs modeled and optimized routinely.

### L6 — Purpose
*Are decisions tied to declared goals?* *(v1.1: 3 requires traceability)*
- 0: No declared goals guiding decisions.
- 1: Goals exist but aren't linked to decisions.
- 2: Decisions mostly aligned to declared goals.
- 3: Decisions are **traceable** to declared goals.

### L7 — Action
*Are decisions executed as managed workflows?* *(v1.1: 2 = ≥50%, 3 = ≥90%/automated)*
- 0: Execution ad hoc.
- 1: Some standard procedures.
- 2: **≥50%** of decisions executed via managed workflow.
- 3: **≥90%** / automated execution.

### L8 — Learning
*Do outcomes change future decision rules?*
- 0: Outcomes not fed back.
- 1: Informal lessons learned.
- 2: Outcomes systematically update rules each cycle.
- 3: Continuous, measured learning loop with demonstrated lift.

### L9 — Adaptation
*Does the system reconfigure its **behavior** to changing conditions?* *(within current structure)*
- 0: Rigid; no adaptation.
- 1: Reacts slowly/manually to change.
- 2: Adapts behavior across a known range of conditions.
- 3: Rapid, broad adaptation with short time-to-adapt.

### L10 — Evolution
*Does the system change **its own structure/strategy** over time?* *(structure, not just behavior)*
- 0: Structure unchanged.
- 1: Occasional, externally driven restructuring.
- 2: Periodic deliberate structural change.
- 3: Continuous self-directed structural evolution / high autonomy.

## Section C — Adaptation outcome (for H2)

Self-reported outcome anchors; **triangulate with secondary data where possible**
(these are weaker than measured outcomes and should be validated).
- C1. Time to recover from the most recent significant disruption.
- C2. Improvement in your main performance metric over the reporting period.
- C3. Performance variability under disruption (stable ↔ volatile).

---

## Scoring & quality notes

- **Maturity Profile** = the 11 block scores; **Maturity Index** = their mean;
  **Attained Level** = highest contiguous level ≥2 (report Index alongside it — v1.1 rule).
- **Self-report bias is the main threat.** Mitigate by: ≥2 respondents/unit;
  evidence boxes; and **rater verification** of a subsample against documents
  (compare self-report vs. independent rubric scoring; report agreement).
- This instrument supplies the **independent variable** (maturity). The **dependent
  variable** (outcome) should come from secondary data per
  [`../05-data/candidate-datasets.md`](../05-data/candidate-datasets.md) wherever feasible.

## Ethics

Even organizational surveys typically need ethics/IRB review and informed consent.
Anonymize organizations; store responses per `../05-data/` data-handling rules.

---

_Status: draft v0.1 — pilot with the worked-example cases, then refine wording.
See [`../phd-roadmap.md`](../phd-roadmap.md) Phases 3–4._
