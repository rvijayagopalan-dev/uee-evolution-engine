# Study 4 (H2) — Predictive Validity, Operationalized for Agriculture

*Closes the key design gap: turns "maturity predicts adaptation outcomes" into a
measurable, testable study for one domain. Template to replicate for supply chain and
clinical. Read with [`../00-proposal/definition-of-done.md`](../00-proposal/definition-of-done.md)
and [`../05-data/candidate-datasets.md`](../05-data/candidate-datasets.md).*

> **H2:** A system's adaptive-capability maturity predicts its adaptation outcomes
> **better than a domain-specific baseline.** Pre-registered; a null result still
> completes the study (see definition of done).

---

## 1. Unit of analysis
The **farm operation** (or farm-household), observed over multiple seasons (panel).

## 2. Independent variable (the model under test)
**Maturity** of the farm's adaptive capability, scored with the
[rubric v1.1](../../docs/evaluation/maturity-rubric.md) + survey:
- **Maturity Index** (mean of the 11 levels, 0–3) — primary, continuous.
- **Attained Level** (0–10) — secondary, reported alongside (v1.1 rule).

## 3. Dependent variable — adaptation outcome (the gap, now defined)

**Construct:** how well the farm *absorbs and recovers from a shock* (climate or price).

**Primary measure — Yield Resilience to Shock (YRS):**
> The ratio of realized yield in a shock season to the farm's expected
> (pre-shock trend) yield — i.e., proportional yield retained under disturbance.
> `YRS = yield_shock / expected_yield_trend` (1.0 = no loss; <1.0 = loss).

**Secondary measure — Recovery Time (RT):**
> Number of seasons until yield returns to ≥95% of the pre-shock trend after the shock.

**Shock definition:** a season where a documented climate event (drought/flood/heat,
e.g., rainfall or temperature anomaly beyond the regional 10th/90th percentile) or a
price shock (input/output price move beyond a set threshold) occurred. Identified from
climate/market records, independent of the maturity score.

## 4. Baseline (what maturity must beat)
A **domain-specific comparator** predicting the same outcome:
- **Primary baseline:** a technology-adoption / input-intensity index (e.g., irrigation
  + mechanization + improved-seed adoption) — the conventional "advancement" proxy.
- **Secondary baseline:** farm size + wealth proxy alone (controls-only model).

H2 holds only if **Maturity Index adds predictive power beyond these.**

## 5. Analysis
- **Model:** regression of YRS (and RT) on Maturity Index + controls.
- **Controls:** farm size, region/agro-ecological zone, crop type, shock severity.
- **Test of H2:** does adding Maturity Index to the baseline model significantly
  improve fit (ΔR² / likelihood-ratio; lower AIC; or ΔAUC if outcome is dichotomized
  as "resilient ≥ threshold")? Pre-registered threshold: **p < 0.05 and meaningful
  effect size**, maturity beating baseline.
- **Robustness:** alternative shock thresholds; YRS and RT both; multilevel model for
  region clustering.

## 6. Data
Panel with farm-level practices + yields + a shock window — e.g., **World Bank
LSMS-ISA** (practice modules → maturity; yield series → outcome) supplemented by
climate records for shock identification. See candidate-datasets.

## 7. Threats to validity & mitigations
| Threat | Mitigation |
|--------|-----------|
| Maturity confounded with wealth/size | Include as controls; test incremental validity over a wealth-only baseline |
| Reverse causality (good outcomes → invest in maturity) | Use maturity measured *before* the shock season (temporal precedence) |
| Shock mis-classification | Objective climate/market thresholds, set a priori |
| Data granularity (practices coarse) | Score conservatively; report measurement error; triangulate survey + records |
| Survivorship (failed farms drop out) | Model attrition; report as a limitation |

## 8. Pre-registration checklist
- [ ] Hypothesis, DV, baseline, and analysis fixed **before** touching outcome data.
- [ ] Shock thresholds and controls specified a priori.
- [ ] Null result reported regardless.

---

_Status: S4 agriculture operationalization v0.1 — replicate for supply chain
(e.g., service-level recovery after a disruption) and clinical (e.g., outcome
stability under a demand surge). This is the template that makes H2 a real study._
