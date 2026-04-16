---
title: A Grid-Search Framework for Dataset-Specific Calibration of Actigraphy Sleep Detection Algorithms
title_zh: 一种用于体动记录仪睡眠检测算法特定数据集校准的网格搜索框架
authors: "Rahjouei, A."
date: 2026-04-09
pdf: "https://www.biorxiv.org/content/10.64898/2026.04.07.706161v1.full.pdf"
tags: ["query:slp-ns"]
score: 9.0
evidence: 体动记录仪睡眠检测算法的校准
tldr: 针对体动记录仪睡眠检测算法中手动调参导致的可重复性低问题，本研究提出了一种基于网格搜索的自动校准框架。通过在PSG验证数据集和双设备数据集上的评估，该框架不仅能替代手动调参，提高实验的可重复性，还在睡眠起止时间预测和觉醒敏感性指标上实现了小幅性能提升，并能通过集成投票机制有效处理睡眠中的微小觉醒干扰。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-04-07-706161-v1/fig-001.webp\", \"caption\": \"Figure 5. Detection of wake bouts occurring within sleep across actigraphy 513 algorithms. 514 (A) Wake-bout detection rate by reference bout duration. Wake bouts were defined from 515 the reference sleep–wake signal as contiguous runs of wake occurring within sleep (i.e., 516 flanked by sleep on both sides). A bout was considered detected when an algorithm 517 classified ≥50% of epochs within the bout as wake. Detection rates are shown for 518 duration bins (1–2 min, 3–5 min, 6–10 min, 11–20 min, >60 min). Sample sizes for each 519 bin are indicated below the x-axis labels. Colors represent algorithms: Cole–Kripke, 520 Sadeh, Oakley, Crespo, MASDA, Consensus, and Majority. The dashed horizontal line 521 indicates the 50% detection threshold. 522 (B) Overall wake-bout detection rate across all durations. Values represent the 523 percentage of reference wake bouts correctly detected by each algorithm. 524 (C) Mean fraction of wake epochs detected within each bout, averaged by duration bin. 525 This metric reflects how much of each wake bout is identified as wake by the algorithm, 526 independent of the binary detection threshold. 527 528 529\", \"page\": 26, \"index\": 1, \"width\": 977, \"height\": 640}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-04-07-706161-v1/fig-002.webp\", \"caption\": \"Figure 1. Hyperparameter tuning and consensus optimization workflow for actigraphy-301 based sleep detection algorithms. The process is divided into four distinct phases: 302 (Phase 1) Grid Search & Filtering, where parameter grids are defined for five algorithms 303 (Cole-Kripke, Sadeh, Oakley, Crespo, MASDA) and results are filtered to retain only 304 biologically plausible sleep percentages (10–50%); (Phase 2) Pruning for Diversity, 305 which reduces the computational load by selecting the top 𝐾 (e.g., 40) configurations 306\", \"page\": 15, \"index\": 2, \"width\": 977, \"height\": 683}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-04-07-706161-v1/fig-003.webp\", \"caption\": \"Figure 4. Comparison of sleep timing estimates between algorithms and PSG 454 using manual and grid-search parameter configurations. 455\", \"page\": 23, \"index\": 3, \"width\": 977, \"height\": 1241}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-04-07-706161-v1/fig-004.webp\", \"caption\": \"Figure 3. Performance of actigraphy-based sleep–wake algorithms compared with 381 polysomnography (PSG) across 23 subjects. 382 (A) Pooled confusion matrices showing epoch-level classification relative to PSG for 383 each algorithm. 384 (B) Mean performance metrics across subjects (±SD), including Accuracy, Balanced 385 Accuracy, Precision, Recall (Sensitivity), Specificity, Cohen’s κ, F1-score, and Matthews 386 Correlation Coefficient (MCC). 387 (C) Boxplots showing per-subject distributions of performance metrics across the cohort 388 (N = 23). Red dashed lines indicate commonly used reference thresholds for agreement 389 (e.g., κ = 0.6). 390 (D) Heatmap of pairwise Cohen’s κ values showing agreement between algorithms and 391 PSG. 392 393\", \"page\": 19, \"index\": 4, \"width\": 977, \"height\": 608}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-04-07-706161-v1/fig-005.webp\", \"caption\": \"Figure 2. Performance of sleep–wake algorithms using manually selected parameter 337 settings across 23 subjects. 338 (A) Mean per-subject confusion matrices (±SD) relative to the PSG reference. Values 339 represent the percentage of epochs classified as wake or sleep averaged across 340 subjects. Across algorithms, sleep epochs were identified with high sensitivity, whereas 341 wake epochs were more frequently misclassified as sleep. 342 (B) Mean performance metrics (±SD) across subjects, including Accuracy, Balanced 343 Accuracy, Precision, Recall (Sensitivity), Specificity, F1-score, Cohen’s κ, and Matthews 344 Correlation Coefficient (MCC). The red dashed lines indicate reference thresholds for 345 comparison across metrics. 346 (C) Boxplots showing the distribution of performance metrics across subjects (N = 23). 347 While accuracy and F1-score remain consistently high across algorithms, greater 348 variability is observed in specificity and agreement-based metrics such as Cohen’s κ and 349 MCC. 350\", \"page\": 17, \"index\": 5, \"width\": 977, \"height\": 667}]"
motivation: 传统的体动记录仪睡眠评分算法依赖手动调参，过程繁琐且缺乏可重复性，限制了算法在不同数据集上的应用。
method: 提出一种基于网格搜索的自动化校准框架，用于优化现有算法参数，并结合共识与多数投票机制来减少睡眠期间短暂觉醒的影响。
result: 实验表明网格搜索在睡眠起止检测上优于手动调参，且能产生更稳健的觉醒敏感性指标，有效降低了睡眠预测的分碎化。
conclusion: 该框架为体动记录仪算法提供了一种透明、可重复且高效的校准方案，是替代手动调参并提升睡眠监测准确性的实用工具。
---

