# Cortex Research Coverage Map — What Else the Product Needs

*Companion to [`enterprise-strategic-cortex-validation.md`](./enterprise-strategic-cortex-validation.md).
Routes every Cortex module/layer NOT underwritten by the PhD to its actual research
area, with a maturity flag. Conclusion: the Cortex is a multi-disciplinary platform;
the PhD is ~1 of a dozen research areas it draws on.*

---

## PhD-covered kernel (for reference)

✅ Enterprise Awareness (health score) · ✅ Strategic Reasoning (via H2) ·
✅ Decision Intelligence (maturity→outcome prediction). These are the only modules
with a scientific moat.

## Modules NOT covered by the PhD

| Module | Research area(s) | Field maturity |
|--------|------------------|----------------|
| **Intent & Alignment / Goal Intelligence** (L6) | Goal-setting theory (Locke & Latham); OKR/MBO; multi-criteria decision analysis; goal modeling in RE (i*, KAOS); goal-reasoning AI; AI intent alignment | Mixed — mgmt mature; AI intent-alignment **frontier** |
| **Scenario Intelligence** (L5) | Strategic foresight / scenario planning (Schoemaker); system dynamics (Forrester, Sterman); causal inference (Pearl, counterfactuals); Monte Carlo / decision analysis | Mature research; engineering-buildable |
| **Digital Twin & Simulation** (L3) | Digital-twin engineering; enterprise modeling / EA (ArchiMate, SysML); ontologies; process mining (van der Aalst); simulation science | Mature / active |
| **Executive Council — AI agents, collective decisions** (L7/L8–L10) | Multi-agent systems & MARL; LLM-agent / agentic AI; computational social choice; mechanism design & game theory; human-AI teaming | **Research frontier** (riskiest module) |
| **Learning & Adaptation** (L8–L10) | Reinforcement / continual / meta-learning; self-adaptive systems (autonomic computing, MAPE-K); adaptive control; AutoML; organizational learning (automated) | Active → **frontier** for autonomy |

## Foundation layers (mostly engineering / applied research)

| Layer | Research area | Maturity |
|-------|---------------|----------|
| Knowledge Plane | Knowledge graphs, ontology engineering, KR&R, semantic web | Mature |
| Memory Plane | RAG, vector DBs, memory-augmented NNs, episodic/long-term agent memory | Active, fast-moving |
| Context Engineering | Context-aware computing, situational awareness, context/prompt engineering | Active (LLM era) |
| Agent Operating System | Agent orchestration, workflow/BPM, multi-agent platforms, LLMOps | Engineering (emerging) |
| Data & Integration | Data engineering, integration, MDM, data mesh/fabric | Mature |
| Tech & Infrastructure | Cloud/distributed systems, MLOps | Mature |

## Governance & Security (built-in)

AI governance · responsible/trustworthy AI · explainable AI (XAI) · AI safety &
alignment · privacy-preserving ML · model governance · audit/accountability · GRC.
*(Active research + maturing practice.)*

---

## The three-bucket synthesis

1. **Mature / engineering** (digital twin, knowledge plane, data, infra, scenario sim)
   — buildable now, low research risk, **no moat**.
2. **Active research** (memory/RAG, context, agent orchestration, XAI/governance)
   — buildable, evolving fast.
3. **Frontier** (Executive Council collective AI decisions; autonomous L8–L10 Learning
   & Adaptation) — the **unproven, hardest** modules; each arguably its own multi-year
   research program. **Flag as research, do not ship as finished product.**

## Connections

- The uncovered cognitive modules (memory, knowledge, agents, simulation) are exactly
  **UTI-ERP's EEI / ERP-X / ERP-SIM** territory — see
  [`../research/related-work-uti-erp.md`](../research/related-work-uti-erp.md).
- They map onto the **Tier 1–3 areas** in
  [`../research/research-horizons.md`](../research/research-horizons.md).
- So "what covers the rest" = the **scope-2 research programme** + standard AI/data
  engineering.

## Implication

No single PhD covers the Cortex. The PhD owns the falsifiable adaptation-science core;
the rest is a **portfolio**: ship bucket 1, integrate bucket 2, and treat bucket 3 as
research — never market the two frontier modules as delivered capability (the
commercial form of the scope-overreach trap).

_Status: coverage map v0.1 — based on the v1 architecture image; revisit as modules
are scoped for build vs. research._
