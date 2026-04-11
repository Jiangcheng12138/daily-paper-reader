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
体动记录仪广泛用于长期睡眠监测，但既有的睡眠-觉醒评分算法通常需要参数调优，而调优过程通常由人工完成，这可能会降低研究的可重复性。本研究针对既有的体动记录仪算法提出了一种基于网格搜索的校准框架，并评估其是否可以作为人工调优的实用替代方案。该方法通过两个数据集进行了评估：一个经过多导睡眠图（PSG）验证的多受试者体动记录数据集，以及一个自行采集的双设备数据集。在经多导睡眠图验证的数据集中，网格搜索优化产生的性能模式与人工参数选择相似，同时略微改善了入睡和醒来时间的检测，并在觉醒敏感指标上取得了适度提升。在双设备数据集中，共识和多数投票法有助于减少主睡眠期内发生的短暂觉醒事件的影响，包括可能导致单个算法睡眠预测碎片化的微觉醒。总体而言，这些研究结果表明，网格搜索可以通过更明确且可重复的流程取代人工参数调优，同时在睡眠时间估算方面提供小幅改进，并有利于基于集成的方法处理睡眠期间的觉醒。

## Abstract
Actigraphy is widely used for long-term sleep monitoring, but established sleep-wake scoring algorithms often require parameter tuning, which is commonly performed manually and can reduce reproducibility. In this study, a grid-search-based calibration framework is presented for established actigraphy algorithms and evaluate whether it can serve as a practical alternative to manual tuning. The method was evaluated using two datasets: a multi-subject polysomnography-validated actigraphy dataset and a self-collected dual-device dataset. In the polysomnography-validated dataset, grid-search optimization produced performance patterns similar to manual parameter selection, while slightly improving detection of sleep onset and sleep offset and yielding modest gains in wake-sensitive metrics. In the dual-device dataset, consensus and majority voting were useful for reducing the influence of brief wake episodes occurring within the main sleep period, including micro-awakenings that can fragment sleep predictions across individual algorithms. Overall, these findings show that grid-search can replace manual parameter tuning with a more explicit and reproducible procedure while providing small improvements in sleep timing estimation and benefiting ensemble-based handling of within-sleep wakefulness.

---

## 论文详细总结（自动生成）

这是一份关于论文《A Grid-Search Framework for Dataset-Specific Calibration of Actigraphy Sleep Detection Algorithms》的深度结构化总结：

### 1. 核心问题与整体含义（研究动机和背景）
体动记录仪（Actigraphy）是临床和科研中长期监测睡眠的主流工具。然而，现有的经典睡眠检测算法（如 Cole-Kripke, Sadeh 等）高度依赖参数设置（如活动阈值、平滑窗口）。
*   **痛点**：最优参数随设备型号、佩戴位置及受试人群的不同而剧烈波动。目前研究者多依赖厂家默认设置或主观的“手动调参”，这导致研究结果缺乏透明度、难以复现，且容易引入人为偏差。
*   **核心目标**：开发一个自动化的、基于共识的校准框架，在缺乏生理金标准（如 PSG）的情况下，为特定数据集自动寻找最优参数，提高算法的稳健性和可重复性。

### 2. 方法论：核心思想与算法流程
该论文提出了一个**基于网格搜索（Grid-Search）的无监督校准框架**，其核心逻辑是：**如果多个原理不同的算法在某组参数下能达成最高的一致性，那么该结果最接近真实的生理行为模式。**

**算法流程分为四个阶段：**
1.  **网格搜索与初步过滤**：为 5 种经典算法（Cole-Kripke, Sadeh, Oakley, Crespo, MASDA）定义参数搜索空间。通过“生理合理性过滤器”剔除极端结果（例如预测睡眠比例不在 10%-50% 范围内的参数组合）。
2.  **多样性剪枝**：为了降低计算量，从通过过滤的配置中筛选出在睡眠比例分布上具有代表性的候选子集。
3.  **共识优化（核心步骤）**：计算不同算法预测结果之间的**平均成对 Jaccard 相似度**。目标是最大化算法间的一致性。若出现平局，则优先选择预测睡眠时长标准差最小、且均值更接近典型睡眠比例的组合。
4.  **集成决策**：利用校准后的参数生成两种集成掩码：
    *   **严格共识（Strict Consensus）**：所有算法均判定为睡眠才计为睡眠（高置信度）。
    *   **多数投票（Majority Vote）**：超过半数算法判定为睡眠（更具普适性）。

