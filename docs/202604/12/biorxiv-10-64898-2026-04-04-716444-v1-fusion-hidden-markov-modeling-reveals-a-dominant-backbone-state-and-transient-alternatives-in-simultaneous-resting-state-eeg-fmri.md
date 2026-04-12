---
title: Fusion hidden Markov modeling reveals a dominant backbone state and transient alternatives in simultaneous resting-state EEG-fMRI
title_zh: 融合隐马尔可夫建模揭示了同步静息态 EEG-fMRI 中的主导骨干状态与瞬态备选状态
authors: "Cruz, G. E."
date: 2026-04-07
pdf: "https://www.biorxiv.org/content/10.64898/2026.04.04.716444v1.full.pdf"
tags: ["query:slp-ns"]
score: 8.0
evidence: 静息态EEG-fMRI中的大脑动力学
tldr: 本研究针对同步EEG-fMRI多模态融合建模的挑战，开发了一套基于隐马尔可夫模型（HMM）的融合框架。通过对健康成年人静息态数据的分析，识别出由一个高占用率的“骨干状态”和两个瞬时替代状态组成的动态系统。该方法不仅提供了实用的全脑融合工作流，还揭示了电生理与血氧动力学网络在不同潜在脑状态下的差异化表达，为理解静息态脑动态提供了新的生物学解释。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-04-04-716444-v1/fig-001.webp\", \"caption\": \"Figure 3. Final-state dynamics of the full-data 𝑲 = 𝟑 fusion HMM.\", \"page\": 26, \"index\": 1, \"width\": 976, \"height\": 781}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-04-04-716444-v1/fig-002.webp\", \"caption\": \"Figure 5. Descriptive cross-modal BOLD-EEG block structure of the final 𝑲 = 𝟑 fusion-HMM solution\", \"page\": 29, \"index\": 2, \"width\": 974, \"height\": 1072}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-04-04-716444-v1/fig-003.webp\", \"caption\": \"Figure 4. State-wise BOLD network organization of the final 𝑲 = 𝟑 fusion-HMM solution.\", \"page\": 27, \"index\": 3, \"width\": 976, \"height\": 1049}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-04-04-716444-v1/fig-004.webp\", \"caption\": \"Figure 2. LOSO-CV model selection and shortlist stability supported a three-state fusion HMM.\", \"page\": 24, \"index\": 4, \"width\": 852, \"height\": 895}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-04-04-716444-v1/fig-005.webp\", \"caption\": \"Figure 6. Parcelized cortical maps of dominant and contrast BOLD state organization.\", \"page\": 31, \"index\": 5, \"width\": 774, \"height\": 1014}]"
motivation: 旨在解决同步EEG-fMRI数据在全脑动态建模中难以有效融合、对齐以及缺乏稳定共享特征空间的问题。
method: 开发了一种基于隐马尔可夫模型（HMM）的融合框架，通过严格的多模态对齐和留一法交叉验证来确定最佳脑状态模型。
result: 识别出一个占主导地位的“骨干状态”和两个瞬时替代状态，发现不同状态下电生理与血氧动力学网络的表达模式存在显著差异。
conclusion: 该研究提供了一种可重复的全脑EEG-fMRI融合分析流程，并揭示了静息态下低阶脑动态的生物学组织规律。
---

## 摘要
同步 EEG-fMRI 为研究大脑动力学提供了一种强大的手段，但将这两种模态整合到一个通用的全脑模型中仍然具有挑战性。在本研究中，我开发了一种用于静息态同步 EEG-fMRI 的融合建模框架，该框架强调精细的多模态对齐、稳定共享特征空间的构建，以及基于交叉验证和可重复性的模型选择。利用来自公开同步 EEG-fMRI 数据集的 12 名健康成人的 15 次睁眼静息态运行数据，我构建了一个无滞后、最小 15-TR 的融合数据集，包含 3550 个保留的 TR 和 124.25 分钟的可用数据。留一受试者交叉验证（leave-one-subject-out cross-validation）支持一个简洁的三状态融合隐马尔可夫模型。在最终的全数据方案中，一个状态作为主导骨干状态出现，具有最高的占用率、最强的持久性以及最清晰的标准 BOLD 网络组织。两个较低占用率的状态表现为瞬态备选状态：其中一个表现为骨干状态的广泛减弱版本，而另一个则显示出更具选择性的网络权重重组。这些状态在描述性的跨模态 BOLD-EEG 结构上也存在差异，表明电生理和血流动力学网络表达在不同的潜在脑状态下可能具有不同的对齐方式。这些结果既提供了一个实用的全脑 EEG-fMRI 融合工作流，也对低阶静息态大脑动力学提供了具有生物学解释性的说明。

## Abstract
Simultaneous EEG-fMRI offers a powerful way to study brain dynamics, but combining the two modalities in a common whole-brain model remains challenging. Here, I developed a fusion modeling framework for resting-state simultaneous EEG-fMRI that emphasized careful multimodal alignment, construction of a stable shared feature space, and cross-validated, reproducibility-based model selection. Using 15 eyes-open resting-state runs from 12 healthy adults in an open simultaneous EEG-fMRI dataset, I constructed a no-lag, 15-TR-minimum fusion dataset comprising 3550 retained TRs and 124.25 min of usable data. A leave-one-subject-out cross-validation sweep supported a parsimonious three-state fusion hidden Markov model. In the final full-data solution, one state emerged as a dominant backbone state with the highest occupancy, strongest persistence, and clearest canonical BOLD network organization. Two lower-occupancy states behaved as transient alternatives: one appeared as a broadly attenuated version of the backbone state, whereas the other showed more selective network reweighting. The states also differed in their descriptive cross-modal BOLD-EEG structure, suggesting that electrophysiological and hemodynamic network expression may align differently across latent brain states. These results provide both a practical whole-brain EEG-fMRI fusion workflow and a biologically interpretable account of low-order resting-state brain dynamics.