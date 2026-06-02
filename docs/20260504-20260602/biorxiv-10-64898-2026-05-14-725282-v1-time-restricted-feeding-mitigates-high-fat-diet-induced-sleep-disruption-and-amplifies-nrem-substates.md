---
title: Time Restricted Feeding Mitigates High-Fat-Diet Induced Sleep Disruption and Amplifies NREM Substates
title_zh: 限时饮食减轻高脂饮食诱导的睡眠中断并增强NREM子状态
authors: "Lam, M. T. Y., Askari, K., Changiz Ashtiani, K., Li, Y., Andrews, N. A., Panda, S."
date: 2026-05-18
pdf: "https://www.biorxiv.org/content/10.64898/2026.05.14.725282v1.full.pdf"
tags: ["query:slp-ns"]
score: 9.0
evidence: 高脂饮食下的睡眠破坏与NREM子状态
tldr: 高脂饮食引起小鼠睡眠碎片化和潜伏期延长，而将进食限制在昼夜活动窗口（时间限制性进食）可缓解这些宏观睡眠紊乱。利用无监督机器学习对NREM睡眠进行微状态聚类，发现两种高振幅子状态：低δ波功率的慢波睡眠和含α/σ/β功率的子状态。时间限制性进食在光期长睡眠片段中选择性增加这两种子状态的频率。该研究建立了量化小鼠睡眠微结构的客观框架，表明调整进食时间与昼夜节律同步可改善高脂饮食诱导的睡眠障碍并增强不同NREM亚状态。
source: biorxiv
selection_source: fresh_fetch
motivation: 探究高脂饮食限制性进食时机对睡眠宏观和微观结构的影响，尤其是NREM睡眠中的异质性子状态。
method: 结合EEG特征提取与无监督机器学习聚类，对小鼠10秒NREM睡眠片段进行子状态识别并分析不同饮食干预的影响。
result: 高脂饮食增加睡眠潜伏期和碎片化；主动阶段时间限制性进食改善这些异常并增加两种NREM子状态（低δ波子状态和含α/σ/β功率子状态）的频率。
conclusion: 将热量摄入限制在昼夜主动窗口可减轻高脂饮食诱导的宏观睡眠紊乱并选择性增强不同的NREM亚状态，为睡眠与代谢联合干预提供新策略。
---

## 摘要
饮食质量和进食时间对睡眠质量的影响仍知之甚少，尤其是在睡眠微结构层面。传统的视觉评分仅能捕捉粗略的睡眠分期，忽略了小鼠非快速眼动（NREM）睡眠中脑电图（EEG）模式的显著异质性。在此，我们应用一种结合EEG特征提取与基于无监督机器学习聚类的流程，以解析离散的NREM子状态，并探究高脂饮食（HFD）和限时饮食（TRF）如何影响睡眠微结构。HFD增加睡眠潜伏期和睡眠碎片化；这两种异常均通过活跃期TRF得到改善。对10秒时段的聚类识别出两种对TRF敏感的高幅NREM子状态：聚类1富含低Delta功率，在光照期早期（ZT 0-6）达到峰值，符合经典慢波睡眠；聚类6以Alpha、Sigma和Beta功率升高为特征，在光照期后半段（ZT6-12）达到峰值。TRF增加两种NREM子状态的频率，尤其是在光照期较长的不间断睡眠片段中。这些发现引入了一个量化小鼠睡眠微结构的客观框架，并表明将热量摄入与昼夜活跃窗口对齐可减轻HFD诱导的宏观睡眠中断，同时选择性地增强两种生理上不同的NREM子状态。

意义声明：限时饮食——将食物摄入限制在昼夜活跃期内的特定窗口——具有公认的代谢益处，但其对睡眠的影响在很大程度上尚未被探索。通过连续EEG/EMG记录，我们表明活跃期进食窗口可减轻高脂饮食诱导的小鼠睡眠中断。我们采用了一种新颖的机器学习流程，进一步揭示定时进食选择性地增强不同的NREM子状态，证明“我们何时进食”精细调节了睡眠的宏观和微观结构。这些见解为未来旨在利用定时进食改善代谢和睡眠健康的转化研究和临床试验奠定了基础。

