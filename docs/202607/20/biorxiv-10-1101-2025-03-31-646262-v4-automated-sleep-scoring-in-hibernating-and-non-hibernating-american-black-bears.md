---
title: Automated sleep scoring in hibernating and non-hibernating American black bears
title_zh: 冬眠与非冬眠的美洲黑熊自动睡眠评分
authors: "Toien, O., Pittaras, E. C., Huang, Y.-G., Brodersen, P. J. N., Allocca, G., Barnes, B. M., Heller, H. C."
date: 2026-07-14
pdf: "https://www.biorxiv.org/content/10.1101/2025.03.31.646262v4.full.pdf"
tags: ["query:tr-hb"]
score: 9.0
evidence: 冬眠黑熊的自动睡眠评分，涉及代谢抑制和体温下降
tldr: 研究黑熊冬眠期间的睡眠，由于3500天EEG数据量巨大，需自动化评分。测试Somnotate（基于多日训练）和Somnivore（基于子集训练）两种分类器，考虑脑温变化对EEG影响。结果显示，F-measure达0.90-0.98，冬眠睡眠时长约为夏季2倍，自动评分在冬眠期与人工无显著差异，夏季略有高估。表明高质量训练下自动评分可接近人工水平。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-03-31-646262-v4/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1658, \"height\": 410}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-03-31-646262-v4/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1616, \"height\": 460}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-03-31-646262-v4/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1283, \"height\": 783}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-03-31-646262-v4/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1282, \"height\": 783}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-03-31-646262-v4/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1394, \"height\": 842}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-03-31-646262-v4/fig-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 1316, \"height\": 948}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-03-31-646262-v4/fig-007.webp\", \"caption\": \"\", \"page\": 0, \"index\": 7, \"width\": 1366, \"height\": 725}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-03-31-646262-v4/fig-008.webp\", \"caption\": \"\", \"page\": 0, \"index\": 8, \"width\": 1364, \"height\": 728}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-03-31-646262-v4/fig-009.webp\", \"caption\": \"\", \"page\": 0, \"index\": 9, \"width\": 1398, \"height\": 499}]"
tables_json: "[{\"url\": \"assets/tables/biorxiv/biorxiv-10-1101-2025-03-31-646262-v4/table-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1489, \"height\": 171}]"
motivation: 手动评分大量冬眠黑熊的睡眠数据耗时且不可行，且脑温变化可能影响机器学习检测的准确性。
method: 采用Somnotate和Somnivore两种机器学习分类器，分别对冬眠与非冬眠数据训练，并分析高低温对评分的影响。
result: 两种方法F-measure在0.90-0.98，冬眠睡眠时间约夏季2倍；冬眠期自动与人工评分无显著差异，夏季睡眠时间略高估。
conclusion: 自动睡眠评分方法在高质量训练数据下准确性接近人工，可用于冬眠物种的睡眠分析。
---

## 摘要
冬眠熊表现出显著的代谢抑制。它们的核心体温(Tb)下降幅度适中(从38°C降至30-35°C)，但代谢率下降高达75%。为了解睡眠在这种低代谢状态中的作用，我们在半自然条件下记录了16只圈养美洲黑熊在冬眠期和非冬眠期超过3500天的脑电图(EEG)、眼电图(EOG)和肌电图(EMG)数据。该数据集太大，无法手动对清醒、快速眼动睡眠和非快速眼动睡眠进行评分，因此我们测试了两种机器学习分类器：(1) 基于多个单日录音训练的Somnotate，以及(2) 基于每个录音的一小部分子集训练的Somnivore。由于自动评分方法此前未应用于冬眠物种，一个主要问题是脑温变化对脑电图和基于机器学习的检测的影响。因此，我们从6只熊中各选取了参考数据，采用3名手动睡眠评分者的共识，分别选取了冬眠期间体温在多日周期中振荡时的最高和最低体温下的两个单日录音，以及夏季非冬眠的一个单日录音。当分别针对冬眠和非冬眠数据进行训练时，Somnotate的结果非常出色。在冬眠期内分别针对高Tb和低Tb训练Somnotate并未进一步改善结果。无论是自动评分还是手动评分，冬眠期的睡眠时间约为夏季的两倍(p<0.0001)。冬眠期自动评分与手动评分在警戒状态占用率上没有显著差异(p>0.05)，但夏季睡眠时间存在轻微高估(p<0.05)。两种应用相对于手动评分的F-measure均在0.90-0.98范围内。异常值在0.67-0.88范围内，在两个应用之间相关，表明特定文件注释更具挑战性。我们得出结论，当使用高质量数据训练时，两种应用的准确性接近手动评分者。

