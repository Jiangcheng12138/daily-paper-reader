---
title: Drowsiness alters the neural dynamics but not the core computations of multisensory integration
title_zh: 困倦改变了多感觉整合的神经动力学而非核心计算
authors: "Alameda, C., Avancini, C., Sanabria, D., Bekinschtein, T. A., Ciria, L. F."
date: 2026-06-25
pdf: "https://www.biorxiv.org/content/10.64898/2026.01.12.699055v2.full.pdf"
tags: ["query:slp-ns"]
score: 8.0
evidence: 研究困倦与清醒转换期间的神经动态
tldr: 警觉性波动影响感知行为，但对多感觉整合的影响未知。本研究采用听觉-触觉检测任务结合脑电图，追踪自发警觉性下降。结果发现，行为上多感觉刺激仍促进反应，但事件相关电位减弱；多变量解码显示神经表征保留但时间稳定性降低，跨警觉水平泛化表明核心计算不变。揭示了多感觉整合在困倦时功能保留但动态改变，维持适应性行为。
source: biorxiv
selection_source: fresh_fetch
motivation: 探究从清醒到困倦过程中，多感觉整合的神经机制是否发生变化。
method: 被试执行听觉-触觉检测任务，同时记录脑电图分析警觉性波动对多感觉整合的影响。
result: 行为上多感觉整合仍促进反应，神经事件相关电位减弱，但解码显示表征保留且稳定性降低。
conclusion: 多感觉整合在困倦时保留核心计算，但神经动态发生改变。
---

## 摘要
警觉性的波动塑造了感知和行为，但它是如何影响大脑跨感官整合信息的能力仍然知之甚少。本研究探讨了当人类从清醒过渡到睡眠时，多感觉整合是否得以保留。参与者（18名女性，8名男性）在执行听觉-触觉检测任务的同时，脑电图跟踪了警觉性的自发下降。行为上，尽管反应变慢且遗漏增加，多感觉刺激在困倦期间仍能促进反应。尽管竞赛模型预测与保留的多感觉整合证据一致，但多感觉相互作用的事件相关特征在困倦期间减弱或不再可检测。关键在于，多变量解码表明多感觉神经表征仍然可检测，尽管时间稳定性降低，并且早期跨状态泛化揭示了不同警觉水平之间共享的表征结构，表明核心多感觉计算得以保留。这些发现表明，随着警觉性下降，多感觉整合仍然保持功能，但动态改变，揭示了大脑在清醒-睡眠过渡期间如何维持适应性行为。

## Abstract
Fluctuations in alertness shape perception and behaviour, yet how they affect the ability of our brain to integrate information across senses remains poorly understood. Here we investigated whether multisensory integration is preserved as humans transition from wakefulness to sleep. Participants (18 females, 8 males) performed an audiotactile detection task while electroencephalography tracked spontaneous declines in alertness. Behaviourally, multisensory stimulation continued to facilitate responses during drowsiness, despite slowing and increased omissions. Although race-model predictions were consistent with preserved evidence for multisensory integration, event-related signatures of multisensory interactions were attenuated or no longer detectable during drowsiness. Crucially, multivariate decoding showed that multisensory neural representations remained detectable, although less temporally stable, and early cross-state generalization revealed shared representational structure across alertness levels, indicating preserved core multisensory computations. These findings show that multisensory integration remains functional but dynamically altered as alertness declines, revealing how the brain maintains adaptive behaviour during the wake-to-sleep transition.

---

## 论文详细总结（自动生成）

### 1. 论文的核心问题与整体含义（研究动机和背景）
- **核心问题**：警觉性波动（如困倦）如何影响大脑跨感官整合信息的能力？多感觉整合这一基本过程在从清醒到睡眠的过渡中是否得以保留？
- **研究动机**：日常生活和临床场景（如夜班医生）中，困倦会减慢反应、增加疏忽，但多感觉整合（如同时听到蜂鸣和振动）是否能补偿这种衰退尚不清楚。已有研究多基于单感官范式，缺乏对多感觉整合在警觉性下降时的全面刻画。
- **整体含义**：揭示大脑在警觉性自然下降时如何维持适应性行为，为理解睡眠过渡期的认知弹性提供证据，并为疲劳驾驶、临床监控等实际场景提供理论参考。

---

### 2. 论文提出的方法论：核心思想、关键技术细节
- **核心思想**：通过听觉-触觉检测任务结合EEG，在单试次水平上分类警觉状态（清醒 vs. 困倦），比较多感觉整合的行为、计算和神经指标是否随警觉性变化。
- **关键技术细节**：
  - **警觉性分类**：基于试次前2秒的EEG theta/alpha功率比值（中枢—枕区），采用百分位法（最高33%为困倦，最低33%为清醒），并加入时序平滑（≥10连续试次）和块起始前100试次强制标记为清醒。
  - **行为分析**：线性混合效应模型分析反应时（RT）和响应率，固定因素为警觉状态、刺激类型、侧别。
  - **竞赛模型**：计算Grice界（多感觉CDF与最快单感觉CDF之间的面积）和Miller界违例（多感觉CDF超出单感觉概率和），检验多感觉整合是否超出统计易化。
  - **ERP分析**：基于加性模型，将多感觉ERP与单感觉（听觉+触觉）求和ERP比较，通过团块置换检验识别超加性（早期）和亚加性（晚期）差异。
  - **MVPA**：使用线性判别分析（LDA）对多感觉 vs. 单感觉求和进行解码，计算时间泛化矩阵（TGM）和跨状态泛化（清醒→困倦，困倦→清醒）。

