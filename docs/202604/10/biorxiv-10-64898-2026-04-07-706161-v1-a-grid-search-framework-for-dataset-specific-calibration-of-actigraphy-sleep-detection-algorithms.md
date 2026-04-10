---
title: A Grid-Search Framework for Dataset-Specific Calibration of Actigraphy Sleep Detection Algorithms
title_zh: 一种用于体动记录仪睡眠检测算法特定数据集校准的网格搜索框架
authors: "Rahjouei, A."
date: 2026-04-09
pdf: "https://www.biorxiv.org/content/10.64898/2026.04.07.706161v1.full.pdf"
tags: ["query:slp-ns"]
score: 9.0
evidence: 体动记录仪睡眠检测算法的校准
tldr: 本研究针对体动记录仪睡眠检测算法中手动调参导致的可重复性差问题，提出了一种基于网格搜索的自动校准框架。通过在PSG验证数据集和双设备数据集上的评估，该框架不仅能替代手动调参，还提升了睡眠起止时间的检测精度及对觉醒指标的敏感度。此外，结合共识投票机制有效减少了睡眠期间微觉醒对预测结果的干扰，为睡眠监测提供了更具可重复性和准确性的技术方案。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-04-07-706161-v1/fig-001.webp\", \"caption\": \"Figure 5. Detection of wake bouts occurring within sleep across actigraphy 513 algorithms. 514 (A) Wake-bout detection rate by reference bout duration. Wake bouts were defined from 515 the reference sleep–wake signal as contiguous runs of wake occurring within sleep (i.e., 516 flanked by sleep on both sides). A bout was considered detected when an algorithm 517 classified ≥50% of epochs within the bout as wake. Detection rates are shown for 518 duration bins (1–2 min, 3–5 min, 6–10 min, 11–20 min, >60 min). Sample sizes for each 519 bin are indicated below the x-axis labels. Colors represent algorithms: Cole–Kripke, 520 Sadeh, Oakley, Crespo, MASDA, Consensus, and Majority. The dashed horizontal line 521 indicates the 50% detection threshold. 522 (B) Overall wake-bout detection rate across all durations. Values represent the 523 percentage of reference wake bouts correctly detected by each algorithm. 524 (C) Mean fraction of wake epochs detected within each bout, averaged by duration bin. 525 This metric reflects how much of each wake bout is identified as wake by the algorithm, 526 independent of the binary detection threshold. 527 528 529\", \"page\": 26, \"index\": 1, \"width\": 977, \"height\": 640}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-04-07-706161-v1/fig-002.webp\", \"caption\": \"Figure 1. Hyperparameter tuning and consensus optimization workflow for actigraphy-301 based sleep detection algorithms. The process is divided into four distinct phases: 302 (Phase 1) Grid Search & Filtering, where parameter grids are defined for five algorithms 303 (Cole-Kripke, Sadeh, Oakley, Crespo, MASDA) and results are filtered to retain only 304 biologically plausible sleep percentages (10–50%); (Phase 2) Pruning for Diversity, 305 which reduces the computational load by selecting the top 𝐾 (e.g., 40) configurations 306\", \"page\": 15, \"index\": 2, \"width\": 977, \"height\": 683}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-04-07-706161-v1/fig-003.webp\", \"caption\": \"Figure 4. Comparison of sleep timing estimates between algorithms and PSG 454 using manual and grid-search parameter configurations. 455\", \"page\": 23, \"index\": 3, \"width\": 977, \"height\": 1241}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-04-07-706161-v1/fig-004.webp\", \"caption\": \"Figure 3. Performance of actigraphy-based sleep–wake algorithms compared with 381 polysomnography (PSG) across 23 subjects. 382 (A) Pooled confusion matrices showing epoch-level classification relative to PSG for 383 each algorithm. 384 (B) Mean performance metrics across subjects (±SD), including Accuracy, Balanced 385 Accuracy, Precision, Recall (Sensitivity), Specificity, Cohen’s κ, F1-score, and Matthews 386 Correlation Coefficient (MCC). 387 (C) Boxplots showing per-subject distributions of performance metrics across the cohort 388 (N = 23). Red dashed lines indicate commonly used reference thresholds for agreement 389 (e.g., κ = 0.6). 390 (D) Heatmap of pairwise Cohen’s κ values showing agreement between algorithms and 391 PSG. 392 393\", \"page\": 19, \"index\": 4, \"width\": 977, \"height\": 608}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-04-07-706161-v1/fig-005.webp\", \"caption\": \"Figure 2. Performance of sleep–wake algorithms using manually selected parameter 337 settings across 23 subjects. 338 (A) Mean per-subject confusion matrices (±SD) relative to the PSG reference. Values 339 represent the percentage of epochs classified as wake or sleep averaged across 340 subjects. Across algorithms, sleep epochs were identified with high sensitivity, whereas 341 wake epochs were more frequently misclassified as sleep. 342 (B) Mean performance metrics (±SD) across subjects, including Accuracy, Balanced 343 Accuracy, Precision, Recall (Sensitivity), Specificity, F1-score, Cohen’s κ, and Matthews 344 Correlation Coefficient (MCC). The red dashed lines indicate reference thresholds for 345 comparison across metrics. 346 (C) Boxplots showing the distribution of performance metrics across subjects (N = 23). 347 While accuracy and F1-score remain consistently high across algorithms, greater 348 variability is observed in specificity and agreement-based metrics such as Cohen’s κ and 349 MCC. 350\", \"page\": 17, \"index\": 5, \"width\": 977, \"height\": 667}]"
motivation: 传统的体动记录仪睡眠评分算法依赖手动参数调整，过程繁琐且缺乏可重复性。
method: 开发了一种基于网格搜索的校准框架，用于针对特定数据集自动优化算法参数并进行集成评估。
result: 该方法在睡眠起止时间预测和觉醒敏感性指标上优于手动调参，并能通过集成投票减少微觉醒引起的预测碎片化。
conclusion: 网格搜索框架是手动调参的可靠替代方案，能显著提高睡眠检测算法的透明度、可重复性及性能。
---

