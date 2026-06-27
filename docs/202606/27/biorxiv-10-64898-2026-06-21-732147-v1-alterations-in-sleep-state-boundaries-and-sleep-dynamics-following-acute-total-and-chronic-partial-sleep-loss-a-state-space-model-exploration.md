---
title: "Alterations in sleep state boundaries and sleep dynamics following acute total and chronic partial sleep loss: a state space model exploration"
title_zh: 急性完全性睡眠剥夺与慢性部分性睡眠缺失后睡眠状态边界及睡眠动力学的改变：一项状态空间模型探索
authors: "Reutimann, S., Imbach, L., Burkhard, Z., Baumann, C. R., Maric, A."
date: 2026-06-25
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.21.732147v1.full.pdf"
tags: ["query:slp-ns"]
score: 9.0
evidence: 研究睡眠剥夺后睡眠状态边界和动态，直接相关睡眠神经科学
tldr: 急性和慢性睡眠损失对睡眠结构的影响不同。本研究使用状态空间模型分析EEG，发现慢性睡眠限制增加了REM与清醒状态的频谱相似性，模糊了状态边界；而急性睡眠剥夺则改变了NREM频谱组成，使慢波睡眠更稳定。这些差异表明睡眠结构具有状态依赖性，未来可用于监测临床治疗。
source: biorxiv
selection_source: fresh_fetch
motivation: 探究急性和慢性睡眠损失对睡眠状态边界和动态的量化影响差异。
method: 对14名受试者在基线、慢性限制(5小时/床7晚)和急性剥夺(40小时清醒)后，应用状态空间模型分析EEG。
result: 慢性限制降低REM与清醒区分度；急性剥夺改变NREM频谱并增强慢波睡眠稳定性。
conclusion: 睡眠结构变化具有状态依赖性，可用于追踪睡眠失调人群的治疗效果。
---

## 摘要
慢性部分性睡眠缺失与急性完全性睡眠剥夺对睡眠结构有着截然不同的影响。即，急性睡眠剥夺主要导致慢波睡眠的强烈反弹，而慢性睡眠限制则导致快速眼动睡眠倾向的增加。本研究的目的是运用基于模型的方法，探讨这些不同效应是否会转化为睡眠状态边界及动力学的可量化改变。

除了传统的睡眠分期评分，我们还采用了脑电图模型（状态空间方法）对14名健康受试者在实验性慢性睡眠限制（连续7晚，每晚卧床5小时中的最后一晚）后以及急性睡眠剥夺（40小时觉醒后的睡眠）后的夜间脑电图记录进行动态分析，并与基线睡眠进行比较。

处于慢性睡眠限制下的受试者显示出快速眼动睡眠与觉醒状态在频率成分上更高的相似性，因此两种行为状态之间的边界区分度降低。相反，急性睡眠剥夺影响了非快速眼动睡眠的频谱组成。只有急性睡眠剥夺导致了更稳定的慢波睡眠。

我们的探索性研究证实，急性完全性睡眠剥夺后的快速眼动睡眠倾向增加和慢波睡眠倾向增加这两种截然不同的效应，在行为状态边界和睡眠动力学的差异变化中得到了体现。这表明这些睡眠结构特征具有状态依赖性，未来可能利用这些指标来追踪以睡眠行为状态失调为特征的临床人群的治疗效果。

## Abstract
Chronic partial and acute total sleep loss have a distinct impact on sleep architecture. Namely, acute sleep deprivation primarily leads to a strong rebound of slow wave sleep, while chronic sleep restriction results in an increased propensity of REM sleep. The aim of this work was to examine whether these different effects would translate into quantifiable changes in sleep state boundaries and dynamics using a model-based method.

Besides conventional sleep stage scoring, we applied an EEG model (state space approach) for dynamic analysis of nocturnal EEG recordings in 14 healthy subjects under experimental chronic sleep restriction (last of 7 nights with 5 hours of time in bed) and after acute sleep deprivation (sleep following 40 hours of wakefulness), in comparison to baseline sleep.

Subjects under chronic sleep restriction revealed increased similarities in the frequency composition of REM sleep and wakefulness and thus, a decreased differentiation of state boundaries between the two behavioral states. Contrarily, acute sleep deprivation affected the spectral composition of NREM sleep. Only acute sleep deprivation resulted in more stable slow wave sleep.

Our explorative study confirmed that the distinct effects of increased REM sleep and slow wave sleep propensity following acute total and chronic partial sleep loss are reflected in differential changes of behavioral state boundaries and sleep dynamics. This suggests that these sleep structure characteristics are state dependent, which may allow using such measures in the future to track treatment effects in clinical populations characterized by sleep behavioral state dysregulation.

---

## 论文详细总结（自动生成）

# 中文详细总结

## 1. 论文的核心问题与整体含义（研究动机和背景）

- **核心问题**：急性完全性睡眠剥夺（ASD）与慢性部分性睡眠限制（CSR）对睡眠结构的影响不同——ASD主要引发慢波睡眠（SWS）反弹，CSR主要增加快速眼动睡眠（REM）倾向。但两者对睡眠状态边界（state boundaries）和睡眠动力学（sleep dynamics）的量化影响尚不清楚。
- **研究动机**：传统睡眠分期仅提供全局睡眠架构信息，而状态空间分析（SSA）能定量评估睡眠状态间的频谱相似性、稳定性及动态转换。之前SSA已用于病理人群（如嗜睡症、帕金森病）的睡眠异常，但未知SSA指标是否受睡眠调控机制调节。
- **整体含义**：验证SSA能否区分ASD和CSR的不同效果，从而证明这些指标是状态依赖的，未来可用于监测临床治疗（如睡眠行为失调患者）。

