# Systematic Literature Review — Protocol

*The make-or-break component. Its job is to prove a **gap**: that no
domain-invariant, empirically validated, predictive maturity meta-model exists —
and thereby to differentiate this work from the CMMI / DMM lineage. If this fails,
the thesis is a relabel.*

---

## 1. Review questions

- **RQ1.** What maturity / capability models exist, and what is their *scope of
  applicability* (single-domain vs. cross-domain)?
- **RQ2.** Which models have been **empirically validated** (reliability, construct
  validity) versus proposed conceptually only?
- **RQ3.** Which models offer **predictive validity** (maturity predicts an outcome),
  versus descriptive staging only?
- **RQ4.** Is there any **domain-invariant** maturity model tested across unrelated
  domains without structural modification? *(The gap hypothesis: no.)*

## 2. Method

Follow **PRISMA 2020** for transparent search, screening, and reporting.
Pre-register the protocol (e.g., OSF) before screening to guard against bias.

### 2.1 Databases
- Scopus, Web of Science (core coverage)
- IEEE Xplore, ACM Digital Library (engineering / CS)
- AIS eLibrary (information systems)
- PubMed (clinical maturity / learning-health-system literature)
- Google Scholar (grey-literature / snowballing only, capped)

### 2.2 Search strings (adapt syntax per database)
```
("maturity model" OR "capability maturity" OR "maturity assessment"
  OR "stage model" OR "maturity framework")
AND
("cross-domain" OR "domain-agnostic" OR "domain-independent" OR "generaliz*"
  OR "transfer" OR "universal")
AND
("validat*" OR "empirical" OR "reliability" OR "predict*" OR "construct validity")
```
Plus a focused lineage string:
```
("CMMI" OR "Capability Maturity Model" OR "DAMA" OR "DMM"
  OR "data maturity" OR "digital maturity" OR "analytics maturity")
```

### 2.3 Inclusion criteria
- Peer-reviewed; presents, validates, or reviews a maturity/capability model.
- English; no date floor (CMM lineage starts ~1990s).
- Reports scope, validation, or predictive use.

### 2.4 Exclusion criteria
- Vendor white papers / marketing maturity grids (logged separately as grey lit).
- Models with no defined levels or assessment method.
- Pure application of an existing model with no methodological content.

### 2.5 Screening & extraction
- Two reviewers screen title/abstract independently; record κ; adjudicate conflicts.
- Full-text screen with the same rules.
- Extraction sheet per included paper: model name, domain(s), # levels, theoretical
  basis, **validation type**, **predictive evidence (y/n)**, **cross-domain tested (y/n)**.

### 2.6 Quality appraisal
Appraise empirical papers for reliability reporting, construct validity, sampling,
and falsifiability. Flag conceptual-only models distinctly.

## 2A. Sources & tools (where to search)

### Core academic databases (run the formal search here)
| Database | Why for this topic | Access |
|----------|--------------------|--------|
| **Scopus** | Broadest coverage + citation analysis; primary index | Institutional |
| **Web of Science** | Curated; strong citation chaining | Institutional |
| **AIS eLibrary (AISeL)** | **Critical** — IS digital/data/analytics maturity models cluster here | Mostly free |
| **IEEE Xplore** | CMMI / capability-maturity & engineering | Institutional |
| **ACM Digital Library** | Software / process maturity | Institutional |
| **PubMed** | Clinical maturity / learning-health-system | Free |
| **Business Source / ABI-Inform (ProQuest)** | Management, dynamic capabilities | Institutional |

### Open / free indexes (no institution needed)
- **OpenAlex**, **Semantic Scholar** — free APIs for reproducible, scriptable search/extraction.
- **Lens.org** — scholarly + patents (tech-evolution angle).
- **Google Scholar** — recall/snowballing only (not reproducible enough to be primary).
- **CORE.ac.uk** — open-access full texts.

### Citation-chaining & gap-spotting (the gap usually surfaces here)
- **Connected Papers** — visual field map around a seed; reveals empty space.
- **Research Rabbit** / **Litmaps** — forward/backward citation discovery & lineage (CMMI → DMM → digital maturity).
- **Inciteful** / **Citation Gecko** — citation-network gap finding.

### AI-assisted (triage only — never replaces human screening)
- **Elicit** (extraction tables), **Scite.ai** (supported vs. contested claims — useful for "is anyone predictive?"), **Consensus** (quick orientation).
- ⚠️ These hallucinate/miss; included-paper decisions and the gap claim must be human-verified.

### Registration & management
- **Register on OSF before screening** (PROSPERO only if a health angle) — this is what makes the gap claim credible vs. post-hoc.
- **Rayyan** (two-reviewer blind screening + κ), **Zotero** (references/dedup), **Covidence** if available.

### Recommended starting sequence
1. Register protocol on **OSF**.
2. **Seed scan** (~1 day): CMMI/DMM seeds into **Connected Papers** + **Research Rabbit** to see the lineage and where it thins.
3. Formal search in **Scopus + WoS + AISeL + IEEE + PubMed** → export to **Zotero/Rayyan** → dedup.
4. Two-reviewer screen in **Rayyan** (record κ).
5. Extract with the §2.5 sheet (Elicit-assisted, human-verified).
6. Plot on the §3 2×2 matrix; show the bottom-right cell is empty → the gap.

> Highest-value first move for this specific gap: **AISeL + Scopus** for the corpus,
> then **Connected Papers** to visually confirm no cluster sits in the
> "cross-domain + validated + predictive" region.

## 3. Synthesis & the positioning argument

Map every included model on two axes:

```
            Predictive validity →
            no                         yes
   single  | descriptive grids     | domain-specific
   domain  | (most maturity models)| predictive models
   --------+-----------------------+----------------------
   cross-  | conceptual "universal"| ◀ TARGET CELL ▶
   domain  | claims (untested)     | (claimed empty = the gap)
```

**The contribution lives in the bottom-right cell.** The review must show it is
empty — i.e., no model is simultaneously (a) cross-domain, (b) empirically
validated, and (c) predictive — with the matrix as evidence.

## 4. The "isn't this just CMMI?" rebuttal (must be written)

A standalone subsection contrasting this work with the dominant lineage:

| Dimension | CMMI / DMM / digital-maturity lineage | This work |
|-----------|----------------------------------------|-----------|
| Scope | Single domain (software, data, digital) | Domain-invariant claim, tested |
| Validation | Often practitioner-derived / conceptual | Reliability + construct validity |
| Use | Descriptive staging / benchmarking | **Predictive** of adaptation outcomes |
| Falsifiability | Rarely tested to fail | Pre-registered null (H0) |
| Unit | Process areas | System adaptation across 11 levels |

If any existing model already occupies the target cell, **the topic must pivot** —
better to learn that in the review than in the viva.

## 5. Adjacent literatures to position against (not just maturity models)

- Complex adaptive systems; cybernetics / Viable System Model
- Organizational learning & absorptive capacity
- Digital twins (maturity & adaptation)
- Dynamic capabilities (strategy) — note conceptual overlap with Levels 8–10
- Meta-learning / transfer learning (the ML sense of "transfer")

## 6. Outputs
- PRISMA flow diagram + extraction dataset → `./` (this folder)
- The 2×2 evidence matrix and the gap statement
- A publishable systematic-review paper (Study 1) → `../06-publications/`

---

_Status: protocol draft v0.1 — register, then run screening. See
[`../phd-roadmap.md`](../phd-roadmap.md) Phase 1._
