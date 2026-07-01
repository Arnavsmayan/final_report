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

The project implements an SDK for evaluating agentic AI outputs using an LLM as judge approach. It uses a three agent pipeline with governance evaluators across five pillars, multi model consensus, and a self contained HTML report. The project demonstrates a practical industry solution developed through requirement analysis, proof of concept validation, and production implementation.

## Three Strengths of the Work

1. The project addresses a real evaluation gap in agentic AI systems within an enterprise environment.
2. The work goes beyond a simple evaluation library and includes architecture design, technology evaluation, and custom implementation.
3. The solution integrates well with existing infrastructure, reducing cost while maintaining strong evaluation capabilities.

## Useful Recommendations

1. Extend evaluation support to multi modal agent outputs alongside text based outputs.
2. Add persistent evaluation history and cross run comparison for longitudinal quality tracking.
3. Explore continuous integration gating for automated evaluation of agentic features.

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
