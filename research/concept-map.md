# Concept Map / Mind Map — PhD Program

*A single-page visual of the whole program: scopes, thesis core, theory, method,
studies, governance, and field. Mermaid renders in GitHub/VS Code; a text outline
follows for plain viewers.*

---

## 1. Mind map (whole program at a glance)

```mermaid
mindmap
  root((Domain-Invariant Maturity Model of Adaptive Capability))
    Vision and Scope
      Scope 1 PhD provable core
      Scope 2 Program ladder plus invariant
      Scope 3 Vision universal science of adaptation
      Scope 4 Frontier universal language of intelligence
    Thesis Core
      Hard core measurable domain-invariant predictive
      11-Level Ladder Reality to Evolution
      H1 Transfer
      H2 Predictive validity
      H0 Falsifier
    Theory
      DIKW levels 2 to 5
      Cybernetics sense-adapt loop
      Org learning single double deutero
      Dynamic capabilities levels 9 to 10
    Method
      Rubric v1.1
      Self-report survey instrument
      Data three domains
      Validity kappa and construct
    Studies
      S1 Systematic review gap
      S2 Instrument validation
      S3 Cross-domain transfer
      S4 Predictive validity
    Governance
      Scope contract
      Lakatos validation
      Definition of done
    Field
      Prior theses Legg Shalizi Wang
      Active labs SFI UCL DeepMind
      Sibling program UTI-ERP
```

## 2. Logical dependency map (how the core connects)

```mermaid
flowchart TD
    GAP[S1 Gap proven in 2x2 matrix] --> INSTR[S2 Validated instrument]
    THEORY[Theory: DIKW + adaptive loop] --> LADDER[11-Level Ladder]
    LADDER --> INSTR
    INSTR --> H1[S3 H1 Transfer across 3 domains]
    INSTR --> H2[S4 H2 Predicts adaptation outcomes]
    DATA[Outcome data + maturity survey] --> H1
    DATA --> H2
    H1 --> CONTRIB[Contribution: domain-invariant validated predictive model]
    H2 --> CONTRIB
    H0[H0 falsifier: any domain needs structural edit] -.refutes.-> CONTRIB
    CONTRIB --> DONE[Definition of Done: viva passed]
```

## 3. Document map (where each file sits)

```mermaid
flowchart LR
    subgraph Preliminary [docs/evaluation - grounded base]
      EVAL[evolution-map] --> PROP0[research-proposal]
      RUBRIC[maturity-rubric v1.1] --> WORK[worked-example]
    end
    subgraph Governance [research - top level]
      VS[vision-and-scope] --> S4[scope-4-frontier]
      VS --> LAK[eternal-research-program-validation]
      HOR[research-horizons]
      UTI[related-work-uti-erp]
    end
    subgraph Pipeline [research 00-07]
      P0[00 proposal + definition-of-done]
      P1[01 review protocol + related-theses]
      P2[02 theoretical-framework]
      P3[03 survey instrument]
      P4[04 studies]
      P5[05 candidate-datasets]
      P6[06 publications]
      P7[07 thesis]
    end
    PROP0 --> P0
    RUBRIC --> P3
    WORK --> P4
    P0 --> P1 --> P2 --> P3 --> P4 --> P6 --> P7
    P5 --> P4
    LANDSCAPE[active-research-landscape] --> P0
    VS --> P0
```

---

## 4. Text outline (plain-viewer fallback)

- **PhD Program — Domain-Invariant Maturity Model of Adaptive Capability**
  - **Vision & Scope** — scope 1 (PhD) → 2 (program) → 3 (vision) → 4 (frontier)
  - **Thesis Core**
    - Hard core: adaptive capability is measurable, domain-invariant, predictive
    - 11-Level Ladder: Reality → … → Evolution
    - Hypotheses: H1 transfer · H2 predictive validity · H0 falsifier
  - **Theory** — DIKW (L2–L5) + cybernetics loop + organizational learning (single/double/deutero) + dynamic capabilities (L9–L10)
  - **Method** — rubric v1.1 · survey instrument · 3-domain data · reliability (κ) + construct validity
  - **Studies** — S1 review (gap) · S2 instrument · S3 transfer · S4 prediction
  - **Governance** — scope contract · Lakatos validation · definition of done
  - **Field** — prior theses (Legg, Shalizi, Wang) · active labs (SFI, UCL, DeepMind) · sibling UTI-ERP

---

_Status: concept map v0.1 — regenerate when the study plan or scope structure changes._
