---
title: A Grid-Search Framework for Dataset-Specific Calibration of Actigraphy Sleep Detection Algorithms
title_zh: 一种用于体动记录仪睡眠检测算法特定数据集校准的网格搜索框架
authors: "Rahjouei, A."
date: 2026-04-09
pdf: "https://www.biorxiv.org/content/10.64898/2026.04.07.706161v1.full.pdf"
tags: ["query:slp-ns"]
score: 9.0
evidence: 体动记录仪睡眠检测算法的校准框架
tldr: 本研究针对体动记录仪睡眠检测算法中手动调参导致的可重复性差问题，提出了一种基于网格搜索的自动校准框架。通过在PSG验证数据集和双设备数据集上的评估，该框架不仅能替代手动调参，提高睡眠起止时间的检测精度，还能通过集成投票机制有效减少睡眠中短暂觉醒的干扰，显著提升了算法的稳健性和透明度。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-04-07-706161-v1/fig-001.webp\", \"caption\": \"Figure 5. Detection of wake bouts occurring within sleep across actigraphy 513 algorithms. 514 (A) Wake-bout detection rate by reference bout duration. Wake bouts were defined from 515 the reference sleep–wake signal as contiguous runs of wake occurring within sleep (i.e., 516 flanked by sleep on both sides). A bout was considered detected when an algorithm 517 classified ≥50% of epochs within the bout as wake. Detection rates are shown for 518 duration bins (1–2 min, 3–5 min, 6–10 min, 11–20 min, >60 min). Sample sizes for each 519 bin are indicated below the x-axis labels. Colors represent algorithms: Cole–Kripke, 520 Sadeh, Oakley, Crespo, MASDA, Consensus, and Majority. The dashed horizontal line 521 indicates the 50% detection threshold. 522 (B) Overall wake-bout detection rate across all durations. Values represent the 523 percentage of reference wake bouts correctly detected by each algorithm. 524 (C) Mean fraction of wake epochs detected within each bout, averaged by duration bin. 525 This metric reflects how much of each wake bout is identified as wake by the algorithm, 526 independent of the binary detection threshold. 527 528 529\", \"page\": 26, \"index\": 1, \"width\": 977, \"height\": 640}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-04-07-706161-v1/fig-002.webp\", \"caption\": \"Figure 1. Hyperparameter tuning and consensus optimization workflow for actigraphy-301 based sleep detection algorithms. The process is divided into four distinct phases: 302 (Phase 1) Grid Search & Filtering, where parameter grids are defined for five algorithms 303 (Cole-Kripke, Sadeh, Oakley, Crespo, MASDA) and results are filtered to retain only 304 biologically plausible sleep percentages (10–50%); (Phase 2) Pruning for Diversity, 305 which reduces the computational load by selecting the top 𝐾 (e.g., 40) configurations 306\", \"page\": 15, \"index\": 2, \"width\": 977, \"height\": 683}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-04-07-706161-v1/fig-003.webp\", \"caption\": \"Figure 4. Comparison of sleep timing estimates between algorithms and PSG 454 using manual and grid-search parameter configurations. 455\", \"page\": 23, \"index\": 3, \"width\": 977, \"height\": 1241}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-04-07-706161-v1/fig-004.webp\", \"caption\": \"Figure 3. Performance of actigraphy-based sleep–wake algorithms compared with 381 polysomnography (PSG) across 23 subjects. 382 (A) Pooled confusion matrices showing epoch-level classification relative to PSG for 383 each algorithm. 384 (B) Mean performance metrics across subjects (±SD), including Accuracy, Balanced 385 Accuracy, Precision, Recall (Sensitivity), Specificity, Cohen’s κ, F1-score, and Matthews 386 Correlation Coefficient (MCC). 387 (C) Boxplots showing per-subject distributions of performance metrics across the cohort 388 (N = 23). Red dashed lines indicate commonly used reference thresholds for agreement 389 (e.g., κ = 0.6). 390 (D) Heatmap of pairwise Cohen’s κ values showing agreement between algorithms and 391 PSG. 392 393\", \"page\": 19, \"index\": 4, \"width\": 977, \"height\": 608}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-04-07-706161-v1/fig-005.webp\", \"caption\": \"Figure 2. Performance of sleep–wake algorithms using manually selected parameter 337 settings across 23 subjects. 338 (A) Mean per-subject confusion matrices (±SD) relative to the PSG reference. Values 339 represent the percentage of epochs classified as wake or sleep averaged across 340 subjects. Across algorithms, sleep epochs were identified with high sensitivity, whereas 341 wake epochs were more frequently misclassified as sleep. 342 (B) Mean performance metrics (±SD) across subjects, including Accuracy, Balanced 343 Accuracy, Precision, Recall (Sensitivity), Specificity, F1-score, Cohen’s κ, and Matthews 344 Correlation Coefficient (MCC). The red dashed lines indicate reference thresholds for 345 comparison across metrics. 346 (C) Boxplots showing the distribution of performance metrics across subjects (N = 23). 347 While accuracy and F1-score remain consistently high across algorithms, greater 348 variability is observed in specificity and agreement-based metrics such as Cohen’s κ and 349 MCC. 350\", \"page\": 17, \"index\": 5, \"width\": 977, \"height\": 667}]"
motivation: 传统的体动记录仪睡眠评分算法依赖手动调参，存在效率低下且研究结果难以重复的问题。
method: 提出一种基于网格搜索的自动化校准框架，用于优化现有算法参数，并引入共识投票机制处理睡眠碎片化。
result: 实验表明网格搜索在睡眠起止时间预测和觉醒敏感性指标上优于手动调参，并能有效平滑睡眠期间的微小觉醒。
conclusion: 该网格搜索框架为体动记录仪算法提供了一种更具可重复性且高效的参数优化方案，是手动调参的理想替代工具。
---