## 摘要
体动记录仪广泛用于长期睡眠监测，但现有的睡眠-觉醒评分算法通常需要参数调优，而这种调优通常由人工完成，可能会降低研究的可重复性。本研究提出了一种针对现有体动记录仪算法的基于网格搜索的校准框架，并评估了其作为人工调优实用替代方案的可行性。该方法在两个数据集上进行了评估：一个经过多导睡眠图（PSG）验证的多受试者体动记录数据集，以及一个自行采集的双设备数据集。在多导睡眠图验证的数据集中，网格搜索优化产生的性能模式与人工参数选择相似，同时略微改善了入睡（sleep onset）和醒来（sleep offset）时间的检测，并在觉醒敏感指标上取得了适度提升。在双设备数据集中，共识和多数投票法有助于减少主睡眠期内发生的短暂觉醒事件的影响，包括可能导致单个算法睡眠预测碎片化的微觉醒。总体而言，这些研究结果表明，网格搜索可以通过更明确且可重复的流程取代人工参数调优，同时在睡眠时间估算方面提供小幅改进，并有助于通过集成方法处理睡眠期间的觉醒。

## Abstract
Actigraphy is widely used for long-term sleep monitoring, but established sleep-wake scoring algorithms often require parameter tuning, which is commonly performed manually and can reduce reproducibility. In this study, a grid-search-based calibration framework is presented for established actigraphy algorithms and evaluate whether it can serve as a practical alternative to manual tuning. The method was evaluated using two datasets: a multi-subject polysomnography-validated actigraphy dataset and a self-collected dual-device dataset. In the polysomnography-validated dataset, grid-search optimization produced performance patterns similar to manual parameter selection, while slightly improving detection of sleep onset and sleep offset and yielding modest gains in wake-sensitive metrics. In the dual-device dataset, consensus and majority voting were useful for reducing the influence of brief wake episodes occurring within the main sleep period, including micro-awakenings that can fragment sleep predictions across individual algorithms. Overall, these findings show that grid-search can replace manual parameter tuning with a more explicit and reproducible procedure while providing small improvements in sleep timing estimation and benefiting ensemble-based handling of within-sleep wakefulness.

---

## 论文详细总结（自动生成）

这是一份关于论文《A Grid-Search Framework for Dataset-Specific Calibration of Actigraphy Sleep Detection Algorithms》的深度结构化总结：

### 1. 核心问题与整体含义（研究动机和背景）
*   **核心问题**：体动记录仪（Actigraphy）是睡眠监测的重要工具，但其核心算法（如 Cole-Kripke, Sadeh 等）高度依赖参数设置。目前研究者多采用默认参数或主观的手动调参，这导致了研究结果的**低可重复性**和**跨设备/跨人群的性能不稳定**。
*   **研究背景**：不同设备灵敏度、佩戴位置及个体活动模式的差异，使得一套固定参数难以通用。论文旨在提出一个自动化的校准框架，在缺乏金标准（如 PSG）的情况下，实现算法参数的客观优化。

