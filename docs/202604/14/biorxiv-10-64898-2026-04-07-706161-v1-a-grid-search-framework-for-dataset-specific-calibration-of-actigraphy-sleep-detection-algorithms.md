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
体动记录仪广泛用于长期睡眠监测，但现有的睡眠-觉醒评分算法通常需要参数调优，而这种调优通常由人工完成，可能会降低研究的可重复性。本研究提出了一种针对现有体动记录仪算法的基于网格搜索的校准框架，并评估了其作为人工调优实用替代方案的可行性。该方法在两个数据集上进行了评估：一个经过多导睡眠图（PSG）验证的多受试者体动记录数据集，以及一个自行采集的双设备数据集。在多导睡眠图验证的数据集中，网格搜索优化产生的性能模式与人工参数选择相似，同时略微改善了入睡（sleep onset）和醒来（sleep offset）时间的检测，并在觉醒敏感指标上取得了适度提升。在双设备数据集中，共识和多数投票法有助于减少主睡眠期内发生的短暂觉醒事件的影响，包括可能导致单个算法睡眠预测碎片化的微觉醒。总体而言，这些研究结果表明，网格搜索可以通过更明确且可重复的流程取代人工参数调优，同时在睡眠时间估算方面提供小幅改进，并有助于通过集成方法处理睡眠期间的觉醒。

## Abstract
Actigraphy is widely used for long-term sleep monitoring, but established sleep-wake scoring algorithms often require parameter tuning, which is commonly performed manually and can reduce reproducibility. In this study, a grid-search-based calibration framework is presented for established actigraphy algorithms and evaluate whether it can serve as a practical alternative to manual tuning. The method was evaluated using two datasets: a multi-subject polysomnography-validated actigraphy dataset and a self-collected dual-device dataset. In the polysomnography-validated dataset, grid-search optimization produced performance patterns similar to manual parameter selection, while slightly improving detection of sleep onset and sleep offset and yielding modest gains in wake-sensitive metrics. In the dual-device dataset, consensus and majority voting were useful for reducing the influence of brief wake episodes occurring within the main sleep period, including micro-awakenings that can fragment sleep predictions across individual algorithms. Overall, these findings show that grid-search can replace manual parameter tuning with a more explicit and reproducible procedure while providing small improvements in sleep timing estimation and benefiting ensemble-based handling of within-sleep wakefulness.

---

## 论文详细总结（自动生成）

这是一份关于论文《A Grid-Search Framework for Dataset-Specific Calibration of Actigraphy Sleep Detection Algorithms》的深度结构化总结：

### 1. 核心问题与整体含义（研究动机和背景）
*   **核心问题**：体动记录仪（Actigraphy）是睡眠监测的重要工具，但其核心算法（如 Cole-Kripke, Sadeh 等）高度依赖参数设置。目前研究者多采用设备默认参数或主观的人工调参，这导致了研究结果的**低可重复性**和**跨设备/跨人群的不一致性**。
*   **研究背景**：不同设备灵敏度、佩戴位置及个体活动差异使得单一固定参数难以通用。论文旨在提出一种自动化的校准框架，在缺乏生理金标准（如 PSG）的情况下，实现算法参数的客观优化。

### 2. 核心思想与方法论
该论文提出了一个**基于共识的无监督网格搜索校准框架**，其核心逻辑是：如果多个经典算法在某组参数下对同一段数据的预测达成高度一致，那么该预测结果极大概率反映了真实的睡眠行为模式。

*   **算法流程（四个阶段）**：
    1.  **网格搜索与过滤**：对五种经典算法（Cole-Kripke, Sadeh, Oakley, Crespo, MASDA）定义参数网格，生成大量候选掩码，并剔除睡眠比例不在生理合理范围（10%–50%）内的配置。
    2.  **多样性剪枝**：在保留生理合理性的基础上，选取具有代表性的候选配置以降低后续计算量。
    3.  **共识优化**：通过计算**平均成对 Jaccard 相似度**，寻找使不同算法之间达成最大共识的参数组合。若出现平局，则以睡眠时长标准差最小化作为破缺准则。
    4.  **集成决策**：基于校准后的参数生成“严格共识（100%一致）”和“多数投票（>50%一致）”两种集成掩码。

### 3. 实验设计
*   **数据集**：
    1.  **数据集 1 (PSG 验证集)**：包含 23 名受试者的同步体动记录与多导睡眠图（PSG）数据，用于评估算法与生理金标准的一致性。
    2.  **数据集 2 (双设备自测集)**：单人连续 10 天同时佩戴研究级体动仪与 Apple Watch Series 10，用于评估长期监测下的稳定性和碎片化分析。
*   **Benchmark 与对比方法**：
    *   **基准**：PSG 标注（数据集 1）和 Apple Watch 睡眠分期（数据集 2）。
    *   **对比**：将自动化网格搜索校准的效果与经验丰富的人工手动调参（Manual Tuning）进行直接对比。

### 4. 资源与算力
*   论文**未明确说明**具体的硬件型号（如 GPU/CPU）或具体的训练/搜索时长。
*   由于该框架基于经典规则算法（非深度学习），其计算开销主要集中在网格搜索的组合遍历上。文中提到通过“随机采样”和“多样性剪枝”来确保计算可行性，暗示其在普通商用电脑上即可运行。

### 5. 实验数量与充分性
*   **实验规模**：涵盖了 23 例 PSG 样本和 10 天的连续双设备监测。
*   **充分性评价**：
    *   **客观性**：通过与人工调参的对比，证明了自动化方法在不损失性能的前提下提高了可重复性。
    *   **全面性**：不仅评估了常规的分类指标（准确率、F1、MCC），还深入分析了睡眠起止时间（Onset/Offset）的偏差以及对微觉醒（Wake Bouts）的检测率。
    *   **局限性**：样本量（23人）相对较小，且多天连续监测仅针对单一受试者，其在病理人群（如失眠症患者）中的泛化性尚待验证。

### 6. 主要结论与发现
*   **性能对等**：网格搜索自动校准产生的性能模式与人工调参高度相似，证明了其替代人工的可行性。
*   **精度提升**：在睡眠起止时间估算上，自动校准比人工调参更接近 PSG 参考值，且在觉醒敏感性指标（如特异性、MCC）上有小幅改进。
*   **集成优势**：多数投票法能有效保持睡眠连续性，而严格共识法在识别高置信度睡眠区间和微觉醒方面表现更佳。
*   **本质限制**：实验再次确认了体动仪的局限性——算法收敛反映的是“行为静止”而非“电生理睡眠”，因此对睡眠中的静止觉醒识别依然困难。

### 7. 优点与亮点
*   **提高可重复性**：将“黑箱式”的人工视觉判断转化为透明、可审计的数学优化过程。
*   **无监督校准**：在没有 PSG 金标准的大规模临床/居家研究中，提供了一种科学的参数确定方法。
*   **集成视角**：通过融合多种算法，抵消了单一算法的系统性偏差（如某些算法过度平滑，某些过度敏感）。

### 8. 不足与局限
*   **共识偏差风险**：如果所有经典算法都存在某种共同的系统性偏差（如都无法识别静止觉醒），那么共识优化可能会强化这种偏差。
*   **生理假设依赖**：框架依赖于预设的睡眠比例范围（10%-50%），对于极短睡眠或极长睡眠的特殊人群可能失效。
*   **人群覆盖有限**：实验主要针对健康受试者，未涵盖睡眠结构严重紊乱的临床患者。

（完）
