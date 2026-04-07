
# MiL: Learning Under Limited Data — Supplementary Materials

**ICML 2026 Submission #17563**

This repository provides updated materials for our ICML 2026 submission in response to reviewer feedback during the rebuttal period.

---

## Contents

| File | Description |
|:--|:--|
| `icml2026_full_paper.pdf` | Updated full paper with more materials |
| `MiL+Updated+Supplemental.pdf` | Rigorously updated supplemental materials (67 pages), including completely rewritten proofs (Suppl. A–F), robustness analyses, ablation studies, and extended comparisons |
| `MiL vs SOTA peers.png` | Performance comparison of MiL against four SOTA baselines: Meta-Learning (ProtoNet/MAML), SAM, LNN, and Global Pretraining across all five LH-P benchmarks |

---

## What's Updated

- **Theoretical proofs (Suppl. A–F):** All propositions and theorems have been rigorously rewritten with explicit assumptions, formal probability models, and detailed proof steps. We also added a Remark in the Proposition 2 proof in the Supplemental to show Proposition 2: Existence AND strict superiority: they are the same claim.
- **Robustness analysis (Suppl. N):** LHI stability verified across three independent methods (raw features, t-SNE, UMAP) with statistical tests confirming invariance.
- **LH-P Diagnostic Protocol:** We added a new paragraph to demonstrate that LH-P identification is strictly independent of any specific solver, including MiL.
- **Extended baselines (Suppl. M, P, Q, U):** 20+ methods compared, including ProtoNet, MAML, SAM, DAE/DDPM pretraining, and Liquid Neural Networks.
- **Ablation study (Suppl. I):** Wilcoxon signed-rank tests confirm each PTC component contributes significantly.
- **New synthetic validation (Suppl. X):** The 'Poisoned Spiral' experiment independently verifies both LH-P conditions (C1 and C2).
- **New Figure on Synthetic Validation of LH-P Theory and MiL. See  Figure 3**
- **New SOTA impelementations:** We add a new subsection: `\subsection{Comparing MiL with Recent Small-Sample SOTA Models}` in paper. MiL is benchmarked against the latest small-sample foundation models — **TabPFN** (*Nature* 2025) and **TabLLM** (AISTAT 2023). MiL statistically outperforms both (sign test: p = 0.004 vs TabPFN; p = 0.00003 vs TabLLM). Both foundation models suffer majority-class collapse on imbalanced LH-Ps, while MiL achieves 100% minority sensitivity.
- **New Figure for SC-let (an extension of MiL for large vision data): Figure 5**
- **New subsection: Extending MiL to handle large scale vision data: Tiny ImageNet data (00 classes, 100,000 training images, 64 × 64 resolution) and its results on SC-let is added besides the original CIFAR100 data.**
  **New Tables: table 3 and Table 4**
- **New Figure to compare MiL MiL against a global RBF SVM on the complete Poisoned Spiral (N = 2,250, LHI=1.00). (See Figure 8 in the updatd paper)**
  

---

## Code and Data

Full implementation and benchmark datasets are available at:
[https://anonymous.4open.science/r/micro-learning-LHP-B8FA](https://anonymous.4open.science/r/micro-learning-LHP-B8FA)
