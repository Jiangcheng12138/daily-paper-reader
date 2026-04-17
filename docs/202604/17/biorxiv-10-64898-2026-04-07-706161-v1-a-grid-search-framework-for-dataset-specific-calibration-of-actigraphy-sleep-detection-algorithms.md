---
title: A Grid-Search Framework for Dataset-Specific Calibration of Actigraphy Sleep Detection Algorithms
title_zh: 一种用于体动记录仪睡眠检测算法特定数据集校准的网格搜索框架
authors: "Rahjouei, A."
date: 2026-04-09
pdf: "https://www.biorxiv.org/content/10.64898/2026.04.07.706161v1.full.pdf"
tags: ["query:slp-ns"]
score: 9.0
evidence: 体动记录仪睡眠检测算法的校准
tldr: 本研究针对体动记录仪睡眠检测算法中手动调参导致的可重复性差问题，提出了一种基于网格搜索的自动校准框架。通过在PSG验证数据集和双设备数据集上的评估，该框架不仅实现了与手动调参相当的性能，还在睡眠起止时间预测和唤醒敏感性指标上有所提升。此外，结合共识投票机制有效减少了微觉醒对睡眠预测的干扰，为体动记录仪算法提供了一种更透明、可重复的参数优化方案。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-04-07-706161-v1/fig-001.webp\", \"caption\": \"Figure 5. Detection of wake bouts occurring within sleep across actigraphy 513 algorithms. 514 (A) Wake-bout detection rate by reference bout duration. Wake bouts were defined from 515 the reference sleep–wake signal as contiguous runs of wake occurring within sleep (i.e., 516 flanked by sleep on both sides). A bout was considered detected when an algorithm 517 classified ≥50% of epochs within the bout as wake. Detection rates are shown for 518 duration bins (1–2 min, 3–5 min, 6–10 min, 11–20 min, >60 min). Sample sizes for each 519 bin are indicated below the x-axis labels. Colors represent algorithms: Cole–Kripke, 520 Sadeh, Oakley, Crespo, MASDA, Consensus, and Majority. The dashed horizontal line 521 indicates the 50% detection threshold. 522 (B) Overall wake-bout detection rate across all durations. Values represent the 523 percentage of reference wake bouts correctly detected by each algorithm. 524 (C) Mean fraction of wake epochs detected within each bout, averaged by duration bin. 525 This metric reflects how much of each wake bout is identified as wake by the algorithm, 526 independent of the binary detection threshold. 527 528 529\", \"page\": 26, \"index\": 1, \"width\": 977, \"height\": 640}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-04-07-706161-v1/fig-002.webp\", \"caption\": \"Figure 1. Hyperparameter tuning and consensus optimization workflow for actigraphy-301 based sleep detection algorithms. The process is divided into four distinct phases: 302 (Phase 1) Grid Search & Filtering, where parameter grids are defined for five algorithms 303 (Cole-Kripke, Sadeh, Oakley, Crespo, MASDA) and results are filtered to retain only 304 biologically plausible sleep percentages (10–50%); (Phase 2) Pruning for Diversity, 305 which reduces the computational load by selecting the top 𝐾 (e.g., 40) configurations 306\", \"page\": 15, \"index\": 2, \"width\": 977, \"height\": 683}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-04-07-706161-v1/fig-003.webp\", \"caption\": \"Figure 4. Comparison of sleep timing estimates between algorithms and PSG 454 using manual and grid-search parameter configurations. 455\", \"page\": 23, \"index\": 3, \"width\": 977, \"height\": 1241}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-04-07-706161-v1/fig-004.webp\", \"caption\": \"Figure 3. Performance of actigraphy-based sleep–wake algorithms compared with 381 polysomnography (PSG) across 23 subjects. 382 (A) Pooled confusion matrices showing epoch-level classification relative to PSG for 383 each algorithm. 384 (B) Mean performance metrics across subjects (±SD), including Accuracy, Balanced 385 Accuracy, Precision, Recall (Sensitivity), Specificity, Cohen’s κ, F1-score, and Matthews 386 Correlation Coefficient (MCC). 387 (C) Boxplots showing per-subject distributions of performance metrics across the cohort 388 (N = 23). Red dashed lines indicate commonly used reference thresholds for agreement 389 (e.g., κ = 0.6). 390 (D) Heatmap of pairwise Cohen’s κ values showing agreement between algorithms and 391 PSG. 392 393\", \"page\": 19, \"index\": 4, \"width\": 977, \"height\": 608}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-04-07-706161-v1/fig-005.webp\", \"caption\": \"Figure 2. Performance of sleep–wake algorithms using manually selected parameter 337 settings across 23 subjects. 338 (A) Mean per-subject confusion matrices (±SD) relative to the PSG reference. Values 339 represent the percentage of epochs classified as wake or sleep averaged across 340 subjects. Across algorithms, sleep epochs were identified with high sensitivity, whereas 341 wake epochs were more frequently misclassified as sleep. 342 (B) Mean performance metrics (±SD) across subjects, including Accuracy, Balanced 343 Accuracy, Precision, Recall (Sensitivity), Specificity, F1-score, Cohen’s κ, and Matthews 344 Correlation Coefficient (MCC). The red dashed lines indicate reference thresholds for 345 comparison across metrics. 346 (C) Boxplots showing the distribution of performance metrics across subjects (N = 23). 347 While accuracy and F1-score remain consistently high across algorithms, greater 348 variability is observed in specificity and agreement-based metrics such as Cohen’s κ and 349 MCC. 350\", \"page\": 17, \"index\": 5, \"width\": 977, \"height\": 667}]"
motivation: 传统的体动记录仪睡眠评分算法依赖手动调参，过程繁琐且缺乏可重复性。
method: 提出一种网格搜索框架，用于针对特定数据集自动优化现有睡眠检测算法的参数。
result: 该方法在睡眠起止时间估算上优于手动调参，并能通过集成投票机制有效处理睡眠中的微觉醒。
conclusion: 网格搜索框架是手动调参的可靠替代方案，能显著提高体动记录仪算法的校准效率和结果的可重复性。
---

