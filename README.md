
This professional README revision is structured to highlight your ability to critically analyze state-of-the-art research. It uses the specific technical details from your summaries and presentation to demonstrate depth.

Trustworthy Machine Learning: Research Synthesis & Adversarial Analysis
This repository contains a collection of critical reviews and technical analyses of contemporary research in Trustworthy Machine Learning. The work focuses on three core pillars: Privacy Preservation, Model Interpretability, and Adversarial Robustness.

📑 Research Critical Reviews
These reviews evaluate the technical merit, novelty, and empirical rigor of recent publications. Each review includes a synthesis of the methodology, a critique of strengths and weaknesses, and targeted research questions.

1. Enhancing Facial Privacy Protection via Weakening Diffusion Purification

Core Challenge: Addressing the "diffusion purification" effect where protective adversarial perturbations are unintentionally removed during denoising.


Technical Highlights: * Analysis of a two-stage learning strategy within Latent Diffusion Models (LDM).

Evaluation of per-timestamp unconditional embeddings used as null-text guidance to retain identity-related modifications.

Integration of self-attention guidance to ensure structural consistency and high visual quality.


Critical Insight: While the method shows superior Protection Success Rates (PSR), the review notes a discrepancy in the authors' claims regarding PSNR performance relative to established baselines like TIP-IM.

2. GRAPHTRAIL: Translating GNN Predictions into Human-Interpretable Logical Rules

Core Challenge: Moving beyond local, instance-level explainers to uncover global reasoning patterns in Graph Neural Networks (GNNs).

Technical Highlights:

Decomposition of message-passing GNNs into computation trees to reduce the search space from exponential to linear complexity.

Use of Shapley Values to assess the global impact of computation trees.

Generation of Boolean functions via Symbolic Regression for human-interpretable transparency.


Critical Insight: The review identifies a limitation in capturing the "multiplicity" of concept occurrences due to the reliance on Boolean logic, suggesting a trade-off between simplicity and fidelity.

🎤 Technical Presentation
A comprehensive 60-minute session (40-minute deep dive and 20-minute defense) on the mechanics of backdoor attacks and algorithmic fairness.

Influence-Based Fair Selection for Sample-Discriminative Backdoor Attacks

Authors: Qi Wei, Shuo He, Jiahan Zhang, Lei Feng, Bo An (AAAI 2025).


Problem Statement: Identifying how low "manipulation strength" (visibility) of triggers leads to uneven class-wise Attack Success Rates (ASR).

Proposed Framework (IFS):


Data-Efficient Influence Computation: Utilizing group-based pruning and class prototypes to reduce the search space for poisoned samples.


Fair Sample Selection: Implementing dynamic class-level thresholds to ensure an equal proportion of influential samples are selected from each class.


Analysis & Results: Discussion of the complexity-ASR trade-off and performance across diverse datasets (CIFAR-10, ImageNet-10, Raf-db, and ModelNet40).

📂 Repository Structure
Paper_Summary_1.pdf: Critical analysis of Diffusion-based privacy protection.

Paper_Summary_2.pdf: Evaluation of GNN global explainability.

Paper_Presentation.pdf: Full technical slide deck for Influence-Based Backdoor Attacks.
