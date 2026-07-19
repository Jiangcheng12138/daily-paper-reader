---
title: Automated sleep scoring in hibernating and non-hibernating American black bears
title_zh: 冬眠与非冬眠美洲黑熊的自动睡眠评分
authors: "Toien, O., Pittaras, E. C., Huang, Y.-G., Brodersen, P. J. N., Allocca, G., Barnes, B. M., Heller, H. C."
date: 2026-07-14
pdf: "https://www.biorxiv.org/content/10.1101/2025.03.31.646262v4.full.pdf"
tags: ["query:tr-hb"]
score: 9.0
evidence: 对冬眠和非冬眠美洲黑熊进行自动睡眠评分，涉及代谢抑制、体温调节和睡眠
tldr: "冬眠熊代谢抑制幅度高达75%，但体温降幅温和，其睡眠在代谢抑制中的作用尚不明确。本研究对16只美洲黑熊在冬眠与非冬眠状态下采集的3500天脑电图数据进行自动睡眠评分，测试了Somnotate和Somnivore两种机器学习分类器。结果发现，两种方法在冬眠期表现优秀，F-measure达0.90-0.98，冬眠期睡眠时长约为夏季的2倍，且自动评分与人工评分无显著差异。本研究首次将自动评分应用于冬眠物种，验证了其接近人工的准确度，为大规模睡眠分析提供了可靠工具。"
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-03-31-646262-v4/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1658, \"height\": 410, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-03-31-646262-v4/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1616, \"height\": 460, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-03-31-646262-v4/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1283, \"height\": 783, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-03-31-646262-v4/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1282, \"height\": 783, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-03-31-646262-v4/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1394, \"height\": 842, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-03-31-646262-v4/fig-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 1316, \"height\": 948, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-03-31-646262-v4/fig-007.webp\", \"caption\": \"\", \"page\": 0, \"index\": 7, \"width\": 1366, \"height\": 725, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-03-31-646262-v4/fig-008.webp\", \"caption\": \"\", \"page\": 0, \"index\": 8, \"width\": 1364, \"height\": 728, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-03-31-646262-v4/fig-009.webp\", \"caption\": \"\", \"page\": 0, \"index\": 9, \"width\": 1398, \"height\": 499, \"label\": \"Figure\"}]"
tables_json: "[{\"url\": \"assets/tables/biorxiv/biorxiv-10-1101-2025-03-31-646262-v4/table-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1489, \"height\": 171, \"label\": \"Table\"}]"
motivation: 为了大规模分析冬眠熊的脑电图数据，自动评估睡眠在代谢抑制中的作用。
method: 采用Somnotate和Somnivore两种机器学习分类器，分别训练于冬眠和非冬眠数据，并评估体温波动对检测效果的影响。
result: 两种分类器F-measure为0.90-0.98，冬眠期睡眠时长约夏季2倍，自动与手动评分无显著差异（夏季轻微高估）。
conclusion: 自动睡眠评分在高质量数据训练下可达到接近人工评分的准确度，适用于冬眠物种的睡眠研究。
---

## 摘要
冬眠的熊表现出显著的代谢抑制。它们的核心体温（Tb）下降幅度适中（从38°C降至30-35°C），但代谢率下降高达75%。为理解睡眠在这种低代谢状态中的作用，我们通过生物遥测技术记录了16只圈养美洲黑熊在冬眠期和非冬眠期、半自然条件下的脑电图（EEG）、眼电图（EOG）和肌电图（EMG）数据，历时超过3500天。这一数据集过于庞大，无法手动对清醒、快速眼动睡眠和非快速眼动睡眠进行评分，因此我们测试了两种机器学习分类器：（1）基于多个单日录音训练的Somnotate，以及（2）基于每个录音中的小样本子集训练的Somnivore。由于此前从未对冬眠物种应用自动评分方法，一个主要关切是脑温变化对EEG以及基于机器学习的检测的影响。为此，我们使用来自6只熊的3位手动睡眠评分者的共识选择了参考数据，包括冬眠期间Tb以多日周期波动时最高和最低体温的两个单日录音，以及夏季非冬眠的一个单日录音。当分别针对冬眠和非冬眠数据训练时，Somnotate的结果非常出色。在冬眠期内分别针对高和低Tb训练Somnotate并未进一步改善结果。对于自动评分和手动评分，冬眠期的睡眠时间大约是夏季的两倍（p<0.0001）。在冬眠期，自动评分与手动评分之间的警觉状态占比无显著差异（p>0.05），但在夏季睡眠时间上略有高估（p<0.05）。两种应用相对于手动评分得到的F值均在0.90-0.98范围内。两个应用之间的异常值（0.67-0.88范围）具有相关性，表明特定文件更具标注挑战性。我们得出结论，当基于高质量数据训练时，两种应用的准确度接近手动评分者。