## 摘要
体动记录仪广泛用于长期睡眠监测，但现有的睡眠-觉醒评分算法通常需要参数调优，而这通常由人工完成，可能会降低研究的可重复性。本研究针对现有的体动记录仪算法提出了一种基于网格搜索的校准框架，并评估其是否可以作为手动调优的实用替代方案。该方法在两个数据集上进行了评估：一个经过多导睡眠图（PSG）验证的多受试者体动记录数据集，以及一个自行收集的双设备数据集。在多导睡眠图验证的数据集中，网格搜索优化产生的性能模式与手动参数选择相似，同时略微改善了入睡和觉醒时间的检测，并在觉醒敏感指标上取得了适度提升。在双设备数据集中，共识和多数投票法有助于减少主睡眠期内发生的短暂觉醒事件的影响，包括可能导致单个算法睡眠预测碎片化的微觉醒。总体而言，这些研究结果表明，网格搜索可以通过更明确且可重复的流程取代手动参数调优，同时在睡眠时间估算方面提供小幅改进，并有利于基于集成的方法处理睡眠期间的觉醒。

## Abstract
Actigraphy is widely used for long-term sleep monitoring, but established sleep-wake scoring algorithms often require parameter tuning, which is commonly performed manually and can reduce reproducibility. In this study, a grid-search-based calibration framework is presented for established actigraphy algorithms and evaluate whether it can serve as a practical alternative to manual tuning. The method was evaluated using two datasets: a multi-subject polysomnography-validated actigraphy dataset and a self-collected dual-device dataset. In the polysomnography-validated dataset, grid-search optimization produced performance patterns similar to manual parameter selection, while slightly improving detection of sleep onset and sleep offset and yielding modest gains in wake-sensitive metrics. In the dual-device dataset, consensus and majority voting were useful for reducing the influence of brief wake episodes occurring within the main sleep period, including micro-awakenings that can fragment sleep predictions across individual algorithms. Overall, these findings show that grid-search can replace manual parameter tuning with a more explicit and reproducible procedure while providing small improvements in sleep timing estimation and benefiting ensemble-based handling of within-sleep wakefulness.

---

## 论文详细总结（自动生成）

以下是对论文《一种用于体动记录仪睡眠检测算法特定数据集校准的网格搜索框架》（A Grid-Search Framework for Dataset-Specific Calibration of Actigraphy Sleep Detection Algorithms）的结构化深入总结：

### 1. 论文的核心问题与整体含义
*   **研究背景**：体动记录仪（Actigraphy）是长期监测睡眠-觉醒模式的常用工具。然而，现有的经典评分算法（如 Cole-Kripke, Sadeh 等）高度依赖参数设置。
*   **核心问题**：在实际应用中，研究人员往往根据经验“手动调参”以适应特定的设备硬件或受试人群。这种做法不仅耗时耗力，且缺乏透明度和可重复性，导致不同研究之间的数据难以比较。
*   **整体含义**：本研究旨在提出一个自动化的、基于网格搜索（Grid-Search）的校准框架，通过系统化的参数优化取代主观的手动调整，从而提高睡眠检测的准确性和科学研究的可重复性。