## 摘要
体动记录仪广泛用于长期睡眠监测，但现有的睡眠-觉醒评分算法通常需要参数调优，而调优过程通常由人工完成，这可能会降低研究的可重复性。本研究针对现有的体动记录仪算法提出了一种基于网格搜索的校准框架，并评估了其作为手动调优实用替代方案的可行性。该方法在两个数据集上进行了评估：一个经过多导睡眠图（PSG）验证的多受试者体动记录数据集，以及一个自行采集的双设备数据集。在经多导睡眠图验证的数据集中，网格搜索优化产生的性能模式与手动参数选择相似，同时略微改善了入睡（sleep onset）和醒来（sleep offset）时间的检测，并在觉醒敏感指标上取得了适度提升。在双设备数据集中，共识和多数投票法有助于减少主睡眠期间发生的短暂觉醒事件的影响，包括可能导致单个算法睡眠预测碎片化的微觉醒。总体而言，这些研究结果表明，网格搜索可以通过更明确且可重复的流程取代手动参数调优，同时在睡眠时间估算方面提供小幅改进，并有利于基于集成的方法处理睡眠期间的觉醒。

## Abstract
Actigraphy is widely used for long-term sleep monitoring, but established sleep-wake scoring algorithms often require parameter tuning, which is commonly performed manually and can reduce reproducibility. In this study, a grid-search-based calibration framework is presented for established actigraphy algorithms and evaluate whether it can serve as a practical alternative to manual tuning. The method was evaluated using two datasets: a multi-subject polysomnography-validated actigraphy dataset and a self-collected dual-device dataset. In the polysomnography-validated dataset, grid-search optimization produced performance patterns similar to manual parameter selection, while slightly improving detection of sleep onset and sleep offset and yielding modest gains in wake-sensitive metrics. In the dual-device dataset, consensus and majority voting were useful for reducing the influence of brief wake episodes occurring within the main sleep period, including micro-awakenings that can fragment sleep predictions across individual algorithms. Overall, these findings show that grid-search can replace manual parameter tuning with a more explicit and reproducible procedure while providing small improvements in sleep timing estimation and benefiting ensemble-based handling of within-sleep wakefulness.

---

## 论文详细总结（自动生成）

这篇论文介绍了一种用于体动记录仪（Actigraphy）睡眠检测算法的自动化校准框架。以下是对该研究的深度结构化总结：

### 1. 论文的核心问题与整体含义
*   **研究背景**：体动记录仪是长期监测睡眠的常用工具，依赖于将肢体活动转化为“睡眠-觉醒”状态的算法（如 Cole-Kripke, Sadeh 等）。
*   **核心问题**：这些传统算法的参数通常是几十年前基于特定人群设定的，或者由研究人员根据经验手动调优。这种“手动调参”过程缺乏透明度、效率低下，且严重影响了研究的可重复性。
*   **整体含义**：本文提出了一种基于**网格搜索（Grid-Search）**的自动化校准框架，旨在为特定数据集提供客观、可重复的参数优化方案，并引入集成学习思想来提升睡眠检测的稳健性。