### 2. 提出的方法论
该论文提出了一个基于**网格搜索（Grid-Search）**和**多算法共识（Consensus）**的无监督校准框架，主要包含四个阶段：
*   **候选参数过滤（Phase 1）**：针对五种经典算法（Cole-Kripke, Sadeh, Oakley, Crespo, MASDA）定义参数网格，并应用“生理合理性过滤器”，仅保留预测睡眠比例在 10%–50% 之间的参数组合。
*   **多样性剪枝（Phase 2）**：为了降低计算量，从通过过滤的配置中筛选出在睡眠比例分布上具有代表性的子集。
*   **共识优化（Phase 3）**：这是核心步骤。框架假设：当多种原理不同的算法在同一段数据上达成最高一致性时，该结果最接近真实行为模式。通过最大化**平均成对 Jaccard 相似度**来选择最优参数组合。
*   **集成决策（Phase 4）**：利用校准后的参数生成两种集成掩码：
    *   **严格共识（Strict Consensus）**：所有算法均判定为睡眠才计为睡眠（高置信度）。
    *   **多数投票（Majority Vote）**：超过半数算法判定为睡眠（更稳健）。

### 3. 实验设计
*   **数据集**：
    1.  **PSG 验证数据集**：包含 23 名受试者的同步体动记录与多导睡眠图（PSG）数据，用于评估算法与生理金标准的一致性。
    2.  **双设备自测数据集**：一名受试者同时佩戴研究级设备（ActiLumus）和 Apple Watch（Series 10）持续 10 天，用于评估长期监测下的表现。
*   **Benchmark（基准）**：
    *   **手动调参（Manual Tuning）**：模拟研究人员通过视觉观察活动图手动调整参数的传统做法。
    *   **PSG 标签**：作为 epoch 级别的分类金标准。
    *   **Apple Watch 睡眠阶段**：作为长期监测的外部参考。
*   **对比指标**：准确率、平衡准确率、Cohen’s Kappa (κ)、Matthews 相关系数 (MCC)、入睡/醒来时间误差等。

### 4. 资源与算力
*   论文**未明确说明**具体的硬件型号（如 GPU/CPU）或具体的训练时长。
*   由于该方法基于网格搜索和规则算法（非深度学习），其计算开销主要集中在参数组合的遍历上。文中提到通过“随机采样”和“多样性剪枝”来控制计算复杂度，暗示该框架可以在普通个人电脑或工作站上运行。

### 5. 实验数量与充分性
*   **实验规模**：涵盖了 23 例 PSG 验证样本和 10 天的连续双设备监测。
*   **充分性评价**：
    *   **对比充分**：对比了手动调参和自动校准，并评估了五种不同的经典算法及其集成效果。
    *   **指标全面**：不仅关注整体准确率，还重点分析了对类别不平衡敏感的 MCC 和 Kappa 指标，以及睡眠起止时间的精确度。
    *   **客观性**：通过 PSG 金标准验证了自动校准的有效性，证明了其不仅能替代人工，甚至在某些指标上更优。

### 6. 主要结论与发现
*   **自动化可行性**：网格搜索框架产生的性能模式与经验丰富的人工调参高度相似，证明了自动化校准可以取代主观的手动过程。
*   **性能提升**：自动校准在**睡眠起止时间（Sleep Onset/Offset）**的估算上比手动调参更精确，且在识别觉醒（Wake）的敏感性指标上略有改善。
*   **集成优势**：多数投票法能有效减少睡眠期间因微小活动导致的预测碎片化；严格共识法则能提供极高置信度的睡眠区间。
*   **本质限制**：尽管校准优化了参数，但体动记录仪本质上测量的是“行为静止”而非“电生理睡眠”，因此在区分“安静觉醒”和“睡眠”方面仍存在固有局限。

### 7. 优点与亮点
*   **提高可重复性**：将“黑箱”式的手动调参转化为透明、可审计、可重复的算法流程。
*   **无监督特性**：不需要 PSG 标签即可在新的数据集上完成校准，非常适合大规模、长期的居家睡眠研究。
*   **集成创新**：通过多算法共识来对冲单一算法的偏差，增强了系统的鲁棒性。

### 8. 不足与局限
*   **共享偏差风险**：如果所有参与共识的算法都存在某种系统性偏差（如都无法识别静止觉醒），共识机制也无法纠正这一错误。
*   **先验假设依赖**：框架依赖于预设的“生理合理范围”（如睡眠比例 10%-50%），这对于患有严重睡眠障碍（如极度失眠或嗜睡）的人群可能不适用。
*   **样本多样性**：多日连续监测仅基于单一受试者，其在不同病理人群（如失眠症、呼吸暂停患者）中的泛化能力仍需进一步验证。

（完）