### 2. 论文提出的方法论
该框架将校准过程分为四个关键阶段：
*   **阶段 1：网格搜索与初步过滤**：针对五种主流算法（Cole-Kripke, Sadeh, Oakley, Crespo, MASDA）定义参数搜索空间。运行算法后，过滤掉产生非生物学合理结果（例如觉醒比例不在 10%–50% 范围内）的参数配置。
*   **阶段 2：多样性剪枝**：为了降低计算复杂度并保证配置的代表性，从候选池中筛选出前 $K$ 个（如 40 个）在性能和多样性上表现最优的配置。
*   **阶段 3：共识优化（Consensus Optimization）**：引入集成学习思想，通过“共识投票（Consensus）”或“多数投票（Majority）”机制结合多个算法的预测结果。
*   **阶段 4：最终评估**：在独立的验证集上，利用多导睡眠图（PSG）作为金标准，对优化后的参数配置进行性能评估。

### 3. 实验设计
*   **数据集**：
    1.  **PSG 验证数据集**：包含 23 名受试者的同步体动记录与 PSG 数据，用于评估算法的分类准确性。
    2.  **双设备数据集**：由作者自行收集，受试者同时佩戴两个不同设备，用于测试算法在不同硬件间的一致性。
*   **Benchmark（基准）**：以 PSG 标注的每分钟（Epoch）睡眠/觉醒状态为金标准。
*   **对比方法**：
    *   五种经典算法的**手动调参版本**。
    *   五种经典算法的**网格搜索优化版本**。
    *   基于网格搜索结果的**集成投票法**（Consensus & Majority）。

### 4. 资源与算力
*   **算力说明**：论文中**未明确指出**具体的 GPU 型号或训练时长。
*   **分析**：由于体动记录数据属于一维时间序列，且所涉及的经典算法（非深度学习）计算量相对较小，网格搜索在普通工作站或商用服务器上即可高效完成，不需要大规模 GPU 集群支持。

### 5. 实验数量与充分性
*   **实验规模**：涵盖了 5 种不同的算法，并在 23 名受试者的 PSG 数据上进行了逐分钟的对比分析。
*   **充分性评价**：
    *   **优点**：实验设计较为全面，不仅对比了分类准确率，还对比了睡眠起止时间（Onset/Offset）等临床关键指标。引入双设备数据集验证了框架的鲁棒性。
    *   **局限**：23 人的样本量在睡眠研究中虽属标准，但对于验证算法的普适性（如针对不同睡眠障碍人群）仍显略窄。

### 6. 论文的主要结论与发现
*   **性能对等与提升**：网格搜索框架达到的性能与经验丰富的人工调参相当，甚至在睡眠起止时间的预测精度上略有提升。
*   **唤醒敏感性改善**：优化后的算法在识别睡眠中的短暂觉醒（Wake-sensitive metrics）方面表现更好。
*   **集成法的优势**：共识投票机制能有效减少“微觉醒”对睡眠预测的干扰，解决了单一算法容易导致睡眠预测碎片化的问题。
*   **可重复性**：该框架提供了一种标准化的流程，使得不同实验室之间的体动记录仪数据校准具有可比性。

### 7. 优点（亮点）
*   **自动化与标准化**：将原本“黑箱”化、主观的手动调参过程转化为透明、可重复的数学优化过程。
*   **集成创新**：通过共识机制结合多种算法的优势，提高了系统对复杂体动信号的容错能力。
*   **临床相关性**：研究不仅关注统计学指标（如 Accuracy），更关注临床关注的睡眠参数（如睡眠潜伏期、觉醒时间）。

### 8. 不足与局限
*   **依赖金标准**：该框架的校准过程仍需要一部分 PSG 数据作为参考。在完全缺乏 PSG 数据的实地研究中，如何进行初始校准仍是挑战。
*   **计算开销**：虽然单次运行快，但如果参数网格设置过大，搜索空间会呈指数级增长。
*   **人群覆盖面**：实验主要基于健康或特定受试者，对于患有严重睡眠呼吸暂停或周期性肢体运动障碍（PLMS）的患者，该框架的有效性尚需进一步验证。

（完）
