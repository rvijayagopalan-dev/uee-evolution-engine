# Maturity Engine — Operational Scoring Rubric (Levels 0–10)

*Companion to [`research-proposal.md`](./research-proposal.md). This is the
instrument that makes the 11-level ladder **measurable** and therefore testable.*

---

## How to use this rubric

- A **system** is scored independently at each level; it does **not** have to be
  contiguous (a system can be strong at Data but weak at Learning).
- Each level has an **objective indicator** (what to look for), a **measurable
  signal** (the evidence), and a **0–3 attainment scale**.
- Score with **≥2 independent raters**; report inter-rater agreement (κ / α).
- The rubric is **fixed before** looking at domain data — no per-domain tuning.

### Attainment scale (applies to every level)

| Score | Meaning |
|------:|---------|
| **0** | Absent — no evidence of the capability |
| **1** | Ad hoc — present informally / manually / inconsistently |
| **2** | Systematic — repeatable process or tooling in place |
| **3** | Optimized — automated, measured, and continuously improved |

A system's **level is "attained"** when it scores ≥2 on that level *and* all lower levels.

---

## The 11 Levels

| Lvl | Name | Objective indicator | Measurable signal | Rice example | Supply-chain example | Clinical example |
|----:|------|---------------------|-------------------|--------------|----------------------|------------------|
| **0** | Reality | The physical/operational system and its actors are explicitly identified | Documented inventory of entities, actors, inputs, outputs | Seed, soil, water, farmer, harvest catalogued | SKUs, suppliers, nodes, lanes mapped | Patients, clinicians, sites, encounters defined |
| **1** | Observation | Signals are captured from reality | % of key variables instrumented; sampling frequency | Sensors/drones/satellites on rainfall, soil moisture, yield | IoT/telemetry on inventory, transit, demand | EHR/vitals/labs captured per encounter |
| **2** | Data | Observations are stored with structure & governance | Schema coverage; metadata completeness; data-quality score | Field/variety/yield/input records, governed | Order/shipment/inventory tables, lineage | Structured clinical data, coding standards |
| **3** | Knowledge | Relationships & rules are made explicit | Existence of an ontology / knowledge graph; % entities linked | Variety→soil→climate→yield graph | Supplier→lead-time→risk graph | Symptom→diagnosis→pathway graph |
| **4** | Intelligence | The system produces recommendations | Decision coverage; recommendation accuracy vs. ground truth | "Plant variety X, expected 7.5 t/ha" | Reorder-point / routing recommendations | Diagnostic / treatment decision support |
| **5** | Wisdom | Trade-offs are reasoned about explicitly | Documented objective trade-offs; multi-criteria decisions | Yield vs. water; profit vs. soil health | Cost vs. resilience; speed vs. carbon | Efficacy vs. risk vs. cost-of-care |
| **6** | Purpose | Decisions are tied to declared goals | Traceability of decisions to objectives; goal coverage | Food security, prosperity, export goals | Service level, margin, sustainability goals | Outcomes, access, safety, equity goals |
| **7** | Action | Decisions are executed as managed workflows | % of decisions executed via workflow/automation | Planting/irrigation/harvest plans run | Procurement/fulfilment orchestration | Care plans / order sets executed |
| **8** | Learning | Outcomes change future decision rules | # of decision rules updated from outcomes per cycle; lift over time | "Yield +15%, water −20%" → updated practice | Forecast error → retrained model | Outcome data → updated protocol |
| **9** | Adaptation | The system reconfigures to changing conditions | Time-to-adapt to a shock; range of conditions handled | Seed/irrigation strategy shifts with climate | Re-routing under disruption | Surge / variant response reconfiguration |
| **10** | Evolution | The system changes its own structure/strategy over generations | Structural change rate; autonomy level (manual→autonomous) | Traditional → precision → AI → autonomous farming | Manual → digital → autonomous supply network | Reactive → learning health system |

---

## Composite metrics (per system)

- **Attained Level** — highest contiguous level with score ≥ 2 (headline number).
- **Maturity Profile** — the full 11-value vector (0–3 each); preserves non-contiguous strengths.
- **Maturity Index** — mean of the 11 scores, 0–3 (continuous, good for correlations).

## Linking back to the research question

- **H1 (Transfer):** the *same table* scores all three domains with only the
  example column changing — no rows added or removed. If any domain needs a new
  row, that is a recorded **H0 falsification**.
- **H2 (Predictive validity):** test whether *Attained Level* or *Maturity Index*
  correlates with an adaptation outcome (e.g., shock-recovery time, per-cycle
  improvement) better than a domain-specific baseline maturity model.

## Rater protocol (for reliability)

1. Each rater scores every level 0–3 from the same evidence pack, blind to the other.
2. Compute Cohen's κ (2 raters) or Krippendorff's α (>2); target ≥ 0.7.
3. Adjudicate disagreements; refine *wording* of indicators only — never the
   structure — and re-document the rubric version.

---

*One-line purpose:* **This rubric is what turns "Level 8 — Learning" from a slogan
into a number two independent people can agree on — the precondition for testing
the engine at all.**
