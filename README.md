# Yurii Muktarov — AI Agent Developer & LLM Researcher

**Autonomous software engineering · LLM agents · Reasoning systems · Reproducible evaluation**

[One-page CV (PDF)](AI_Developer_CV.pdf) · [CV (Markdown)](CV_AI_DEVELOPER.md) · [Kaggle profile](https://www.kaggle.com/yuriimuktarov) · [GitHub profile](https://github.com/yuriimuktarov)

I develop experimental AI agents that inspect source code, propose and validate changes, explore solutions to reasoning tasks, and evaluate results against independently checked baselines. My current research program, **C-AGI**, focuses on building mechanisms that transfer across tasks rather than relying on unverified demonstrations.

## Official Kaggle results

The scores below are from **completed official submissions** as of **23 November 2026**. They are **public leaderboard scores**, not final/private scores or medals. These competitions use different scoring scales and must not be directly compared.

| Competition | Public score | Completed submission | What the work covers |
|:--|--:|:--|:--|
| [ARC Prize 2026 — ARC-AGI-2](https://www.kaggle.com/competitions/arc-prize-2026-arc-agi-2) | **28.61** | `56162536` · 2026-09-11 | Visual abstraction, symbolic transformations, generalization |
| [ARC Prize 2026 — ARC-AGI-3](https://www.kaggle.com/competitions/arc-prize-2026-arc-agi-3) | **28.15** | `57322706` · 2026-10-17 | Interactive tasks, planning, evaluation of a frozen Franzen A0 baseline |
| [Gemma 4 Developer Agent](https://www.kaggle.com/competitions/gemma-4-developer-agent) | **0.15** | `58673177` · 2026-11-21 | Repository issue repair using a Gemma 4 coding-agent pipeline |

**Gemma coding-agent improvement:** official public score **0.13 → 0.15** (**+15.4% relative**) between submissions `58341417` (2026-11-14) and `58673177` (2026-11-21). This is an observed submission-to-submission gain; broader generalization is still under test.

## Featured research and engineering

### 1. C2-R — autonomous repository repair with Gemma 4

**Goal:** make an LLM coding agent produce valid patches against real repository issues.

**Implemented and investigated:**
- Source-first repository inspection and Python AST-based diagnostics;
- Model-guided patch attempts, Git diff checks, and sandboxed execution;
- Independent validation and baseline comparison through the competition environment;
- Cost tracking (tokens, elapsed time, attempts, regressions) and replayable evidence.

**Measured outcome:** official Kaggle public score improved from 0.13 to 0.15. Not every newer research variant improved upon the frozen C2-R baseline.

### 2. ARC-AGI-2 — abstract visual reasoning

Exploration of programmatic transformations, visual pattern hypotheses, and transfer on unfamiliar grid tasks. The completed competition submission achieved a **28.61 public score**. Unsuccessful follow-up transfer attempts are tracked separately from the best result.

### 3. ARC-AGI-3 — interactive agent research

Research on agent loops, goal semantics, action selection, and independent task evaluation. A completed official **frozen Franzen A0 baseline** submission scored **28.15** publicly. This figure is a benchmark result associated with the account, **not evidence that a new C-AGI controller outperformed that baseline**.

### 4. C-AGI — experimental agent-research framework

**C-AGI is a research program, not a claim of achieved artificial general intelligence.** Its focus is an iterative workflow:

`Task → hypothesis/mechanism → tool execution → independent check → cost accounting → transfer test`

Investigated components include typed proof obligations (Lean), AST/source-guided code repair, counterexample-based debugging, causal task planning, experiment provenance, and portable replay artifacts. Some components are working research prototypes; cross-domain superiority remains unproven.

## How I evaluate systems

- **Frozen controls:** new variants are compared against the strongest reproducible baseline.
- **Independent tests:** separate task outcomes from agent self-reports.
- **Reproducibility:** SHA-256 manifests, recorded submissions, logs and clean replay where available.
- **Economics:** track model calls, tokens, elapsed time and failed attempts, not success rate alone.
- **Honest scope:** distinguish working prototypes, public scores, baseline results and unverified generalization.

## Tools and methods

**Python · LLM agents · Google Gemma 4 · Python AST · Git · Linux/Windows · Kaggle CPU/GPU · JSON · isolated execution · experiment orchestration · reproducible benchmarks · SHA-256**

**Additional research:** Lean proof assistants, solver orchestration, symbolic search, planning, transfer evaluation.

## Evidence and contact

- [Machine-readable competition results](evidence/kaggle_submissions.json)
- [Evidence notes and important limits](evidence/EVIDENCE.md)
- [English CV](CV_AI_DEVELOPER.md) / [PDF CV](AI_Developer_CV.pdf)
- [Kaggle](https://www.kaggle.com/yuriimuktarov) · [GitHub](https://github.com/yuriimuktarov)

*Evidence snapshot: 2026-11-23. The research description is intentionally conservative: no medal, private score, rank, peer-reviewed paper, or production deployment is claimed.*