### 3. 实验设计
研究使用了两个具有代表性的数据集进行验证：
*   **数据集 1（PSG 验证集）**：包含 23 名受试者的同步体动数据与多导睡眠图（PSG）金标准。用于评估自动化校准与手动调参在生理准确性上的差异。
*   **数据集 2（双设备自测集）**：一名受试者同时佩戴研究级设备（ActiLumus）和 Apple Watch（作为外部参考），持续 10 天。用于评估算法在多日纵向监测中的表现及对碎片化睡眠的捕捉能力。
*   **Benchmark（对比基准）**：
    *   **手动调参（Manual Tuning）**：由研究者根据活动图视觉经验反复迭代调整出的参数。
    *   **PSG 标签**：作为 epoch 级别的分类金标准。
    *   **Apple Watch 睡眠阶段**：作为真实场景下的外部参考。

### 4. 资源与算力
论文**未明确说明**具体的硬件型号（如 GPU/CPU）或具体的计算时长。
*   由于该框架处理的是一维时间序列数据（体动计数），且经典算法计算复杂度较低，预计在普通商用 CPU 上即可完成网格搜索。
*   作者在文中提到了“随机采样”策略，以应对参数组合爆炸时的计算限制，这表明该方法在普通算力环境下具有可行性。

### 5. 实验数量与充分性
*   **实验规模**：涵盖了 23 例 PSG 样本和 10 天的连续双设备监测。
*   **充分性**：实验设计较为全面，不仅对比了分类准确率（Accuracy, F1），还重点分析了对类不平衡敏感的指标（MCC, Cohen’s κ）以及睡眠起止时间（Onset/Offset）的偏差。
*   **客观性**：通过与“手动调参”这一行业现状进行直接对比，客观证明了自动化方法在不损失准确性的前提下提升了可重复性。

### 6. 主要结论与发现
*   **性能对等性**：网格搜索自动校准的性能与经验丰富的人工调参相当，甚至在平衡准确率、特异性和 Cohen’s κ 等指标上略有胜出。
*   **时间估算更准**：自动化校准显著减少了入睡（Sleep Onset）和醒来（Sleep Offset）时间的估算误差，点位更贴近 PSG 识别的边界。
*   **集成优势**：多数投票法能有效减少因微觉醒导致的预测碎片化；而严格共识法能精准识别高置信度的睡眠区间。
*   **本质限制**：实验再次证实了体动记录仪的固有局限——它捕捉的是“行为静止”而非“电生理睡眠”，因此在区分“安静觉醒”和“睡眠”时仍存在挑战。

### 7. 优点与亮点
*   **提高可重复性**：将“黑箱式”的手动调参转变为透明、可审计、可重复的算法流程，解决了体动研究中的一大科研诚信隐患。
*   **无监督特性**：该框架不需要 PSG 标签即可运行，非常适合无法进行实验室监测的大规模居家研究。
*   **集成思路**：通过融合多种算法的优势，抵消了单一算法（如平滑类算法或阈值类算法）的系统性偏差。

### 8. 不足与局限
*   **共识偏差风险**：如果所有选入的经典算法都存在某种共同的系统性偏差（例如都无法识别静止觉醒），那么共识优化也无法纠正这一本质错误。
*   **生理约束的先验依赖**：框架依赖于预设的睡眠比例范围（如 10%-50%），对于患有严重睡眠障碍（如极度失眠或嗜睡症）的特殊人群，这些约束可能失效。
*   **样本多样性**：多日纵向分析仅基于单一受试者，其在不同病理人群（如帕金森、呼吸暂停患者）中的泛化能力尚需进一步验证。

（完）