## Abstract
The effects of diet quality and timing on sleep quality remain poorly understood, particularly at the level of sleep microarchitecture. Traditional visual scoring captures only coarse sleep stages, overlooking the marked heterogeneity of electroencephalographic (EEG) patterns in non-rapid eye movement (NREM) sleep of mice. Here, we apply a pipeline that combines EEG feature extraction with unsupervised machine-learning-based clustering to resolve discrete NREM substates and ask how a high-fat diet (HFD) and time- restricted feeding (TRF) affect sleep microarchitectures. HFD increases sleep latency and sleep fragmentation; both abnormalities were ameliorated by active phase TRF. Clustering of 10s epochs identified two high-amplitude NREM substates sensitive to TRF: Cluster 1, enriched in low-delta power and peaking early in the light phase (ZT 0-6), consistent with canonical slow-wave sleep, and Cluster 6, characterized by elevated alpha, sigma, and beta power and peaking in the latter half of the light phase (ZT6-12). TRF increases the frequency of both NREM substates, particularly within longer uninterrupted sleep episodes during the light phases. These findings introduce an objective framework for quantifying murine sleep microarchitecture and show that aligning caloric intake with the circadian active window mitigates HFD-induced macro-level sleep disruption while selectively enhancing two physiologically distinct NREM substates.

Significance StatementTime-restricted eating - targeting food intake to a defined window during the circadian active phase - confers well-established metabolic benefits, but its impact on sleep is largely underexplored. Using continuous EEG/EMG recordings, we show that an active- phase eating window mitigates high-fat-diet-induced sleep disruption in mice. We employed a novel machine-learning pipeline, further revealing that timed eating selectively increases distinct NREM substates, demonstrating that "when we eat" fine-tunes the macro- and microarchitecture of sleep. These insights lay the foundation for future translational studies and clinical trials aimed at harnessing timed eating to enhance both metabolic and sleep health.

---

## 论文详细总结（自动生成）

## 1. 论文的核心问题与整体含义（研究动机和背景）

- **研究动机**：饮食质量（特别是高脂饮食）和进食时间对睡眠质量的影响尚未被充分理解，尤其是对睡眠微结构（如NREM睡眠中的异质性EEG模式）的影响。传统视觉评分仅能区分粗略的睡眠期（如NREM、REM、清醒），忽略了NREM睡眠内部脑电图模式的显著差异。
- **背景**：限时饮食（TRF，将食物摄入限制在昼夜活跃窗口内）已被证实具有代谢益处，但其对睡眠的影响研究很少。本论文旨在探究高脂饮食（HFD）如何破坏睡眠宏观与微观结构，以及活跃期TRF能否缓解这些破坏，并进一步揭示NREM睡眠中不同的子状态。

## 2. 论文提出的方法论：核心思想、关键技术细节

- **核心思想**：结合EEG特征提取与无监督机器学习聚类，对小鼠NREM睡眠的10秒片段进行子状态识别，从而量化睡眠微结构，并分析饮食干预对子状态的影响。
- **关键技术细节**：
  - 数据采集：连续EEG/EMG记录小鼠睡眠。
  - 特征提取：从10秒NREM片段中提取多种EEG频段功率特征（如Delta、Theta、Alpha、Sigma、Beta等）。
  - 聚类算法：采用无监督机器学习方法（文献未明确具体算法，推测为K-means或层次聚类）对特征进行聚类，识别离散的NREM子状态。
  - 子状态识别：聚类得到多种子状态，重点分析两种高幅子状态——聚类1（低Delta功率，类经典慢波睡眠，在光期早期ZT0-6达峰）和聚类6（高Alpha/Sigma/Beta功率，在光期后半ZT6-12达峰）。
- **流程简述**：EEG原始数据 → 睡眠分期（传统评分） → 提取NREM片段 → 每10秒提取频域特征 → 无监督聚类 → 分析各子状态在不同饮食条件下的出现频率、持续时间、昼夜分布等。

