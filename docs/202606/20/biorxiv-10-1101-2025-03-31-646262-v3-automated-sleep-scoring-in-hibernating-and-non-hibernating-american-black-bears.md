---
title: Automated sleep scoring in hibernating and non-hibernating American black bears
title_zh: 冬眠与非冬眠美洲黑熊的自动睡眠评分
authors: "Toien, O., Pittaras, E. C., Huang, Y.-G., Brodersen, P. J. N., Allocca, G., Barnes, B. M., Heller, H. C."
date: 2026-06-19
pdf: "https://www.biorxiv.org/content/10.1101/2025.03.31.646262v3.full.pdf"
tags: ["query:tr-hb"]
score: 9.0
evidence: 冬眠熊代谢抑制与睡眠评分
tldr: 黑熊冬眠时代谢大幅抑制，体温适中但睡眠时长增加。研究利用EEG/EOG/EMG数据，首次对冬眠物种应用自动睡眠评分。比较两种机器学习方法（Somnotate和Somnivore），分别或联合训练，与人工评分一致性高，F-measure达0.90-0.98。结果表明自动评分可替代人工，但夏季睡眠时间略有高估。
source: biorxiv
selection_source: fresh_fetch
motivation: 冬眠熊的代谢抑制与睡眠的关系未知，且大量生物遥测数据无法手动评分，需测试自动评分方法。
method: 使用Somnotate（多日记录训练）和Somnivore（单次录音子集训练）对黑熊冬眠和非冬眠期的EEG/EOG/EMG进行自动睡眠分期。
result: 两种自动评分与人工评分一致性高（F-measure 0.90-0.98），冬眠期睡眠时长约为夏季两倍，仅夏季睡眠时间略有高估。
conclusion: 自动评分方法在冬眠物种中准确度接近人工，可有效处理大规模数据，但需注意温度变化对EEG的影响。
---

## 摘要
冬眠的熊表现出显著的代谢抑制。它们的核心体温（Tb）下降幅度适中（从38°C降至30-35°C），但代谢下降高达75%。为了解睡眠在这种低代谢状态中的作用，我们在半自然条件下记录了16只圈养美洲黑熊在冬眠期和非冬眠期的生物遥测脑电图、眼电图和肌电图数据，时间跨度超过3500天。这个数据集太大，无法手动评分出清醒、快速眼动睡眠和非快速眼动睡眠，因此我们测试了两种机器学习分类器：（1）基于多个单日记录训练的Somnotate，以及（2）基于每个记录中一小部分子集训练的Somnivore。由于之前从未将自动评分方法应用于冬眠物种，一个主要问题是脑温度变化对脑电图以及基于机器学习的检测的影响。因此，我们选择了参考数据，这些数据来自6只熊的3位手动评分者的共识，包括冬眠期间体温在多日周期内振荡时最高和最低体温的两个单日记录，以及夏季非冬眠的一个单日记录。当分别对冬眠和非冬眠数据进行训练时，Somnotate的结果非常出色。在冬眠期内分别针对高Tb和低Tb训练Somnotate并未进一步改善结果。根据自动评分和手动评分，冬眠期的睡眠时间约为夏季的2倍（p<0.0001）。在冬眠期间，自动评分和手动评分之间在警戒状态占有率上没有显著差异（p>0.05），但夏季的睡眠时间被轻微高估（p<0.05）。两种应用与手动评分的F值均在0.90-0.98范围内。在0.67-0.88范围内的异常值在两个应用之间存在相关性，表明特定文件更具挑战性。我们得出结论，当在高质量数据上训练时，两种应用的准确性都接近手动评分者。

