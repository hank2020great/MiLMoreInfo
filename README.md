# MiL: Learning Under Limited Data — Supplementary Materials


This repository provides updated materials for our ICML 2026 submission in response to reviewer feedback during the rebuttal period.

---

## Contents

| File | Description |
|:--|:--|
| `icml2026_full_paper.pdf` | Updated full paper with more materials |
| `MiL+Updated+Supplemental.pdf` | Rigorously updated supplemental materials (67 pages), including completely rewritten proofs (Suppl. A–F), robustness analyses, ablation studies, and extended comparisons |
| `MiL vs SOTA peers .png` | Performance comparison of MiL against four SOTA baselines: Meta-Learning (ProtoNet/MAML), SAM, LNN, and Global Pretraining across all five LH-P benchmarks |

---

## What's Updated

- **Theoretical proofs (Suppl. A–F):** All propositions and theorems have been rigorously rewritten with explicit assumptions, formal probability models, and detailed proof steps.
- **Robustness analysis (Suppl. N):** LHI stability verified across three independent methods (raw features, t-SNE, UMAP) with statistical tests confirming invariance.
- **Extended baselines (Suppl. M, P, Q, U):** 20+ methods compared, including ProtoNet, MAML, SAM, DAE/DDPM pretraining, and Liquid Neural Networks.
- **Ablation study (Suppl. I):** Wilcoxon signed-rank tests confirm each PTC component contributes significantly.
- **New synthetic validation (Suppl. X):** The 'Poisoned Spiral' experiment independently verifies both LH-P conditions (C1 and C2).

---

## Code and Data

Full implementation and benchmark datasets are available at:
[https://anonymous.4open.science/r/micro-learning-LHP-B8FA](https://anonymous.4open.science/r/micro-learning-LHP-B8FA)

---

## Citation

Under review. Please do not distribute.
