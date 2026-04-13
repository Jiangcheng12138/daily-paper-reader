---
title: A Grid-Search Framework for Dataset-Specific Calibration of Actigraphy Sleep Detection Algorithms
title_zh: 一种用于体动记录仪睡眠检测算法特定数据集校准的网格搜索框架
authors: "Rahjouei, A."
date: 2026-04-09
pdf: "https://www.biorxiv.org/content/10.64898/2026.04.07.706161v1.full.pdf"
tags: ["query:slp-ns"]
score: 9.0
evidence: 体动记录仪睡眠检测算法和睡眠-觉醒评分
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
体动记录仪广泛用于长期睡眠监测，但现有的睡眠-觉醒评分算法通常需要参数调优，而这种调优通常由人工完成，可能会降低研究的可重复性。本研究提出了一种针对现有体动记录仪算法的基于网格搜索的校准框架，并评估了其作为人工调优实用替代方案的可行性。该方法在两个数据集上进行了评估：一个经过多导睡眠图（PSG）验证的多受试者体动记录数据集，以及一个自行采集的双设备数据集。在多导睡眠图验证的数据集中，网格搜索优化产生的性能模式与人工参数选择相似，同时略微改善了入睡（sleep onset）和醒来（sleep offset）时间的检测，并在觉醒敏感指标上取得了适度提升。在双设备数据集中，共识和多数投票法有助于减少主睡眠期内发生的短暂觉醒事件的影响，包括可能导致单个算法睡眠预测碎片化的微觉醒。总体而言，这些研究结果表明，网格搜索可以通过更明确且可重复的流程取代人工参数调优，同时在睡眠时间估算方面提供小幅改进，并有助于基于集成的方法处理睡眠期间的觉醒。

## Abstract
Actigraphy is widely used for long-term sleep monitoring, but established sleep-wake scoring algorithms often require parameter tuning, which is commonly performed manually and can reduce reproducibility. In this study, a grid-search-based calibration framework is presented for established actigraphy algorithms and evaluate whether it can serve as a practical alternative to manual tuning. The method was evaluated using two datasets: a multi-subject polysomnography-validated actigraphy dataset and a self-collected dual-device dataset. In the polysomnography-validated dataset, grid-search optimization produced performance patterns similar to manual parameter selection, while slightly improving detection of sleep onset and sleep offset and yielding modest gains in wake-sensitive metrics. In the dual-device dataset, consensus and majority voting were useful for reducing the influence of brief wake episodes occurring within the main sleep period, including micro-awakenings that can fragment sleep predictions across individual algorithms. Overall, these findings show that grid-search can replace manual parameter tuning with a more explicit and reproducible procedure while providing small improvements in sleep timing estimation and benefiting ensemble-based handling of within-sleep wakefulness.

---

## 论文详细总结（自动生成）

这是一份关于论文《A Grid-Search Framework for Dataset-Specific Calibration of Actigraphy Sleep Detection Algorithms》的深度结构化总结：

### 1. 核心问题与研究背景
*   **核心问题**：体动记录仪（Actigraphy）是睡眠监测的重要工具，但其核心算法（如 Cole-Kripke, Sadeh 等）高度依赖参数设置。目前研究者多采用默认参数或主观的人工调优（Manual Tuning），这导致了研究结果的**不可重复性**和**跨设备/跨人群的性能不稳定性**。
*   **研究动机**：在缺乏多导睡眠图（PSG）金标准的情况下，如何通过一种客观、自动化且可重复的流程，为特定数据集找到最优的算法参数。