## 2. 论文提出的方法论：核心思想、关键技术细节、公式或算法流程

- **核心思想**：将睡眠EEG的频谱特征映射到二维状态空间，通过密度聚类、质心距离、速度等指标量化不同睡眠状态间的分离程度和稳定性。
- **关键步骤**：
  1. **EEG预处理**：滤波（0.5–40 Hz）、去除坏道和伪迹、平均参考；每夜数据统一裁剪为295分钟。
  2. **状态空间构建**：将EEG分为5秒 epochs，计算6个标准电极（F3,F4,C3,C4,O1,O2）的平均功率谱密度（Welch法，5秒汉明窗）。然后计算两个频谱比值：
     - Ratio1 = (8.6–19.3 Hz) / (1.0–10.9 Hz)
     - Ratio2 = (11.5–20.3 Hz) / (17.9–31.5 Hz)
   - 对时间序列用50点汉明窗平滑。取对数后，Ratio1作为x坐标，Ratio2作为y坐标。
  3. **稳定状态与不稳定性**：定义速度为相邻两epoch间的欧氏距离除以时间间隔。速度 < 0.01 为稳定状态（聚类），>0.01为不稳定状态（轨迹）。
  4. **聚类分析**：计算每个睡眠阶段（W、N1、N2、N3、R）稳定epochs的质心位置、质心间距离、峰-峰距离及重叠面积（通过一维和二维概率密度估计）。
  5. **过渡分析**：用二维概率密度将每个epoch分配到最可能的睡眠阶段，统计阶段间转换次数。
- **公式**：论文未给出完整数学公式，主要基于现有文献[20]的方法。

## 3. 实验设计：数据集、基准、对比方法

- **数据集**：14名健康年轻男性（21.9±3.0岁），来自先前已发表的交叉设计睡眠剥夺研究。
- **实验场景**：
  - 基线（BSL）：一周规律睡眠后实验室记录。
  - 慢性睡眠限制（CSR）：连续7晚每晚卧床5小时（第7晚记录）。
  - 急性睡眠剥夺（ASD）：40小时完全清醒后的恢复夜。
  - 洗脱期≥2周。
- **基准**：以BSL为对照，比较CSR和ASD。
- **对比方法**：本文未与其他方法对比，重点是SSA指标与常规睡眠评分参数的对比。但研究本身是对比两种剥夺条件。

## 4. 资源与算力

- 文中未提及任何GPU型号、数量、训练时长等信息。分析使用MATLAB R2018b，未涉及深度学习模型，因此算力要求较低，未说明具体计算资源。

## 5. 实验数量与充分性

- **实验组数**：14名受试者，每种条件（BSL, CSR, ASD）一个夜间记录，共42份记录。无额外消融实验或独立测试集。
- **统计分析**：使用Wilcoxon符号秩检验，Bonferroni校正多重比较（三条件两两比较）。分析包括常规睡眠参数、质心位置、距离、峰-峰距离、重叠面积、稳定epochs数量及比率、碎片化、过渡次数等。
- **充分性评价**：
  - 样本量较小（n=14），且仅限男性、年轻、健康人群，代表性有限。
  - 未进行交叉验证或独立验证，但作为探索性研究，结果可接受。
  - 未报道效应量和功效分析，统计力可能不足。
  - 比较条件差异时部分指标未达显著但趋势一致，结论需谨慎。

## 6. 论文的主要结论与发现

- CSR主要影响REM睡眠：REM质心在x方向上显著位移，与觉醒质心距离缩小，峰-峰距离减小、重叠面积增大，即REM与觉醒的频谱区分度降低。
- ASD主要影响NREM睡眠：N2和N3质心在y方向显著位移，N2与R质心距离缩小；但x方向N2/N3与R分离度增大，y方向减小，呈现频率特异性改变。
- 睡眠动力学：ASD后慢波睡眠（N3）稳定epochs数量比例显著增加，表明更稳定的慢波睡眠；CSR则未改变REM稳定性，仅因REM总量增加而绝对稳定epochs增多。
- 过渡：ASD后N2/N3与R之间的转换次数显著增多。
- 结论：SSA指标能反映ASD和CSR的不同效果，睡眠状态边界和动态具有状态依赖性，可能用于量化临床治疗反应。

## 7. 优点

- **方法新颖**：首次在同一健康受试者内比较两种睡眠剥夺方式对状态空间分析指标的影响。
- **多维量化**：SSA不仅提供睡眠阶段比例，还能量化状态间频谱相似性、稳定性和动态转换，补充传统睡眠分期。
- **临床潜力**：SSA可能区分生理与病理状态（如嗜睡症vs.慢性睡眠不足综合征）的边界改变，有助于鉴别诊断。
- **数据公开**：作者声明数据可根据合理请求提供。

## 8. 不足与局限

- **样本局限**：仅14名年轻健康男性，无法推广到女性、老年人或临床人群。
- **分析周期截断**：为保证可比性，将BSL和ASD夜统一截短为295分钟（即CSR夜时长），丢失了正常睡眠后期更多REM和觉醒片段的信息。
- **觉醒epochs极少**：睡眠剥夺条件下觉醒数量很少，涉及觉醒的分析结果需谨慎解读。
- **无独立验证**：探索性研究，未在独立数据集上验证；统计校正后部分结果仅趋势显著。
- **缺少与病理人群的直接对比**：虽然讨论中对比了嗜睡症，但未在相同数据中直接验证。
- **计算资源未报告**：虽然不影响结果，但降低了可复现性细节。

（完）
