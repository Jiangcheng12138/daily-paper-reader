---
title: "Single-cell Transcriptomic Variance Analysis Reveals Intercellular Circadian Desynchrony in the Alzheimer's Affected Human Brain"
title_zh: 单细胞转录组变异分析揭示阿尔茨海默病患者大脑中的细胞间昼夜节律失步
authors: "Hollis, H. C., Veltri, A., Korac, K., Menon, V., Bennett, D. A., Ronnekleiv-Kelly, S., Kim, J., Anafi, R. C."
date: 2026-03-25
pdf: "https://www.biorxiv.org/content/10.64898/2026.03.23.713759v1.full.pdf"
tags: ["query:slp-ns"]
score: 8.0
evidence: 阿尔茨海默病患者大脑中的细胞间昼夜节律失步
tldr: 本研究针对组织节律受细胞振幅和同步性共同影响的模糊性，开发了名为ORPHEUS的分析方法，通过单细胞转录组表达方差的12小时节律特征来量化细胞间的同步性。在验证该方法后，研究发现小鼠肝脏和人类大脑中的昼夜节律同步性与MTORC活性呈正相关，并揭示了阿尔茨海默病患者兴奋性神经元中存在显著的细胞间去同步化现象，为分析单细胞昼夜节律协调提供了新工具。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-03-23-713759-v1/fig-001.webp\", \"caption\": \"\", \"page\": 30, \"index\": 1, \"width\": 1024, \"height\": 1024}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-03-23-713759-v1/fig-002.webp\", \"caption\": \"\", \"page\": 33, \"index\": 2, \"width\": 1024, \"height\": 1024}]"
motivation: 旨在解决大块组织节律分析中无法区分细胞振幅变化与细胞间同步性差异的根本模糊性问题。
method: 开发了名为ORPHEUS的统计方法，利用细胞间表达方差中独特的12小时节律特征来量化细胞间的相位异质性。
result: 发现MTORC活性与昼夜节律同步性呈正相关，并观察到阿尔茨海默病患者大脑兴奋性神经元中细胞同步性大幅丧失。
conclusion: ORPHEUS通过解耦细胞振幅与同步性，为研究疾病状态下组织内部的昼夜节律协调提供了可解释的新工具。
---

## 摘要
大块组织节律源于数千个单个细胞振荡的协调。大块节律振幅的差异可能反映了底层细胞振荡器振幅的变化，或者是其时间相干性的变化。为了解决这一根本性的歧义，我们开发了 ORPHEUS（利用统计矩估计振荡节律相位异质性），这是一种通过利用其在细胞间表达变异上施加的独特 12 小时节律特征来量化细胞失步的分析方法。在通过计算机模拟以及小鼠视交叉上核 (SCN) 数据验证 ORPHEUS 后，我们将其应用于小鼠肝脏和人脑数据，以揭示与疾病和通路相关的细胞间同步性差异。在两种组织中，我们发现 MTORC 活性较高的细胞和样本中，昼夜节律同步性也更高。最关键的是，我们观察到阿尔茨海默病 (AD) 痴呆受试者的兴奋性神经元中存在严重的细胞同步性丧失。通过解耦细胞振幅和同步性的影响，ORPHEUS 为分析时序单细胞数据中的昼夜节律协调提供了一种新的、具有可解释性的工具。

## Abstract
Bulk tissue rhythms arise from the coordination of thousands of individual cellular oscillations. Bulk rhythm amplitude differences may reflect changes in the amplitude of the underlying cellular oscillators or changes in their temporal coherence. To resolve this fundamental ambiguity, we developed ORPHEUS (Oscillatory Rhythm Phase Heterogeneity Estimated Using Statistical-moments), an analytical method that quantifies cellular desynchrony by leveraging the unique 12hr rhythmic signature it imparts on intercellular expression variance. After validating ORPHEUS in silico and on data from the mouse suprachiasmatic nucleus (SCN), we applied it to data from the mouse liver and human brain to uncover disease- and pathway-related differences in intercellular synchrony. In both tissues, we found that circadian synchrony is higher in cells and samples with higher MTORC activity. Most critically, we observed a dramatic loss of cellular synchrony in excitatory neurons from subjects with Alzheimers Disease (AD) dementia. By decoupling the influence of cellular amplitude and synchrony, ORPHEUS introduces a new, interpretable tool for analyzing circadian coordination in time-course single-cell data.