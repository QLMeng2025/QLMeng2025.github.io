---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

[Email](mailto:qinglinmeng.work@gmail.com) · [Google Scholar](https://scholar.google.com/citations?user=XpbUfTsAAAAJ&hl=en) · [LinkedIn](https://linkedin.com/in/qinglin-meng-544295137)

## Research Interests

Reinforcement learning, large language models, statistical machine learning, multi-armed bandits, and mechanism design.

## Education

- **Purdue University — Ph.D. in Computer Science**, August 2022–May 2027 (expected). Advisor: [Steve Hanneke](https://stevehanneke.com/).
- **Tsinghua University — B.S. in Mathematical Science**, August 2017–June 2022.

## Experience

### Amazon — Applied Scientist Intern

*August 2026–present*

- Developed an LLM embedding and KNN retrieval pipeline for cost and profit prediction on low-volume and cold-start products, reducing MAE by 15–20% relative to the existing economics-based baseline.
- Post-trained a Transformer embedding model with contrastive learning for product retrieval and cost prediction.

### DoorDash — Machine Learning Engineer Intern

*May–August 2026*

- Formulated peak-time incentive allocation as an MDP to capture sequential supply and demand dynamics.
- Developed and evaluated offline reinforcement learning algorithms to improve service quality while controlling incentive cost.
- Built an end-to-end RL pipeline covering offline training and evaluation, online experimentation, and online serving.

## Publications and Manuscripts

<small>\* Equal contribution; alphabetical author order is indicated separately.</small>

{% include publication-list-compact.html %}

## Research and Working Projects

### Reward-Free RL for Mechanism Design and Dynamic Pricing Optimization

*Advisors: Michael I. Jordan, Zhaoran Wang, and Zhuoran Yang*

- Studied online mechanism design with linear function approximation.
- Developed reward-free exploration over a rich policy space to estimate prices.
- Designed optimistic/pessimistic Q-function approximation algorithms to recover mechanisms over repeated interactions while balancing seller and buyer profit.

### Adaptive Training Data Allocation for LLM Safety via Non-stationary Bandits

*Advisor: Xiangyu Zhang*

- Built a data pipeline with OpenFDA drug data, synthetic patient profiles, and generated scenarios for LLM safety evaluation and training.
- Formulated adaptive post-training data selection as a non-stationary multi-armed bandit problem.
- Implemented sliding-window Thompson Sampling to prioritize failure-prone drugs, reducing mean and worst-case error relative to uniform sampling and baseline curricula on LLaMA-3 and Qwen-2.5.

### Near-Optimal Bandit Learning for Multiclass Classification

*Advisors: Steve Hanneke and Shay Moran*

- Proved a sharp Sauer lemma based on the list-DS dimension.
- Developed a chain-of-list learning algorithm achieving near-optimal sample complexity for multiclass learning with bandit feedback.
- Improved an existing list-learning sample complexity bound by a factor of K⁵.

### A Survey of Architecture-Level Design for Interpretable LLMs

*Advisor: Liangming Pan*

- Analyzed architecture-level interpretability techniques, including codebook features, sparse mixture-of-experts architectures, and sparse autoencoder based steering.

### Reduction for Multiclass Learning

*Advisor: Steve Hanneke*

- Studied multiclass reductions with potentially infinite label spaces.
- Developed a representation preserving agnostic-to-realizable reduction by applying a realizable learner to realizable subsets of the input sample.

## Academic Service

**Reviewer:** Transactions on Machine Learning Research (TMLR), COLM 2026, NeurIPS 2026, and ACL ARR 2026.

## Teaching

**Teaching Assistant, Purdue University**

- **CS 177: Python Programming**, Fall 2023–Fall 2025.
- **CS 573: Data Mining**, Spring 2023.

## Skills

- **Programming:** Python, C++, R, MATLAB, SQL.
- **Software and systems:** PyTorch, TensorFlow, Git, Databricks, Snowflake.
