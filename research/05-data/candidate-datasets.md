# Candidate Datasets & Evidence Sources

*For scoring systems against [`maturity-rubric.md`](../../docs/evaluation/maturity-rubric.md)
and testing H1 (transfer) and H2 (predictive validity).*

> **Verify before relying on any entry.** Dataset names, access terms, and licenses
> change. Treat this as a starting shortlist to confirm against the provider, not a
> guarantee of current availability or suitability.

---

## The core constraint: unit of analysis

The rubric scores **a system / organization** (a farm operation, a supply-chain
firm, a hospital or care-pathway) — not a transaction, patient, or country. So a
usable dataset must support **both**:

1. **Maturity evidence** — enough descriptive detail per *system* to score Levels 0–10
   (what they observe, model, decide, automate, learn from).
2. **An adaptation outcome over time** — a measurable signal of how well the system
   adapts (shock-recovery time, improvement per cycle, variance under disruption).

…ideally with a **stable organization-level identifier** so (1) and (2) link.

**Implication:** most clean ML/tabular datasets fail criterion (1). The best fits
are **organization-level, longitudinal** sources — and some maturity evidence will
likely need **primary collection** (surveys / structured case studies). See §5.

---

## 1. Agriculture / Rice

| Source | Level | Gives | Access / ethics | Limitation |
|--------|-------|-------|-----------------|------------|
| **FAOSTAT** (FAO) | Country | Production, yield, input use over decades | Open | No system-level maturity signal |
| **USDA NASS / Quick Stats** | Region / farm-survey | Practices, inputs, yields (US) | Open | Aggregated; maturity inferred |
| **World Bank LSMS-ISA** | Farm household (panel) | Practices + outcomes, repeated waves | Open (registration) | Smallholder focus; sparse tech levels |
| **CGIAR / IRRI repositories** | Trial / variety | Rice agronomy, variety trials | Mostly open | Research plots ≠ operating systems |
| Precision-ag / yield-monitor corpora | Farm / field | Sensor, VRI, yield-map data | Fragmented, often proprietary | Hard to assemble at scale |

**Best bet:** LSMS-ISA panels (longitudinal + practice + outcome) supplemented by
case studies of precision operations for the high-maturity end.

## 2. Supply chain / logistics

| Source | Level | Gives | Access / ethics | Limitation |
|--------|-------|-------|-----------------|------------|
| **DataCo Smart Supply Chain** (Kaggle) | Firm / order | Orders, delivery, risk flags | Open | Single firm; synthetic-ish |
| **M5 Forecasting** (Walmart, Kaggle) | Store / item | Hierarchical demand & sales | Open | Forecasting, not maturity |
| **US BTS / Freight Analysis Framework** | Network / mode | Freight flows, performance | Open | Macro; no firm maturity |
| COVID-era disruption datasets | Mixed | Shock + recovery signals | Varies | Heterogeneous, ad hoc |
| Industry 4.0 / SC maturity surveys | Firm | Self-reported maturity | Often paywalled / by request | Self-report bias |

**Best bet:** pair a transaction dataset (DataCo / M5) for the *outcome* with a
**maturity survey or case study** for the *maturity score* of the same firm class.

## 3. Clinical pathways / healthcare

| Source | Level | Gives | Access / ethics | Limitation |
|--------|-------|-------|-----------------|------------|
| **CMS public datasets** (Hospital Compare, readmissions, quality) | **Hospital** | Org-level quality & outcome measures over time | Open | US; coarse process detail |
| **MIMIC-IV** (PhysioNet) | Patient / ICU | Rich clinical process & outcomes | **Credentialing + CITI training + DUA** | Single institution; patient-level |
| **eICU-CRD** (PhysioNet) | Multi-center ICU | Cross-site process variation | Credentialing + DUA | ICU only |
| **AHRQ HCUP** | Encounter / hospital | Utilization, quality | Application + fees | Access friction |
| **NHS Digital** (UK) | Trust / pathway | Org-level pathway data | Application | Jurisdiction-specific |

**Best bet for *this* study:** **CMS hospital-level** data is the strongest single
fit — it is *organization-level*, *longitudinal*, and *outcome-rich*, which matches
the unit-of-analysis constraint better than patient-level MIMIC. **Ethics/IRB and a
DUA are mandatory** for any patient-level source.

---

## 4. Recommended shortlist (start here)

| Domain | Outcome source | Maturity-evidence source |
|--------|----------------|--------------------------|
| Agriculture | LSMS-ISA panels | LSMS practice modules + precision-farm case studies |
| Supply chain | DataCo / M5 | SC maturity survey or structured firm case studies |
| Clinical | **CMS hospital measures** | CMS process/structural measures + hospital documentation |

This trio keeps all three domains at a comparable **organization-over-time** grain.

## 5. The likely gap: primary data is probably unavoidable

Secondary datasets give you **outcomes** well but **maturity scores** poorly — Levels
5–10 (Wisdom, Purpose, Learning, Adaptation, Evolution) rarely appear in public data.
Expect a **mixed-methods** design:

- **Secondary data** → adaptation outcomes (H2 dependent variable).
- **Primary data** (a maturity survey instrument + structured case studies) → the
  rubric scores (independent variable).

This becomes a methodology decision (`../03-methodology/`) and likely needs ethics
approval even for organizational surveys.

## 6. Selection checklist (apply to each candidate)

- [ ] Unit of analysis = system/organization (not transaction/patient/country)?
- [ ] Longitudinal (≥2 time points or a shock + recovery)?
- [ ] Carries an adaptation **outcome** measure?
- [ ] Allows or pairs with **maturity evidence** for the same units?
- [ ] License permits research use & publication?
- [ ] Ethics/DUA/IRB path understood and feasible?
- [ ] Three domains kept at a **comparable grain** (for a fair H1 transfer test)?

---

_Status: shortlist drafted; access, licensing, and suitability to be verified.
See [`../phd-roadmap.md`](../phd-roadmap.md) Phase 4 and Phase 0 (data partnerships)._