---

### 3. 实验设计：数据集/场景、基准、对比方法
- **数据集/场景**：
  - 26名健康参与者（18女，8男，年龄18–32岁），Epworth嗜睡量表得分7–14（轻度嗜睡倾向）。
  - 刺激：30ms白噪声（听觉）、30ms 100Hz振动（触觉）、同时同侧的听觉-触觉对；左右各6种条件（共12种）；1980试次随机呈现。
  - 实验流程：交替进行短警觉块（240试次，~15min）和长困倦块（750试次，~45min），共2个循环；困倦块允许入睡，无反应则唤醒；块间有短暂休息。
- **基准**：无外部基准，采用自身对照（清醒 vs. 困倦）。对照分析包括：试次历史效应、全局RT减慢、单感觉反应变化对竞赛模型的影响。
- **对比方法**：未与其他算法或模型对比，主要比较清醒与困倦条件下的行为、计算和神经指标。

---

### 4. 资源与算力
- **明确说明**：论文中未提及使用的GPU型号、数量或训练时长。
- **软件环境**：MATLAB（Psychtoolbox）、EEGLAB、FieldTrip、R（lme4包）等；使用自定义硬件（CRAT）保证毫秒级同步。
- **算力需求**：由于分析涉及单试次EEG分类、置换检验和MVPA，推测需要中等计算资源（如多核CPU或简单GPU），但具体信息缺失。

---

### 5. 实验数量与充分性
- **主要实验**：
  - **行为分析**：线性混合效应模型（RT、响应率），含主效应和交互作用，Bonferroni校正post-hoc。
  - **竞赛模型**：两组配对检验（Grice界t检验、Miller界违例Wilcoxon检验），Bonferroni校正（α=0.025）。
  - **ERP分析**：全时间窗口0–500ms团块置换检验（5000次置换），比较清醒 vs. 困倦的多感觉-求和差异。
  - **MVPA**：LDA解码与时间泛化，跨状态泛化，均为置换检验。
- **附加控制分析**：试次历史效应、日志RT变换、不同块上下文中的清醒试次比较、去周期成分的alpha谱校正等（见补充材料）。
- **充分性评价**：实验设计严谨，涵盖了行为、计算、神经三个层面，且进行了多组控制分析确保结果稳健。样本量26人（大于多数类似研究的20–25人），试次数充足（清醒约790试次/人，困倦约563试次/人）。实验客观公平，预注册（OSF）、数据公开。
- **不足**：仅有一种实验任务（检测任务），未涉及判别或估计任务；警觉性分类采用离散阈值，可能忽略连续过渡中的细微差异。

---

### 6. 论文的主要结论与发现
1. **行为层面**：困倦时反应显著变慢、漏报增加，但多感觉冗余效应（RSE）仍存在（多感觉刺激快于单感觉），且未与清醒状态有显著交互。
2. **计算层面**：Miller界违例（多感觉整合标志）在清醒和困倦中均显著大于零，且两者无显著差异，表明核心整合计算保留。
3. **神经层面**：
   - **ERP**：清醒时早期超加性（<150ms）和晚期亚加性（200–500ms）均显著；困倦时早期超加性消失，晚期亚加性延迟约100ms且幅度减小；直接比较仅晚期差异显著。
   - **MVPA**：清醒和困倦均能解码多感觉 vs. 单感觉求和，但困倦时解码稳定性降低；跨状态泛化显示早期（~100–500ms）共享神经表征结构。
4. **总体结论**：多感觉整合的功能（行为收益和核心计算）在困倦时保留，但其神经动态（ERP幅度和时间稳定性）发生改变，表现为延迟和减弱，但并非完全丧失。这表明大脑通过灵活调整神经机制维持适应行为。

---

### 7. 优点
- **方法创新**：首次结合单试次EEG警觉性分类、竞赛模型、ERP和MVPA系统研究困倦对多感觉整合的影响。
- **全面分析**：跨越行为、计算和神经多个层次，且包含跨状态泛化，揭示共享表征。
- **实验控制**：通过块间休息、单试次分类、试次历史效应分析等控制混淆变量；采用日志转换检验结果稳健性。
- **预注册与开放科学**：实验方案、数据、代码均公开，提升可重复性。
- **实际意义**：结果直接关联疲劳驾驶、夜班工作、临床监护等场景，为多感觉预警信号设计提供理论基础。

---

### 8. 不足与局限
- **样本与生态效度**：仅26名健康年轻人，且实验在昏暗房间进行，未能反映真实世界复杂性（如移动、干扰）。
- **警觉性分类的局限性**：百分位阈值忽略连续动态，可能混入中间状态；单试次分类基于theta/alpha比，未考虑睡眠纺锤或慢波等更深睡眠标志。
- **神经指标差异不显著**：早期ERP直接比较未通过统计阈值，可能因被试间变异大或信噪比低，限制结论强度。
- **任务特异性**：仅使用检测任务（简单反应），未评估更复杂的多感觉整合（如辨别、估计或冲突解决），结果可推广性存疑。
- **机制解释风险**：晚期亚加性可能混杂运动准备等非感官过程，加性模型本身有争议；竞赛模型假设独立通道，实际可能存在串扰。
- **算力信息缺失**：未提供具体计算资源，不利于复现时估计需求。

（完）