## Abstract
Hibernating bears show remarkable metabolic suppression. Their decline in core body temperature (Tb) is moderate (from 38{degrees}C to 30-35{degrees}C), but their metabolism declines as much as 75%. To understand the role of sleep in this hypometabolic state, we recorded biotelemetrically EEG, EOG and EMG data over 3500 days from 16 captive American black bears in and out of hibernation under semi-natural conditions. This data set is too large to score manually for Wake, REM- and NREM sleep, so we tested two machine learning classifiers: (1) Somnotate trained on multiple one-day recordings, and (2) Somnivore, trained on a small subset from each recording. As automated scoring methods have not been applied to hibernating species before, a major concern is the effect changing brain temperature has on the EEG and on the machine learning based detection. Therefore, we selected reference data using consensus by 3 manual sleep scorers from each of 6 bears, two one-day recordings at the highest and lowest body temperatures during hibernation when Tb was oscillating in multiday cycles, and a non-hibernating one-day recording in summer. Somnotate results were excellent when trained separately for hibernating and non-hibernating data. Training Somnotate separately for high and low Tb within hibernation did not improve results further. Sleep times in hibernation were about 2x that in summer for both automated scores and manual scores (p<0.0001). There were no significant differences in occupancy of vigilance states between automated and manual scores in hibernation (p>0.05), but a small overestimate of sleep time in summer (p<0.05). Both applications yielded F-measures against manual scores in the 0.90-0.98 range. Outliers in the 0.67-0.88 range were correlated between the two applications, indicating that specific files are more challenging to annotate. We conclude that both applications have accuracies approaching that of manual scorers when trained on high quality data.

---

## 论文详细总结（自动生成）

## 1. 论文的核心问题与整体含义

- **研究动机**：冬眠熊的代谢率下降高达75%，但核心体温仅温和下降（30-35°C），睡眠在这一低代谢状态中的作用尚不清楚。为大规模分析熊的脑电图（EEG）数据，需要自动睡眠评分方法。
- **研究背景**：之前没有对冬眠物种应用自动睡眠评分，且脑温变化可能影响EEG信号频率分布，进而干扰机器学习检测的准确性。本研究首次验证了两种机器学习分类器（Somnotate和Somnivore）在冬眠与非冬眠美洲黑熊数据上的有效性。

## 2. 方法论

- **核心思想**：利用机器学习自动将EEG、EOG、EMG信号分类为Wake、NREM、REM三种警觉状态，以处理超过3500天的庞大数据集。
- **关键技术细节**：
  - **数据预处理**：EEG/EOG/EMG信号经过模拟滤波（0.1-150Hz）和数字滤波（如0.5Hz高通）。epoch长度为10秒。
  - **Somnotate**：基于线性判别分析（LDA）与隐马尔可夫模型（HMM）的概率分类器，可跨多个文件训练。训练时使用EEG+EOG通道，采样间隔10秒。支持holdout模式（排除待测文件）评估鲁棒性。
  - **Somnivore**：专有辅助机器学习，在每个待测文件中随机选取100个epoch的NREM、REM、Wake作为训练数据（仅EEG+EOG），并设置最小3个epoch的评分一致性规则，禁止强制转换规则以允许Wake→REM转换。
- **算法流程**（文字说明）：
  1. 从原始EDF文件中提取10秒epoch的EEG/EOG数据。
  2. 提取频谱特征（如功率谱密度），通过卷积或特征提取获得频率分布。
  3. 使用训练好的分类器（Somnotate: LDA+HMM；Somnivore: 专有模型）对每个epoch进行概率预测，输出NREM/REM/Wake。
  4. 应用后处理规则（如最小一致性epoch数）平滑结果。