## 3. 实验设计

- **数据集/场景**：
  - 动物模型：小鼠。
  - 饮食条件：
    - 正常饮食（ND）
    - 高脂饮食（HFD）
    - 高脂饮食 + 活跃期限时饮食（HFD+TRF，仅允许在昼夜活动窗口进食）
  - 记录方式：连续EEG/EMG监测。
- **基准（Benchmark）**：未明确设立外部基准，主要对比HFD组与ND组、HFD+TRF组与HFD组之间的睡眠宏观和微观指标。
- **对比方法**：未对比其他睡眠分析技术（如传统频谱分析、隐马尔可夫模型等）。方法本身是新的客观框架，未提及与其他方法比较。

## 4. 资源与算力

- **文中未说明**：论文未提及使用的GPU型号、数量、训练时长等算力信息。仅提到采用了机器学习聚类，但未说明具体计算资源。这在预印本中常见，后续版本可能补充。

## 5. 实验数量与充分性

- **实验组数**：主要涉及三组饮食条件（ND、HFD、HFD+TRF），每组可能有多只小鼠。未明确具体样本量。
- **是否充分**：
  - 宏观睡眠分析（潜伏期、碎片化等）结果清晰，TRF改善效果明显。
  - 微状态聚类分析仅汇报了两种显著受TRF影响的子状态，但未展示所有聚类结果（可能共有多个聚类）。
  - 缺乏统计学细节（如p值、效应量）或多次重复实验的验证。
  - 未进行消融实验或交叉验证（如不同特征选择、不同聚类算法对比）。
  - 结论基于单一预印本研究，客观性和可重复性有待后续评估。

## 6. 论文的主要结论与发现

- HFD导致小鼠睡眠潜伏期增加、睡眠碎片化加剧（宏观破坏）。
- 活跃期TRF可以显著改善上述HFD诱导的宏观睡眠异常。
- 通过无监督聚类，识别出两种对TRF敏感的NREM子状态：
  - 聚类1：低Delta功率，在光期早期出现，符合经典慢波睡眠。
  - 聚类6：高Alpha、Sigma、Beta功率，在光期后期出现。
- TRF选择性地增加这两种NREM子状态的频率，尤其是在光期较长的不间断睡眠片段中。
- 结论：将热量摄入与昼夜活跃窗口对齐不仅可以减轻HFD引起的宏观睡眠破坏，还能增强生理上不同的NREM亚状态，表明“何时进食”精细调节睡眠宏观和微观结构。

## 7. 优点：方法或实验设计上的亮点

- **客观量化睡眠微结构**：利用无监督机器学习自动识别NREM子状态，避免人工评分的主观性，为小鼠睡眠研究提供了可重复的客观框架。
- **打破传统分期局限**：首次在饮食干预研究中揭示NREM睡眠内部的异质性，发现两种具有不同频谱特征的子状态，并显示它们对进食时间的不同响应。
- **融合代谢与睡眠**：将TRF（代谢干预）与睡眠微观动力学结合，为未来代谢-睡眠交叉领域研究提供新方向。
- **预印本及时性**：快速公开研究发现，利于学科交流。

## 8. 不足与局限

- **实验覆盖有限**：仅使用小鼠模型，未涉及人类或其他物种。人鼠睡眠结构差异大，转化应用需谨慎。
- **缺乏对照方法**：未与传统睡眠分析（如基于功率谱密度的慢波活动识别）进行对比，难以评估新方法的相对优势。
- **未报告所有聚类结果**：可能丢弃了其他NREM子状态，仅聚焦两个显著聚类，可能存在选择偏向。
- **统计细节缺失**：未展示效应量、置信区间、多重比较校正等，因果推论强度不足。
- **未控制潜在混杂因素**：如活动量、体重变化、光照周期等未明确讨论。
- **算力和代码未公开**：未提供代码或数据，可复现性受限。
- **预印本未经同行评审**：结论有待正式发表验证。

（完）
