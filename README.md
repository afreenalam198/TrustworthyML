# Trustworthy Machine Learning: Research Synthesis & Adversarial Analysis

[cite_start]This repository contains a curated collection of technical analyses and critical reviews of contemporary research in **Trustworthy Machine Learning**[cite: 4, 523]. The work focuses on three core pillars: **Privacy Preservation**, **Model Interpretability**, and **Adversarial Robustness**.

---

## 📑 Research Reviews

These reviews evaluate the technical merit, novelty, and empirical rigor of recent publications. [cite_start]Each review includes a synthesis of methodology, a critique of strengths and weaknesses, and targeted research questions[cite: 17, 31, 539, 551].

### 1. [Enhancing Facial Privacy Protection via Weakening Diffusion Purification](Paper_Summary_1.pdf)
* [cite_start]**Core Challenge**: Addressing the "diffusion purification" effect where protective adversarial perturbations are unintentionally removed during denoising[cite: 526].
* **Technical Highlights**:
    * [cite_start]Analysis of a two-stage learning strategy within Latent Diffusion Models (LDM)[cite: 528].
    * [cite_start]Evaluation of per-timestamp unconditional embeddings used as null-text guidance to retain identity-related modifications[cite: 529].
    * [cite_start]Integration of self-attention guidance to ensure structural consistency and high visual quality[cite: 531, 532].
* [cite_start]**Critical Insight**: While the method shows superior Protection Success Rates (PSR), the review identifies an overstatement regarding PSNR performance, noting that baseline methods like TIP-IM maintain higher scores[cite: 535, 549, 550].

### 2. [GRAPHTRAIL: Translating GNN Predictions into Human-Interpretable Logical Rules](Paper_Summary_2.pdf)
* [cite_start]**Core Challenge**: Moving beyond local, instance-level explainers to uncover global reasoning patterns in Graph Neural Networks (GNNs)[cite: 8].
* **Technical Highlights**:
    * [cite_start]Decomposition of message-passing GNNs into computation trees to reduce the search space from exponential to linear complexity[cite: 10, 11].
    * [cite_start]Use of Shapley Values to assess the global impact of computation trees[cite: 12].
    * [cite_start]Generation of Boolean functions via Symbolic Regression for human-interpretable transparency[cite: 13].
* [cite_start]**Critical Insight**: The review identifies a limitation in capturing the "multiplicity" of concept occurrences due to the reliance on Boolean logic, suggesting a trade-off between simplicity and fidelity[cite: 29, 30].

---

## 🎤 Technical Presentation

[cite_start]A comprehensive 60-minute session (40-minute deep dive and 20-minute defense) on the mechanics of backdoor attacks and algorithmic fairness[cite: 42].

### [Influence-Based Fair Selection for Sample-Discriminative Backdoor Attacks](CS7064%20Trustworthy%20Machine%20Learning%20Presentation.pdf)
* [cite_start]**Authors**: Qi Wei, Shuo He, Jiahan Zhang, Lei Feng, Bo An (AAAI 2025)[cite: 45, 508].
* [cite_start]**Problem Statement**: Identifying how low "manipulation strength" (visibility) of triggers leads to uneven class-wise Attack Success Rates (ASR) due to unfair instance selection[cite: 159, 160, 161].
* **Proposed Framework (IFS)**:
    * [cite_start]**Data-Efficient Influence Computation**: Utilizing group-based pruning and class prototypes to reduce the search space for poisoned samples[cite: 217, 218, 232].
    * [cite_start]**Fair Sample Selection**: Implementing dynamic class-level thresholds to ensure an equal proportion of influential samples are selected from each class[cite: 289, 291, 292].
* [cite_start]**Analysis & Results**: Evaluation of performance across diverse datasets, including CIFAR-10, ImageNet-10, Raf-db, and ModelNet40[cite: 331, 332, 333].

---

## 📂 Repository Structure
* `Paper_Summary_1.pdf`: Critical analysis of Diffusion-based facial privacy protection.
* `Paper_Summary_2.pdf`: Evaluation of global explainability and logical rule translation for GNNs.
* `CS7064 Trustworthy Machine Learning Presentation.pdf`: Full technical slide deck for Influence-Based Fair Selection (IFS).