## Abstract
Hibernating bears show remarkable metabolic suppression. Their decline in core body temperature (Tb) is moderate(from 38{degrees}C to 30-35{degrees}C), but their metabolism declines as much as 75%. To understand the role of sleep in this hypometabolic state, we recorded biotelemetrically EEG, EOG and EMG data over 3500 days from 16 captive American black bears in and out of hibernation under semi-natural conditions. This data set is too large to score manually for Wake, REM- and NREM sleep, so we tested two machine learning classifiers: (1) Somnotate trained on multiple one-day recordings, and (2) Somnivore, trained on a small subset from each recording. As automated scoring methods have not been applied to hibernating species before, a major concern is the effect changing brain temperature has on the EEG and on the machine learning based detection. Therefore, we selected reference data using consensus by 3 manual sleep scorers from each of 6 bears, two one-day recordings at the highest and lowest body temperatures during hibernation when Tb was oscillating in multiday cycles, and a non-hibernating one-day recording in summer. Somnotate results were excellent when trained separately for hibernating and non-hibernating data. Training Somnotate separately for high and low Tbb within hibernation did not improve results further. Sleep times in hibernation were about 2x that in summer for both automated scores and manual scores (p<0.0001). There were no significant differences in occupancy of vigilance states between automated and manual scores in hibernation (p>0.05), but a small overestimate of sleep time in summer (p<0.05). Both applications yielded F-measures against manual scores in the 0.90-0.98 range. Outliers in the 0.67-0.88 range were correlated between the two applications, indicating that specific files are more challenging to annotate. We conclude that both applications have accuracies approaching that of manual scorers when trained on high quality data.

---

## 论文详细总结（自动生成）

## 论文核心问题与整体含义（研究动机和背景）

- **研究动机**：冬眠熊在冬眠期间表现出显著的代谢抑制（代谢率下降高达75%），同时核心体温仅适度降低（从38°C降至30-35°C）。为理解睡眠在这种低代谢状态中的作用，需要大规模分析熊的睡眠-觉醒状态。然而，传统人工睡眠评分耗时巨大，无法处理长达3500天的生物遥测数据。
- **核心问题**：首次将自动化睡眠评分方法应用于冬眠物种，验证机器学习分类器在冬眠熊EEG/EOG/EMG数据上的准确性，并探讨脑温变化对EEG信号和机器学习检测的影响。
- **整体含义**：为大规模研究冬眠动物睡眠模式提供可靠工具，揭示冬眠期间睡眠时间显著增加的现象，并评估自动评分方法在非标准生理状态（如体温波动）下的适用性。

## 论文提出的方法论

- **核心思想**：使用两种机器学习分类器自动对脑电图（EEG）、眼电图（EOG）和肌电图（EMG）进行睡眠分期（清醒、快速眼动睡眠REM、非快速眼动睡眠NREM）。
- **关键技术细节**：
  - **Somnotate**：基于多个单日记录进行训练，适用于多日连续数据。
  - **Somnivore**：基于每个记录中一小部分子集进行训练（即每个录音仅使用少量标记数据）。
  - 参考标准：由3名人工评分者对6只熊的冬眠期（分别选取体温最高和最低的两个单日记录）和夏季（一个单日记录）进行共识评分。
- **算法流程（文字说明）**：
  1. 数据采集：16只圈养美洲黑熊在冬眠期和非冬眠期，半自然条件下记录EEG、EOG、EMG，共超过3500天。
  2. 数据划分：选择6只熊的参考子集（共3个单日记录/熊：冬眠高体温、冬眠低体温、夏季非冬眠）。
  3. 训练与评估：
     - Somnotate：分别对冬眠和非冬眠数据进行单独训练（冬眠内再尝试按高/低体温分开训练）。
     - Somnivore：从每个记录中提取小部分子集训练，然后对全部数据进行评分。
  4. 比较：自动评分结果与人工共识评分对比，计算F值（F-measure）、占有率差异等指标。

## 实验设计

- **数据集/场景**：
  - 数据总规模：16只熊，3500天，EEG/EOG/EMG遥测数据。
  - 参考子集：6只熊，每只3个单日记录（共18个记录），包括：
    - 冬眠期两个记录：体温最高时和最低时（因冬眠期间体温呈多日周期振荡）。
    - 夏季非冬眠一个记录。
  - 人工评分：3位评分者共识生成标准标签。
