# Worked Example — Applying the Rubric to Two Domains

*A dry run of [`maturity-rubric.md`](./maturity-rubric.md) on two representative
cases. Purpose: produce real maturity profiles, and — more importantly — surface
ambiguous indicators **before** a full multi-rater study.*

> **Note on data.** These are *illustrative* cases built from publicly typical
> patterns (a tech-forward rice operation; a mid-maturity regional distributor),
> not proprietary datasets. They exist to test the *instrument*, not to make
> empirical claims. Real studies must use sourced evidence packs.

---

## Case A — Precision Rice Operation ("FarmCo")

A commercial rice producer using soil sensors, satellite imagery, a variety-yield
model, and variable-rate irrigation; agronomists review AI recommendations before
acting; practices are revised season to season from logged outcomes.

| Lvl | Capability | Evidence | Score (0–3) |
|----:|-----------|----------|:-----------:|
| 0 | Reality | Full asset/actor inventory in farm-management system | 3 |
| 1 | Observation | Soil-moisture sensors + satellite NDVI; daily cadence | 3 |
| 2 | Data | Governed field/variety/yield/input records; some gaps in pest logs | 2 |
| 3 | Knowledge | Variety→soil→climate→yield model exists; not a formal graph | 2 |
| 4 | Intelligence | Yield/irrigation recommendations, validated vs. actuals | 3 |
| 5 | Wisdom | Yield-vs-water trade-off explicit; profit-vs-soil informal | 2 |
| 6 | Purpose | Yield & cost goals declared; sustainability goals vague | 2 |
| 7 | Action | Irrigation automated (VRI); planting/harvest semi-manual | 2 |
| 8 | Learning | Season-end review updates next-season practice | 2 |
| 9 | Adaptation | Irrigation adapts within season to weather | 2 |
| 10 | Evolution | Moving precision→AI-assisted; not autonomous | 1 |

- **Attained Level:** **9** (contiguous ≥2 through L9; L10 = 1 breaks the chain)
- **Maturity Profile:** `[3,3,2,2,3,2,2,2,2,2,1]`
- **Maturity Index:** 2.18 / 3

---

## Case B — Regional Distribution Network ("DistCo")

A mid-size distributor with an ERP, telemetry on shipments, demand forecasting,
and reorder automation; replanning under disruption is largely manual; no
self-restructuring of the network.

| Lvl | Capability | Evidence | Score (0–3) |
|----:|-----------|----------|:-----------:|
| 0 | Reality | SKUs, suppliers, nodes, lanes mapped in ERP | 3 |
| 1 | Observation | Shipment + inventory telemetry; demand partially instrumented | 2 |
| 2 | Data | Order/shipment/inventory tables with lineage | 3 |
| 3 | Knowledge | Supplier→lead-time→risk relationships partly modeled | 2 |
| 4 | Intelligence | Reorder-point & forecast recommendations | 2 |
| 5 | Wisdom | Cost-vs-resilience considered in S&OP, inconsistently | 1 |
| 6 | Purpose | Service-level & margin goals declared and tracked | 3 |
| 7 | Action | Procurement/reorder orchestrated; routing semi-manual | 2 |
| 8 | Learning | Forecast error feeds model retraining quarterly | 2 |
| 9 | Adaptation | Disruption re-routing largely manual / playbook-based | 1 |
| 10 | Evolution | No structural self-change of the network | 0 |

- **Attained Level:** **4** (L5 = 1 breaks the chain at Wisdom)
- **Maturity Profile:** `[3,2,3,2,2,1,3,2,2,1,0]`
- **Maturity Index:** 1.91 / 3

---

## Side-by-side

| Metric | FarmCo (rice) | DistCo (supply chain) |
|--------|:-------------:|:---------------------:|
| Attained Level | 9 | 4 |
| Maturity Index | 2.18 | 1.91 |
| Weakest level | L10 Evolution (1) | L10 Evolution (0), L5/L9 (1) |
| Strongest levels | L0,L1,L4 (3) | L0,L2,L6 (3) |

**Reading it:** the *Attained Level* (contiguous) and *Maturity Index* (mean) tell
different stories — DistCo's mean is close to FarmCo's, but a single weak rung
(Wisdom) collapses its attained level to 4. This is the intended behavior: it
flags that DistCo's bottleneck is **trade-off reasoning**, not data or tooling.

---

## What the dry run surfaced (the actual point)

These ambiguities must be resolved in the rubric *before* a real multi-rater study:

1. **"Formal graph" vs. "model" (L3).** Both cases scored 2 because relationships
   exist but not as an explicit knowledge graph. *Decision needed:* does L3 require
   a graph, or any explicit relational model? Current wording is ambiguous → tighten.
2. **Contiguous vs. profile reporting.** Attained Level is brittle to one weak
   rung. *Recommendation:* report **both** Attained Level and Maturity Index as
   standard; never use Attained Level alone.
3. **"Semi-manual" scoring (L7).** Raters could justify 1 or 2. *Add* a threshold:
   score 2 requires ≥50% of decisions executed via managed workflow.
4. **Purpose without measurement (L6).** DistCo tracks goals (3) but FarmCo's
   sustainability goals are "vague" (scored within 2). *Add:* L6 score 3 requires
   decisions *traceable* to declared goals, not merely goals existing.
5. **Evolution vs. Adaptation overlap (L9/L10).** Need a crisp line: L9 =
   reconfigures *behavior* within current structure; L10 = changes *the structure
   itself*. Add one-line disambiguation to the rubric.

**Next action:** fold fixes 1–5 into `maturity-rubric.md` as v1.1, then run the
same two cases with two independent raters to measure κ.

---

*One-line purpose:* **A dry run isn't about the scores — it's about finding the
five places where two smart raters would disagree, and fixing the wording first.**
