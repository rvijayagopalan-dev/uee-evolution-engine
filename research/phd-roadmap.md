# PhD Roadmap — What Needs to Be Done

A realistic plan to take the maturity-engine idea from "strong proposal" to
"defended doctoral thesis." Indicative timeline assumes a full-time 3.5–4 year PhD;
part-time roughly doubles each phase.

---

## Phase 0 — Get into a position to do a PhD (months 0–3)

- [ ] Identify the field & programs (information systems, systems science, complex
      systems, computational social science, or engineering management).
- [ ] Find a supervisor whose research overlaps (maturity models / digital twins /
      complex adaptive systems / meta-learning).
- [ ] Draft an admission proposal from `docs/evaluation/research-proposal.md`
      (expand to 5–10 pages: gap, questions, method, feasibility, contribution).
- [ ] Confirm data access / partnerships for ≥3 domains.
- [ ] Map funding (scholarship, self-funded, industry-sponsored).

**Deliverable:** accepted proposal + supervisor → `00-proposal/`.

## Phase 1 — Literature review & gap (months 3–12)

- [ ] Systematic review protocol (search strings, inclusion criteria, PRISMA flow).
- [ ] Survey maturity-model lineage (CMMI, DAMA-DMM, capability maturity research).
- [ ] Survey adjacent theory: complex adaptive systems, cybernetics/viable system
      model, digital twins, organizational learning, meta-/transfer learning.
- [ ] Articulate the gap: *no domain-invariant, empirically validated, predictive
      maturity meta-model.*
- [ ] **Answer the "isn't this just CMMI?" objection in writing.** This is the crux.

**Deliverable:** review chapter + a publishable review paper → `01-literature-review/`.

## Phase 2 — Theoretical framework (months 9–15, overlaps Phase 1)

- [ ] Justify the 11 levels from theory, not intuition (which constructs, why, how bounded).
- [ ] Define every construct operationally; state assumptions and scope conditions.
- [ ] Specify falsifiable propositions (the H1/H2/H0 from the proposal, formalized).

**Deliverable:** theory chapter → `02-theoretical-framework/`.

## Phase 3 — Methodology & ethics (months 12–18)

- [ ] Research design (mixed methods: rubric scoring + statistical validation).
- [ ] Validity strategy: construct, internal, external, reliability; threats & mitigations.
- [ ] **Ethics / IRB approval** — required for the clinical domain (human-subjects data).
- [ ] Pre-registration of hypotheses and analysis plan (guards against unfalsifiability).
- [ ] Reproducibility plan (open rubric, code, anonymized data where possible).

**Deliverable:** methodology chapter + IRB approval → `03-methodology/`.

## Phase 4 — The studies (months 15–36)

| Study | Question | Method | Output |
|------|----------|--------|--------|
| **S1** | What's the gap & framework? | Systematic review + synthesis | Review paper |
| **S2** | Is the instrument reliable & valid? | Rubric dev; multi-rater κ; construct validity | Methods paper *(closest to done)* |
| **S3** | Does it transfer? (H1) | Score ≥3 unrelated domains, no structural change | Empirical paper |
| **S4** | Does it predict? (H2) | Level vs. adaptation outcome vs. baseline | Empirical paper |

- [ ] S2: recruit ≥2 raters, score the pilot cases, compute κ, refine to v2.
- [ ] S3: add clinical + one more domain; test for any required structural edits (H0).
- [ ] S4: define adaptation outcomes; correlate; compare to a domain-specific baseline.

**Deliverable:** four studies → `04-studies/`, data in `05-data/`.

## Phase 5 — Publications (continuous, months 12–42)

- [ ] Target venues (e.g., MIS Quarterly / ISR / EJIS; systems & digital-twin journals;
      relevant conferences for early results).
- [ ] 2–3 peer-reviewed papers (thesis-by-publication is an option).

**Deliverable:** submitted/accepted papers → `06-publications/`.

## Phase 6 — Thesis & viva (months 36–48)

- [ ] Integrate chapters into the dissertation (intro → review → theory → method → S1–S4 → discussion → conclusion).
- [ ] Address limitations & generalizability honestly.
- [ ] Internal review → submission → **viva / defense** → corrections.

**Deliverable:** thesis → `07-thesis/`.

---

## The critical-path risks (watch these)

1. **Novelty.** If it reads as CMMI relabeled, it fails. Mitigation: domain-invariance
   + predictive validity must be the contribution, proven empirically.
2. **Falsifiability.** A model that fits everything proves nothing. Mitigation:
   pre-register H0; report failures; the worked example already models this.
3. **Data access.** No real multi-domain data → no transfer claim. Mitigation: secure
   partnerships in Phase 0, before committing.
4. **Ethics delays.** Clinical data IRB can take months. Mitigation: start Phase 3 early.
5. **Scope creep into metaphysics.** Mitigation: the v20 boundary, enforced.

## Immediate next actions (independent of admission)

These can start now and strengthen any application:

- [ ] Run the **S2 reliability pilot**: a second rater scores the two worked-example
      cases; compute κ; log disagreements → rubric v2.
- [ ] Draft the **literature-review protocol** (search terms + the CMMI/DMM positioning).
- [ ] Identify **candidate datasets** for a third domain (clinical pathways).