## Abstract
Hibernating bears show remarkable metabolic suppression. Their decline in core body temperature (Tb) is moderate (from 38{degrees}C to 30-35{degrees}C), but their metabolism declines as much as 75%. To understand the role of sleep in this hypometabolic state, we recorded biotelemetrically EEG, EOG and EMG data over 3500 days from 16 captive American black bears in and out of hibernation under semi-natural conditions. This data set is too large to score manually for Wake, REM- and NREM sleep, so we tested two machine learning classifiers: (1) Somnotate trained on multiple one-day recordings, and (2) Somnivore, trained on a small subset from each recording. As automated scoring methods have not been applied to hibernating species before, a major concern is the effect changing brain temperature has on the EEG and on the machine learning based detection. Therefore, we selected reference data using consensus by 3 manual sleep scorers from each of 6 bears, two one-day recordings at the highest and lowest body temperatures during hibernation when Tb was oscillating in multiday cycles, and a non-hibernating one-day recording in summer. Somnotate results were excellent when trained separately for hibernating and non-hibernating data. Training Somnotate separately for high and low Tb within hibernation did not improve results further. Sleep times in hibernation were about 2x that in summer for both automated scores and manual scores (p<0.0001). There were no significant differences in occupancy of vigilance states between automated and manual scores in hibernation (p>0.05), but a small overestimate of sleep time in summer (p<0.05). Both applications yielded F-measures against manual scores in the 0.90-0.98 range. Outliers in the 0.67-0.88 range were correlated between the two applications, indicating that specific files are more challenging to annotate. We conclude that both applications have accuracies approaching that of manual scorers when trained on high quality data.

---

## 论文详细总结（自动生成）

# 中文总结：冬眠与非冬眠美洲黑熊自动睡眠评分

## 1. 论文的核心问题与整体含义（研究动机和背景）
- **核心问题**：冬眠黑熊代谢率显著降低（降至基础代谢率的25%），核心体温从38°C降至30-35°C，且呈现多日体温振荡。为理解睡眠在低代谢状态中的作用，研究者收集了16只黑熊超过3500天的脑电图（EEG）、眼电图（EOG）、肌电图（EMG）等多导睡眠数据。然而，手动评分如此庞大的数据集不可行，亟需可靠的自动评分方法。
- **关键挑战**：这是首次将机器学习自动睡眠评分应用于冬眠物种。冬眠期间脑温变化可能引起EEG频率分布改变，从而影响基于频域特征的机器学习检测的准确性。需验证自动评分在冬眠与非冬眠状态下的鲁棒性。
- **整体意义**：成功验证自动睡眠评分方法后，可大规模分析黑熊冬眠全过程的睡眠结构，为理解冬眠状态下的代谢抑制与睡眠功能提供基础，并为治疗性低代谢（如人工诱导冬眠）提供参考。

## 2. 论文提出的方法论：核心思想、关键技术细节
- **核心思想**：利用两种不同设计的机器学习分类器，对黑熊的EEG和EOG信号进行10秒历元的Wake、NREM、REM三分类。通过人工共识评分建立参考标准，分别评估不同训练策略下的评分准确性。
- **关键技术细节**：
  - **Somnotate**：开源概率分类器，基于线性判别分析（LDA）与隐马尔可夫模型（HMM）组合。可累积多只动物、多日文件进行训练，支持留一法验证（hold-out）。训练使用EEG+EOG信道，采样间隔10秒。
  - **Somnivore**：商用辅助机器学习软件，对每个待测文件随机抽取100个历元（每个状态）进行训练，不跨文件训练。同样使用EEG+EOG信道，设置最小连续3个历元一致性规则。
  - **训练策略**：对Somnotate测试了三种训练集构建方式：(a) 全部参考数据（冬眠+夏季）；(b) 冬眠与夏季分别训练；(c) 冬眠内部按高体温（Tb峰值）和低体温（Tb谷值）分别训练。对Somnivore则测试了同文件训练、同动物不同Tb文件训练、不同动物文件训练。
  - **评分规则**：仅分Wake、NREM、REM三类，未单独标定“昏昏欲睡”状态。允许Wake→REM过渡不做限制。

## 3. 实验设计：数据集、基准方法与对比
- **数据集**：从6只黑熊中选取3个24小时录音：冬眠期最高体温日（Tb≈34.9°C）、冬眠期最低体温日（Tb≈32.1°C）、夏季非冬眠日（Tb≈38.1°C）。共18份单日文件。由3名有经验的手动评分者独立评分，通过投票生成共识评分，作为黄金标准（0.5%的历元无共识）。
- **基准方法**：人工共识评分作为绝对基准。自动评分与共识对比，评估整体准确率、F1值等。
- **对比方法**：主要比较Somnotate与Somnivore两种软件；此外，对Somnotate比较了不同训练集（全部数据、分季节、分体温）和留一法验证与全训练集验证；对Somnivore比较了不同训练通道（仅EEG vs. EEG+EOG）和不同训练数据来源（同文件 vs. 跨动物 vs. 同动物不同Tb）。