- **基准（Benchmark）**：人工评分的共识结果作为金标准。
- **对比方法**：
  - 对比两种自动评分工具：Somnotate vs. Somnivore。
  - 对比冬眠期高体温与低体温分别训练 vs. 合并训练的效果。
  - 对比冬眠期 vs. 夏季的评分准确性和睡眠时间估计。

## 资源与算力

- 论文中**未明确说明**使用的GPU型号、数量或训练时长。仅提及基于机器学习分类器（Somnotate和Somnivore），但未提供具体计算资源细节。推测为常规计算设备，可能无需大量GPU资源（特征提取和分类器较为标准）。

## 实验数量与充分性

- **实验组数**：
  - 主要评估：6只熊×3个记录×2种自动方法，对比人工共识。
  - 额外实验：冬眠期内按高/低体温分别训练Somnotate，与合并训练比较。
  - 统计比较：冬眠期 vs 夏季睡眠时间差异（p值）、自动 vs 人工占有率差异（p值）。
- **充分性**：
  - 样本量（6只熊，18个记录）对于初步验证自动评分在冬眠物种中的可行性较为合理，但可能不足以覆盖所有个体差异。
  - 对比了两种不同的自动方法，且有内部变温条件下的子实验，设计较为周全。
  - 客观性：采用多人共识评分作为金标准，避免了单一人为偏差。
  - 公平性：两种方法使用相同的数据集，评估指标一致（F值、占有率）。

## 论文的主要结论与发现

1. 当分别在冬眠和非冬眠数据上训练时，**Somnotate结果优秀**，F值在0.90-0.98范围内。
2. 在冬眠期内按高/低体温分别训练Somnotate**并未进一步改善结果**，说明体温振荡对自动评分影响不大。
3. **冬眠期睡眠时间约为夏季的2倍**（p<0.0001），自动评分和人工评分一致。
4. 冬眠期自动评分与人工评分在警戒状态占有率上**无显著差异**（p>0.05），但夏季自动评分轻微高估睡眠时间（p<0.05）。
5. 两种方法（Somnotate和Somnivore）与人工评分的F值均在0.67-0.88范围内的异常值存在相关性，说明特定文件更难以标注（可能由于信号噪声、伪迹等）。
6. 两种自动评分方法的准确性**接近人工评分者**，可替代人工处理大规模数据。

## 优点

- **研究创新性**：首次将自动睡眠评分应用于冬眠物种，填补了该领域空白。
- **方法稳健性**：测试了两种不同训练策略的机器学习方法，验证了在不同体温条件下的泛化能力。
- **数据质量**：使用多人共识评分（3位评分者）保证金标准质量，减少主观偏差。
- **统计严谨性**：报告了F值、p值等统计指标，明确自动评分的偏差和异常值。
- **实际应用价值**：为大规模生物遥测数据（如3500天）的自动化处理提供了可行方案，显著提高研究效率。

## 不足与局限

- **样本量有限**：仅对6只熊的18天数据进行了详细验证，且所有熊为圈养状态，可能无法完全代表野外熊的真实睡眠模式。
- **夏季高估问题**：自动评分在夏季轻微高估睡眠时间，需要进一步调优或校准。
- **体温变化影响未完全排除**：尽管按高/低体温分别训练未改善结果，但论文未深入分析脑温变化对EEG频谱的具体影响，可能存在潜在干扰。
- **异常值原因不明**：F值在0.67-0.88的异常文件未详细分析其信号特征或个体差异，限制了方法的鲁棒性理解。
- **算力资源未报告**：未提供训练时间、硬件配置等，难以评估方法的实际效率。
- **仅比较了两种方法**：未与更先进的深度学习模型（如CNN、Transformer）对比，可能错过更优方案。
- **应用限制**：本方法依赖于高质量遥测数据，若信号质量差或存在大量伪迹，自动评分准确性可能下降。

（完）