### 2. 论文提出的方法论
该框架主要分为四个阶段：
*   **阶段 1：网格搜索与初步过滤**：针对五种主流算法（Cole-Kripke, Sadeh, Oakley, Crespo, MASDA）定义参数搜索空间。通过网格搜索遍历组合，并过滤掉产生非生物学合理睡眠比例（如睡眠比例不在 10%–50% 范围内）的参数配置。
*   **阶段 2：多样性剪枝**：为了降低计算负担，从候选配置中筛选出表现最优且具有代表性的 $K$ 个配置。
*   **阶段 3：共识优化（Consensus Optimization）**：引入集成投票机制。
    *   **多数投票（Majority Voting）**：当超过半数的算法配置判定为“睡眠”时，最终结果记为睡眠。
    *   **共识投票（Consensus Voting）**：要求更高的一致性，用于平滑睡眠期间的微小觉醒（Micro-awakenings）。
*   **核心思想**：通过系统化的搜索替代主观判断，利用多算法集成来抵消单一算法对体动噪声的过度敏感。

### 4. 实验设计
*   **数据集**：
    1.  **PSG 验证数据集**：包含 23 名受试者的同步体动数据与多导睡眠图（PSG，金标准）数据，用于评估算法准确性。
    2.  **双设备数据集**：受试者同时佩戴两个设备，用于测试算法在不同硬件采集下的稳定性和一致性。
*   **Benchmark（基准）**：
    *   使用文献中常用的**手动设定参数**作为对照组。
*   **对比方法**：对比了五种经典算法在“手动参数”与“网格搜索优化参数”下的表现，以及新提出的“共识法”和“多数投票法”。

### 4. 资源与算力
*   **算力说明**：论文中**未明确提及**具体的 GPU 或 CPU 型号及训练时长。
*   **分析**：由于体动记录数据属于一维时间序列，且所选的五种算法多为线性加权或简单阈值模型，其计算复杂度远低于深度学习模型。网格搜索在普通商用 CPU 上即可在合理时间内完成，因此算力并非该研究的瓶颈。

### 5. 实验数量与充分性
*   **实验规模**：
    *   使用了 23 例 PSG 样本进行性能验证，这在睡眠研究领域属于标准样本量。
    *   进行了 epoch 级别的混淆矩阵分析、受试者层面的指标分布分析（Accuracy, $\kappa$, F1 等）。
    *   针对“睡眠中觉醒（Wake-bout）”的检测率进行了分段时长（1-2min, 3-5min 等）的详细消融分析。
*   **充分性评价**：实验设计较为全面，不仅验证了整体准确率，还深入探讨了睡眠起止时间（Onset/Offset）的偏差，以及算法对睡眠碎片化的处理能力，实验结果具有较强的说服力。

### 6. 论文的主要结论与发现
*   **性能提升**：网格搜索自动优化的参数在检测“入睡时间”和“醒来时间”上比手动调参更精确，减少了时间偏差。
*   **敏感性优化**：优化后的算法在保持高特异性的同时，适度提升了对觉醒状态（Wake）的敏感性指标（如 Cohen’s $\kappa$ 和 MCC）。
*   **集成优势**：共识投票法能有效过滤掉睡眠期间短暂的、可能由翻身引起的伪觉醒，使睡眠曲线更平滑，更符合临床对“主睡眠期”的定义。
*   **可重复性**：该框架提供了一种标准化的流程，使不同实验室在不同设备上的研究结果更具可比性。

### 7. 优点
*   **解决痛点**：直接针对体动记录仪研究中长期存在的“参数黑箱”和“不可重复”问题。
*   **算法无关性**：该框架具有通用性，可以扩展到任何基于参数的睡眠评分算法。
*   **实用性强**：引入的集成投票机制（Consensus）为处理睡眠碎片化提供了一种简单而有效的非深度学习方案。

### 8. 不足与局限
*   **样本多样性**：PSG 验证集规模（N=23）虽然标准，但对于涵盖不同年龄段、不同睡眠障碍类型的普适性验证仍显不足。
*   **依赖金标准**：网格搜索的效果高度依赖于校准数据集的质量。如果校准集本身存在偏差，优化出的参数可能无法泛化到其他人群。
*   **未对比深度学习**：论文主要关注传统算法的优化，未与近年来兴起的基于深度学习（如 CNN/RNN）的睡眠检测模型进行直接对比。

（完）