## 4. 资源与算力
- **文中未明确说明**：论文没有提及使用的GPU型号、数量、训练时长、内存等计算资源。仅提到Somnotate和Somnivore在普通工作站上运行，但具体硬件配置缺失。因此无法评估算力需求。

## 5. 实验数量与充分性
- **实验数量**：
  - 手动评分基准：3名评分者 × 18个文件，生成共识。
  - Somnivore：对不同训练通道（EEG仅、EEG+EOG等）、不同训练数据源（同文件、跨动物、跨Tb）各测试了6只熊的冬眠和夏季数据。
  - Somnotate：测试了5种训练策略（全部数据、单季节、分体温、留一法 vs. 全训练），每种策略计算整体准确率。
  - 详细性能评估：对每个状态（NREM、REM、Wake）计算F1值，并展示24小时时间序列对照图（图6）。
- **充分性评估**：
  - 优点：实验设计涵盖了冬眠与非冬眠、体温高低变化对自动评分的影响；使用了多名手动评分者共识减少主观偏差；对比了两种代表性软件。
  - 不足：样本仅6只熊，每种条件只有1个24小时录音（冬眠高Tb、低Tb各1天，夏季1天），统计效力有限。未进行跨冬眠季节（例如早冬、晚冬）的验证。没有做更细致的消融实验（如仅使用不同频率子带训练）。对罕见过渡状态（如Wake→REM）的分析仅基于描述性统计。

## 6. 论文的主要结论与发现
- **冬眠睡眠时间约为夏季的2倍**：手动共识显示冬眠NREM 42.9%、REM 22.0%、总睡眠64.9%，夏季分别为21.9%、9.7%、31.7%。自动评分结果与之一致，且冬眠与夏季差异显著（p<0.0001）。
- **自动评分准确性与手动评分相当**：F1值大多在0.90-0.98之间，接近先前人工之间的一致性（94.5%）。冬眠期自动评分与共识在状态占用率上无显著差异；夏季存在轻微（约2-5%）但显著的睡眠高估/清醒低估。
- **脑温变化对评分影响可控**：对Somnotate，分别训练高/低温并未改善结果；统一使用冬眠数据训练即可获得良好性能。但Somnotate若混合夏季数据训练反而降低夏季评分准确率。
- **两种软件性能相似**：Somnotate与Somnivore在F1值和状态分布上无显著差异。低F1值文件（异常值）在两个软件中一致，说明某些文件本身更难评分。
- **辅助机器学习设计的重要性**：Somnivore在不同动物或不同Tb文件间训练时准确率大幅下降，必须采用同文件内训练；Somnotate因能积累多文件训练，故鲁棒性更强。

## 7. 优点：方法或实验设计亮点
- **首次验证了冬眠物种自动睡眠评分**，填补了大型低代谢动物自动评分研究的空白。
- **采用多人人工共识**作为黄金标准，减少单个评分者主观偏差，提高了参考标准的可靠性。
- **系统测试了脑温变化的影响**，通过选取体温周期峰谷及分别训练，确认了冬眠内部体温变化不构成显著障碍。
- **对比两种设计迥异的软件**（开源概率模型 vs. 商业辅助ML），展示了不同训练策略的优劣，为后续研究者选择工具提供参考。
- **数据公开**：原始数据已存入国家睡眠研究资源库，代码开源，提高了可复现性。

## 8. 不足与局限
- **样本量小**：仅6只熊，每只仅3天数据（冬眠2天+夏季1天），季节内变异、个体差异难以充分评估。后续需推广到更多熊、更长时间跨度的数据。
- **实验覆盖不完整**：冬眠期只评估了中冬的两天，未测试入冬初期、出冬期及多日体温循环的其他阶段；夏季只选取1天，可能无法代表整个活动季。
- **未评估更细分的睡眠阶段**（如人类N1/N2/N3或动物的Drowsiness），仅三分类，可能丢失重要信息。作者尝试添加Drowsiness但因一致性差而放弃。
- **对过渡状态的分析较浅**；自动评分中Wake→REM过渡比率远高于手动共识，但论文仅用“短时”解释，未深入验证这些过渡的生理真实性或是否为伪影。
- **未报告计算资源与训练时间**，不利于重复实验或评估可扩展性至更大数据集。
- **Somnivore设计上的局限性**：不能有效跨文件训练，在大规模自动化批处理中需要人工为每个文件挑选训练历元，仍有一定人力成本。
- **EMG信噪比差**：冬眠期黑熊蜷缩姿势导致三角肌EMG几乎无信号，限制了多通道输入的优势，可能影响REM检测。

（完）