## 摘要
体动记录仪广泛用于长期睡眠监测，但既有的睡眠-觉醒评分算法通常需要参数调优，而这种调优通常由人工完成，可能会降低研究的可重复性。本研究针对既有的体动记录仪算法提出了一种基于网格搜索的校准框架，并评估其是否可以作为人工调优的实用替代方案。该方法通过两个数据集进行了评估：一个经过多导睡眠图（PSG）验证的多受试者体动记录数据集，以及一个自行采集的双设备数据集。在经多导睡眠图验证的数据集中，网格搜索优化产生的性能模式与人工参数选择相似，同时略微改善了入睡（sleep onset）和醒来（sleep offset）时间的检测，并在觉醒敏感指标上取得了适度提升。在双设备数据集中，共识和多数投票法有助于减少主睡眠期内发生的短暂觉醒事件的影响，包括可能导致单个算法睡眠预测碎片化的微觉醒。总体而言，这些研究结果表明，网格搜索可以通过更明确且可重复的流程取代人工参数调优，同时在睡眠时间估算方面提供小幅改进，并有利于基于集成的方法处理睡眠期间的觉醒。

## Abstract
Actigraphy is widely used for long-term sleep monitoring, but established sleep-wake scoring algorithms often require parameter tuning, which is commonly performed manually and can reduce reproducibility. In this study, a grid-search-based calibration framework is presented for established actigraphy algorithms and evaluate whether it can serve as a practical alternative to manual tuning. The method was evaluated using two datasets: a multi-subject polysomnography-validated actigraphy dataset and a self-collected dual-device dataset. In the polysomnography-validated dataset, grid-search optimization produced performance patterns similar to manual parameter selection, while slightly improving detection of sleep onset and sleep offset and yielding modest gains in wake-sensitive metrics. In the dual-device dataset, consensus and majority voting were useful for reducing the influence of brief wake episodes occurring within the main sleep period, including micro-awakenings that can fragment sleep predictions across individual algorithms. Overall, these findings show that grid-search can replace manual parameter tuning with a more explicit and reproducible procedure while providing small improvements in sleep timing estimation and benefiting ensemble-based handling of within-sleep wakefulness.

---

## 论文详细总结（自动生成）

这是一份关于论文《A Grid-Search Framework for Dataset-Specific Calibration of Actigraphy Sleep Detection Algorithms》的深度结构化总结：

### 1. 核心问题与整体含义
*   **研究动机**：体动记录仪（Actigraphy）是睡眠监测的重要工具，但其核心算法（如 Cole-Kripke, Sadeh 等）高度依赖参数设置。目前研究者多采用默认参数或主观的人工调优（Manual Tuning），这导致不同研究间结果缺乏可重复性，且难以适应不同设备、人群和环境的差异。
*   **核心问题**：能否开发一种自动化的、无需生理金标准（如 PSG）标注的校准框架，以替代人工调优并提高算法的透明度与准确性？

