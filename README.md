# Agent Eval — Project Semester Report

**Student:** Arnav Jain
**Roll No.:** 102203979
**Institute:** Thapar Institute of Engineering and Technology, Patiala
**Faculty Mentor:** Dr. Anjula Mehto, Assistant Professor
**Industrial Mentor:** Malashree B, Associate Director
**Organization:** Eli Lilly and Company
**Project Duration:** 14 January 2026 – 15 July 2026

---

## Abstract

Agentic AI outputs are probabilistic, free form, and difficult to assess with traditional deterministic testing, and existing open source evaluation libraries lacked governance focused checks, LLM Gateway integration, and multi model consensus. This project delivers **Agent Eval**, a Python SDK that evaluates the outputs of any agentic workflow through a three agent LangGraph pipeline, a fixed catalog of fifteen governance evaluators across five pillars, optional multi model consensus, and a self contained interactive HTML report. Built on the internal Eli Lilly LLM Gateway with GPT 5 and Claude Sonnet, the SDK provides structured, reproducible, and governance aware quality assessment for agentic features before they reach production.

## Three Strengths of the Work

1. **Solves a real engineering problem end to end.** The project addresses a concrete production gap in evaluating agentic AI at Eli Lilly rather than a synthetic academic exercise, and integrates directly with the internal LLM Gateway used by other engineering teams.
2. **Goes beyond tool integration — full architecture design.** The work covers requirement analysis, PoC exploration, custom three agent orchestration, evaluator design across five governance pillars, multi model consensus, scoring algorithm, and self contained reporting, all designed and implemented from scratch.
3. **Leverages existing infrastructure to reduce cost and lock in.** By reusing the internal LLM Gateway and internally approved models, the SDK avoided onboarding a commercial evaluation platform, eliminating recurring licensing costs while retaining full control over evaluator design and future expansion.

## Useful Recommendations

1. **Extend evaluation to multi modal agent outputs** (images, audio, video) through format specific evaluators and model specific judging capabilities.
2. **Add persistent evaluation history and cross run comparison** so teams can track quality trends over time, run regression analysis, and detect drift across agent versions.
3. **Explore adaptive evaluator selection and CI integration** so relevant evaluators are chosen automatically from output structure and evaluations can gate pull requests in a continuous integration pipeline.

---

## Repository Contents

- `main.tex` — Full LaTeX source of the project semester report.
- `Agent_Eval_Presentation.pptx` — Project presentation deck.
- `*.png` — Architecture diagrams, HTML report snapshots, and pillar renderings referenced by the report.
- `EliLilly_Logo.jpeg`, `image.png` — Institute and organization logos used on the title page.

### Build

```bash
pdflatex main.tex
pdflatex main.tex   # second pass for cross-references
```

The build additionally expects the following signed assets to be placed in the repo root before compiling: `IndustrialMentorSign.pdf`, `Project_Sem_Certificate.pdf`, `Arnav_Jain_PeerReview.pdf`.