## 3. 实验设计

- **数据集**：
  - 来自16只圈养美洲黑熊，选择其中6只熊的3个24小时录音：冬眠期高峰Tb（34.9±0.5°C）、低谷Tb（32.1±0.7°C）、夏季非冬眠（38.1±0.4°C）。
  - 手动参考评分由3名独立评分者通过投票产生共识（共154,919个epoch，共识率99.5%）。
- **Benchmark**：手动共识评分作为金标准。
- **对比方法**：Somnotate vs Somnivore，并测试不同训练策略（训练通道、训练数据源、是否holdout、是否区分高/低Tb）。

## 4. 资源与算力

- **文中未明确说明使用的GPU型号、数量、训练时长等算力信息**。所有训练和测试均在CPU上完成？未提及具体硬件资源。

## 5. 实验数量与充分性

- **主要实验组**：
  1. 不同训练通道对Somnivore准确率的影响（图3，仅EEG vs EEG+EOG）。
  2. 不同训练数据源对Somnivore的影响（图4，同文件、同动物不同Tb、跨动物）。
  3. Somnotate在不同训练数据集和holdout模式下的准确率（图5，全部数据、仅冬眠、冬眠内分离/低Tb、仅夏季）。
  4. 各警觉状态的F-measure（图7，NREM、REM、Wake）。
  5. 睡眠状态分布（图8，冬眠 vs 夏季）。
  6. 异常值相关性分析（图9）。
- **充分性评价**：实验设计系统，覆盖了训练数据源、通道选择、体温波动、holdout验证等多个维度，对比公平（两种方法均在同一参考数据集上评估）。但样本量较小（6只熊），且夏季记录存在更多伪迹和信号中断，可能引入偏差。

## 6. 主要结论与发现

1. **准确性**：两种自动评分方法的F-measure大多在0.90-0.98，接近手动评分者（手动评分者共识一致率94.5%）。低温（冬眠）数据表现与高温数据相当，单独训练高/低Tb并未改善结果。
2. **睡眠时间差异**：冬眠期总睡眠时间约为夏季的2.05倍（NREM 1.95x, REM 2.26x），自动评分与手动评分无显著差异（冬眠期p>0.05；夏季有轻微高估，p<0.05）。
3. **体温影响**：脑温变化（30-35°C）对自动评分影响很小，训练模型可跨冬眠期内不同体温阶段通用。
4. **异常文件**：两个应用的低F-measure异常值高度相关（R²=0.57-0.78），表明某些文件本身难以标注，可能是手动或自动评分共同的挑战。

## 7. 优点

- **首次验证自动睡眠评分在冬眠物种上的可行性**，为大规模分析冬眠熊睡眠结构提供了可靠工具。
- **使用三位评分者的共识作为金标准**，降低了主观偏差。
- 测试了多种训练策略（通道选择、数据源、体温条件），系统评估了鲁棒性和泛化能力。
- 两种不同设计的方法（跨文件概率模型 vs 单文件辅助学习）均获得一致优秀结果，增强了结论的可信度。
- 公开了部分数据和代码（Somnotate开源，共识提取代码开源），促进可重复性。

## 8. 不足与局限

- **样本量有限**：仅6只熊的18天录音（冬眠12天+夏季6天），可能无法代表全部个体差异或冬眠全季节变化。
- **夏季数据质量较差**：存在更多伪迹、信号中断，导致自动评分对睡眠时间有轻微高估，可能限制夏季分析的准确性。
- **无法排除某些文件对自动和手动评分均困难**：低F-measure文件可能同时存在手动共识质量低的问题。
- **两种方法训练方式不同**：Somnotate可跨文件训练，Somnivore依赖同文件训练，直接比较F-measure时需谨慎。
- **未探索冬眠期内多日体温周期对睡眠模式的长期动态影响**，仅用了两个时间点（高峰与低谷）。
- **Somnivore为专有代码**，复现受限；Somnotate虽开源但需特定修改。
- **未进行消融实验**（如移除特定特征或通道），也未与其他深度学习模型（如CNN/RNN）对比。

（完）