### 2. 方法论：网格搜索校准框架
该论文提出了一种**无监督的共识优化策略**，核心思想是：当多种不同的经典算法在某组参数下达成最高一致性时，该结果最能反映真实的睡眠模式。
*   **核心流程（四个阶段）**：
    1.  **网格搜索与过滤**：对 5 种经典算法（Cole-Kripke, Sadeh, Oakley, Crespo, MASDA）定义参数网格，生成大量候选掩码，并剔除睡眠比例不在生理合理范围（10%–50%）的配置。
    2.  **多样性剪枝**：为了降低计算量，在不同的睡眠比例区间内筛选出最具代表性的候选配置。
    3.  **共识优化**：计算不同算法组合间的**平均成对 Jaccard 相似度**。目标是最大化算法间的一致性，并以睡眠时长标准差作为平局决胜准则。
    4.  **集成决策**：基于校准后的参数生成两种集成掩码：**严格共识（Strict Consensus）**（所有算法均认为是睡眠）和**多数投票（Majority Vote）**（超过半数算法认为是睡眠）。

### 3. 实验设计
*   **数据集**：
    1.  **数据集 1 (PSG 验证集)**：包含 23 名受试者的同步体动记录与 PSG 金标准数据，用于定量评估准确性。
    2.  **数据集 2 (双设备自测集)**：单人连续 10 天同时佩戴研究级体动仪与 Apple Watch Series 10，用于评估长期监测的稳定性和碎片化分析。
*   **Benchmark（基准）**：
    1.  **人工调优（Manual Tuning）**：由研究者通过视觉观察活动信号手动调整出的参数。
    2.  **PSG 标注**：作为生理金标准。
    3.  **Apple Watch 睡眠分期**：作为现实场景下的外部参考。
*   **对比方法**：对比了 5 种独立算法在“人工调优”与“网格搜索优化”下的表现，以及两种集成方法的增益。

### 4. 资源与算力
*   论文**未明确说明**具体的硬件型号（如 GPU/CPU）或具体的训练时长。
*   由于该方法基于经典规则算法（Rule-based）而非深度学习，其计算压力主要来自于网格搜索的组合遍历。文中提到在组合数过多时采用了**随机采样（Random Sampling）**来保证计算可行性。

### 5. 实验数量与充分性
*   **实验规模**：涵盖了 23 例 PSG 样本和 10 天的连续监测数据。
*   **充分性评价**：
    *   **充分性**：实验对比了多种性能指标（Balanced Accuracy, Cohen’s κ, MCC 等），并详细分析了入睡/醒来时间的偏差（Bland-Altman 分析），实验设计较为全面。
    *   **客观性**：通过引入 PSG 金标准进行定量对比，证明了自动化校准不仅能达到人工水平，甚至在某些指标上略优。
    *   **局限性**：受试者样本量（N=23）相对较小，且多天连续监测仅针对单一受试者，泛化性验证尚有提升空间。

### 6. 主要结论与发现
*   **自动化可替代人工**：网格搜索优化产生的性能与经验丰富的人工调优高度一致，证明了该框架的实用性。
*   **性能提升**：优化后的参数在**睡眠起止时间（Sleep Onset/Offset）**的估算上比人工调优更精准，且在处理类别不平衡的指标（如 MCC）上表现更好。
*   **集成优势**：多数投票法能有效保持睡眠的连续性，而严格共识法则能更准确地识别睡眠中的短暂觉醒（Wake Bouts）。
*   **本质限制**：算法的一致性反映的是“行为静止”而非“电生理睡眠”，体动仪在区分“安静觉醒”和“真实睡眠”方面仍存在固有局限。

### 7. 优点与亮点
*   **提高可重复性**：将主观的“视觉调参”转化为透明、可审计的数学优化过程。
*   **无监督特性**：不需要 PSG 标签即可完成特定数据集的校准，非常适合大规模流行病学研究。
*   **集成视角**：不依赖单一算法，而是利用不同算法（阈值型 vs 平滑型）的互补性来提高鲁棒性。

### 8. 不足与局限
*   **共享偏差风险**：如果所有经典算法在特定场景下（如失眠患者）都存在系统性偏差，共识优化可能只是“错误的一致”。
*   **生理假设依赖**：框架依赖于预设的睡眠比例范围（10%-50%），对于极端睡眠障碍人群可能不适用。
*   **样本多样性**：缺乏对不同年龄段、不同睡眠疾病人群的广泛验证。
*   **应用限制**：虽然优化了参数，但无法突破加速度计无法监测脑电信号的物理极限。

（完）