### 2. 方法论
该论文提出了一种基于**网格搜索（Grid-Search）的共识优化框架**，核心思想是利用多个经典算法之间的“一致性”作为优化目标。
*   **算法流程**：
    1.  **候选参数过滤**：对 5 种经典算法（Cole-Kripke, Sadeh, Oakley, Crespo, MASDA）设定参数网格，过滤掉产生非生理性结果（如睡眠比例不在 10%-50% 范围内）的参数组合。
    2.  **多样性剪枝**：从有效配置中筛选出具有代表性的子集，以降低计算复杂度。
    3.  **共识优化**：计算不同算法输出的睡眠掩码之间的**平均成对 Jaccard 相似度**。目标是找到使各算法预测结果最趋于一致的参数组合。
    4.  **集成决策**：基于校准后的参数，生成“严格共识（所有算法均同意）”和“多数投票（超过半数同意）”两种集成模型。
*   **关键逻辑**：该框架假设当多种数学原理不同的算法在同一段数据上达成一致时，该结果最接近真实的生理行为模式。

### 3. 实验设计
*   **数据集**：
    1.  **PSG 验证数据集**：包含 23 名受试者的同步体动记录与多导睡眠图（PSG）数据，用于评估算法与生理金标准的一致性。
    2.  **双设备自测数据集**：一名受试者同时佩戴研究级设备（ActiLumus）和 Apple Watch（Series 10）持续 10 天，用于评估长期监测下的稳定性和碎片化分析。
*   **Benchmark 与对比方法**：
    *   以 **PSG 标注**为金标准。
    *   对比了**人工手动调优（Manual Tuning）**与**自动化网格搜索优化**的性能差异。
    *   评估指标包括：准确率、平衡准确率、F1-score、Cohen’s kappa、MCC 以及睡眠起止时间的偏差。

### 4. 资源与算力
*   论文**未明确说明**具体的硬件型号（如 GPU/CPU）或具体的训练时长。
*   由于该方法基于传统的规则算法（Rule-based algorithms）而非深度学习模型，其计算开销主要集中在网格搜索的遍历上。文中提到通过“随机采样参数空间”和“多样性剪枝”来确保计算的可行性，暗示其在普通个人电脑上即可运行。

### 5. 实验数量与充分性
*   **实验规模**：涵盖了 23 例 PSG 样本和 10 天的连续双设备监测。
*   **充分性评价**：
    *   **客观性**：通过与 PSG 金标准对比，客观量化了自动化校准的优劣。
    *   **公平性**：对比了人工调优和自动调优在同一数据集上的表现，证明了自动校准在减少“研究者自由度”方面的价值。
    *   **局限性**：样本量（23人）相对较小，且长期监测仅针对单一受试者，对于病理性睡眠（如失眠、呼吸暂停）的覆盖不足。

### 6. 主要结论与发现
*   **性能对等性**：自动化网格搜索校准产生的性能模式与经验丰富的人工调优相似，证明了其替代人工的可行性。
*   **精度提升**：在睡眠起止时间（Onset/Offset）预测上，自动校准比人工调优更接近 PSG 结果，且在处理类不平衡指标（如 MCC、Kappa）上表现更稳健。
*   **集成优势**：多数投票法能有效保留睡眠的连续性，而严格共识法虽然会增加碎片化，但能提供极高置信度的睡眠区间识别。
*   **本质限制**：实验再次确认了体动记录仪的局限性——算法收敛反映的是“行为静止”而非“电生理睡眠”，因此对睡眠中的静止觉醒识别依然困难。

### 7. 优点
*   **提高可重复性**：将主观的“视觉调整”转变为透明、可审计的数学优化过程。
*   **无需标签校准**：在缺乏 PSG 的真实研究场景中，提供了一种科学的参数选择依据。
*   **集成创新**：通过多算法共识降低了单一算法的系统性偏差。

### 8. 不足与局限
*   **共享偏差风险**：如果所有经典算法都对某种特定行为（如静止觉醒）存在共同误判，共识优化无法纠正这种系统性错误。
*   **人群泛化性**：生理约束（如 10%-50% 睡眠比例）是基于健康人群设定的，可能不适用于极短睡眠者或过度睡眠者。
*   **验证集单一**：双设备对比中使用的 Apple Watch 虽为参考，但其本身并非医学金标准，存在一定的参考偏差。

（完）
