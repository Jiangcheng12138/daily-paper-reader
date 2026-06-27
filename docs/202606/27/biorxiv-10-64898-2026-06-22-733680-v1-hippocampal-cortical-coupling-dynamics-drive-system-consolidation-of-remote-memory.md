---
title: Hippocampal-cortical coupling dynamics drive system consolidation of remote memory
title_zh: 海马-皮层耦合动力学驱动远程记忆的系统巩固
authors: "Sheng, T., Wang, S., Zhang, J., Xing, D., Wu, Y., Wang, Q., Lu, W."
date: 2026-06-26
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.22.733680v1.full.pdf"
tags: ["query:slp-ns"]
score: 9.0
evidence: NREM睡眠期间海马-皮层耦合驱动记忆巩固
tldr: 系统巩固将海马记忆转为皮层长期存储。本研究通过记录恐惧记忆形成中局部场电位和神经元活动，发现学习时海马快速伽马相对前额叶theta相位渐进偏移，巩固期在NREM睡眠尖波涟漪和皮层纺锤波事件中重现类似耦合。过程从海马驱动的伽马相干转变为前额叶介导的低频相干。闭环光遗传揭示耦合事件的因果链，证明海马-前额叶耦合相位偏移是记忆近期到远期转化的基质。
source: biorxiv
selection_source: fresh_fetch
motivation: 探究系统巩固中记忆从海马向皮层转移所依赖的海马-前额叶耦合动态及其因果机制。
method: 记录大鼠恐惧记忆形成和巩固中HPC-PFC场电位和单神经元活动，并实施闭环光遗传扰动。
result: 发现学习时HPC快速伽马相位相对PFC theta渐进偏移，NREM睡眠尖波涟漪和纺锤波事件重现此模式，并伴随HPC驱动到PFC驱动的耦合转换。
conclusion: HPC-PFC耦合相位偏移是记忆近期到远期转化的关键神经基质。
---

## 摘要
系统巩固将记忆的海马暂时性表征转化为皮层中的长期存储。然而，其潜在的神经基础仍不清楚。在这里，我们追踪了恐惧记忆形成过程中行为动物海马与皮层局部场电位和单神经元峰电位的时空演化。在学习过程中，海马快伽马相对于前额叶皮层θ振荡表现出渐进性相位偏移，伽马功率对齐于前额叶皮层θ周期中逐渐延迟的相位。引人注目的是，在后续巩固过程中，与海马尖波涟漪和非快速眼动睡眠期间短暂的前额叶皮层纺锤波事件相关联，一种相关的相位偏移耦合模式重新出现。在此过程中，区域间相互作用从近期阶段的海马驱动的皮层伽马一致性演变为远期阶段的前额叶皮层介导的皮层低频一致性。利用闭环光遗传扰动，我们证明了支持远程记忆形成的逐步因果耦合链。我们的研究揭示了海马-前额叶皮层耦合相位偏移是介导记忆近期到远期转化的可行基础。

## Abstract
System consolidation transforms temporary hippocampal representation of memory into long-term storage in cortex. The underlying neural substrate, however, remains enigmatic. Here, we tracked the spatiotemporal evolution of hippocampus (HPC)-cortex local field potentials and single-neuron spikes in behaving animals during fear memory formation. During learning, HPC fast gamma exhibited a progressive phase shift relative to PFC theta oscillations, with gamma power aligning to progressively later phases of the PFC theta cycle. Strikingly, a related phase-shifted coupling pattern re-emerged during subsequent consolidation in association with hippocampal sharp-wave ripples and transient PFC spindle events during NREM sleep. Across this process, interregional interactions evolved from HPC-driven cortical gamma coherence at recent stages to PFC-mediated cortical low-frequency coherence at remote stages. Using closed-loop optogenetic perturbations, we demonstrated a stepwise causal chain of coupling events underlying remote memory formation. Our study revealed HPC-PFC coupling phase shift as a feasible substrate mediating recent-to-remote transformation of memory.

---

## 论文详细总结（自动生成）

# 论文详细中文总结

## 1. 论文的核心问题与整体含义（研究动机和背景）

- **研究动机**：系统巩固是记忆处理的关键过程，记忆存储从海马转移到皮层。然而，系统巩固背后的神经基础（尤其是在远程记忆形成阶段的精细时空动态）仍不清楚。此前研究多关注早期巩固的突触和环路机制，对后期过程（尤其是远程记忆形成）的神经活动时空特征缺乏系统描述。
- **整体含义**：本文旨在揭示海马（HPC）与皮层（特别是前额叶皮层PFC、前扣带回ACC、后顶叶皮层PPC）之间振荡耦合动态如何驱动恐惧记忆从近期向远程的转化，并首次提供了因果证据。

## 2. 论文提出的方法论：核心思想、关键技术细节、算法流程

- **核心思想**：利用多通道电极同时记录多个脑区的局部场电位（LFP）和单神经元峰电位，追踪恐惧条件化过程中及后续28天内HPC-皮层耦合动态的时空演化；并通过闭环光遗传技术因果性地检验特定耦合事件的作用。
- **关键技术细节**：
  - **多通道植入式电极阵列**：自主设计的3D打印多驱动系统，可同时记录HPC、PFC、ACC、PPC的LFP和spike。使用铂铱微丝（grid或tetrode），阻抗控制在800 kΩ以下。
  - **行为范式**：大鼠痕迹恐惧条件化（trace fear conditioning），CS为2kHz正弦音，US为足底电击，CS和US间隔18秒痕迹期。对照组仅CS或仅US。
  - **信号分析**：
    - **相位-幅度耦合（PAC）**：使用调制指数（MI）衡量HPC快伽马（60-90 Hz）功率与PFC θ相位（4-12 Hz）之间的耦合强度。
    - **相位偏移（PAS）**：通过圆-线性回归计算PAC偏好相位随条件化试次或巩固天数的斜率，量化“相位幅度偏移”。
    - **相干性分析**：采用多窗口法计算HPC与皮层之间、皮层之间的γ或低频相干性。
    - **方向性分析**：包括尖峰-尖峰互相关、尖峰-LFP相位一致性、格兰杰因果指数（GCI）以及基于图论的枢纽中心度。
  - **闭环光遗传干预**：
    - **低频相位扰动**：在巩固期（day4-21）随机给予4-12 Hz光脉冲干扰PFC低频节律。
    - **基于相干性的闭环抑制**：实时计算HPC与皮层之间的γ相干性，当超过阈值时触发抑制HPC神经元的光遗传刺激。
    - **基于尖波涟漪（SWR）的闭环抑制**：实时检测SWR，触发抑制HPC神经元。
    - **基于低频相干性的闭环抑制**：在远程阶段抑制PFC神经元以干扰皮层间低频相干。
- **算法流程（文字说明）**：
  1. LFP信号被带通滤波提取θ、慢γ、快γ振荡。
  2. 用希尔伯特变换获得瞬时相位和幅值。
  3. 计算PAC的MI值，并通过循环移位（1-30秒）构建零假设分布检验显著性。
  4. 对每个试次/天的PAC偏好相位进行圆-线性回归，得到PAS斜率。
  5. 相干性计算采用多窗口傅里叶变换，在SWR后1秒窗内分析。
  6. 闭环系统：实时400ms窗口傅里叶变换，计算相干性，当超过50%通道对相干性超过均值+3标准差时触发400ms光刺激。

## 3. 实验设计：数据集、场景、benchmark、对比方法

- **数据集/场景**：
  - 采用大鼠痕迹恐惧条件化范式，在训练箱中进行条件化，随后在家庭笼中进行1、2、4、7、11、14、16、21、28天纵向记录（home cage）。行为状态通过EEG、EMG、呼吸、心率、视频监控分类为清醒、NREM、REM。
  - 主要比较组：CS-US组（条件化+足底电击，n=8只），CS only组（仅条件化刺激，n=6），Shock only组（仅电击，n=4）。
- **Benchmark**：没有外部benchmark，本研究属于基础神经科学，主要与自身基线（pre-FC或day -1）和对照组比较。
- **对比方法**：
  - 分析了HPC与三个皮层（PFC、ACC、PPC）之间的PAC和相干性，发现PAS仅存在于HPC-PFC回路，HPC-ACC虽也有PAC但无偏移。
  - 比较了CS-US组与CS only组、Shock only组的差异。
  - 在巩固期比较了SWR+与SWR−窗内耦合的差异。
  - 药物实验（CNQX注入HPC或PFC）检验了枢纽作用。
  - 闭环光遗传实验（随机低频相位干预、γ相干抑制、低频相干抑制、SWR抑制）提供了因果证据。

## 4. 资源与算力

- **文中未明确说明GPU型号、数量、训练时长**。所有数据采集使用Plexon OmniPlex-64系统，实时闭环控制使用MATLAB（2014b）和NI-DAQ，GPU并行计算加速实时相干分析，但未提及具体GPU信息。
- 光遗传使用561 nm（eNpHR）或473 nm激光，功率约10 mW/mm²。

## 5. 实验数量与充分性

- **主要实验数量**：
  - **行为/电生理**：CS-US组n=8，CS only组n=6，Shock only组n=4。
  - **单单元分析**：共记录数百个HPC神经元（如46个相位锁定到PFC θ的单元，104个未锁定；巩固期51个单元中34.2%锁定）。
  - **闭环光遗传**：
    - 低频相位干预：n=5（干预组） vs n=5（对照组）。
    - 基于γ相干性的HPC抑制：n=5 vs n=5。
    - 基于低频相干性的PFC抑制：n=4 vs n=4。
    - SWR抑制实验：n=4（图S15）。
    - 延迟干预对照、随机干预对照均进行。
  - **药物实验**：CNQX注入HPC或PFC，n=3只/组。
- **充分性评价**：
  - 实验设计较全面：包含多个对照组（CS only、Shock only、预条件化基线）、多种分析方法（PAC、相干、方向性、图论）、多个时间点（0-28天）、多种行为状态（清醒、NREM、REM）、多种因果干预（光遗传、药理）。
  - 消融实验充分：如闭环抑制γ相干后，后续PAS和低频相干均消失；抑制PAS后，枢纽转换和方向性转换均失败。
  - 统计方法严谨：使用双尾t检验、ANOVA、Bonferroni校正、圆-线性回归、置换检验等。
  - 客观性：实验者采用自动睡眠分期、冷冻行为自动分析，但手动验证；数据分析有盲法（如睡眠评分者不知实验条件）。
  - 不足之处：单单元长期追踪困难，导致无法直接比较编码和巩固期的同一神经元；样本量适中（每组4-8只），某些组（如药物实验n=3）偏小。

## 6. 论文的主要结论与发现

- **发现1（PAS）**：在条件化过程中，HPC快伽马（60-90 Hz）的功率相对于PFC θ相位逐渐向“更晚”的相位偏移，称相位-幅度偏移（PAS）。该现象仅存在于HPC-PFC回路，与学习性能正相关。
- **发现2（PAS在巩固期重现）**：在巩固期（day4-21）的NREM睡眠中，与SWR相关的短暂PFC低频活动（类似于纺锤波）上，PAS模式重现，且偏移幅度与编码期相似。其强度与远程记忆保留正相关。
- **发现3（HPC-皮层γ相干先于PAS）**：在近期记忆阶段（day0-7），SWR后1秒窗内HPC与三个皮层区域出现快γ相干性增强，HPC为主要驱动者。
- **发现4（皮层间低频相干继于PAS之后）**：在远程阶段（day14-28），SWR后PFC与ACC、PPC之间出现低频相干性增强，PFC成为枢纽，方向性从HPC→PFC转为PFC→ACC/PPC。
- **发现5（因果链）**：
  - 闭环抑制SWR减少PAS重现。
  - 闭环抑制HPC-皮层γ相干（day3-7）消除后续PAS和皮层间低频相干，并损害远程记忆。
  - 随机扰动PFC低频相位（day4-21）破坏PAS，阻止枢纽转换和方向性转换，损害远程记忆。
  - 闭环抑制PFC低频相干（day14-21）破坏皮层间相干并损害远程记忆稳定。
- **总结**：系统巩固由一系列“接力式”耦合事件组成：编码期PAS → 近期HPC驱动的γ相干 → 巩固期PAS重现（伴随SWR-纺锤波耦合） → 远程PFC驱动的低频相干。PAS是连接近期-远程记忆转化的关键基质。

## 7. 优点

- **方法创新**：
  - 自主设计3D打印多通道电极，实现4个脑区同步LFP和spike记录。
  - 开发了基于实时相干性的闭环光遗传干预系统（延迟20-40 ms），可靶向特定频段的区域间耦合。
  - 首次在系统巩固中记录了长达28天的连续神经动态，覆盖多个时间尺度。
- **实验设计严谨**：
  - 多模态监测（EEG、EMG、呼吸、心率、视频）确保行为状态准确分类，排除运动、呼吸等混淆因素。
  - 多重对照组（CS仅、US仅、基线）和多种干扰方式（光遗传、药理学）提供因果证据。
  - 全面分析多种耦合指标（PAC、相干、方向性、图论枢纽），从多个角度验证结论。
- **发现新颖**：
  - 首次描述PAS现象及其在编码和巩固期的重现，且与已有θ相位预留给构不同（是相位幅度偏移而非尖峰偏移）。
  - 揭示了系统巩固中HPC和PFC交替主导的时间序列，并提出“接力式”耦合链模型。

## 8. 不足与局限

- **机制层面**：PAS的细胞和环路机制未解明（如参与神经元类型、突触可塑性变化等），虽然观察到与SWR和spindle相关，但PAS的具体信息内容（是否携带重放序列）未知。
- **技术限制**：
  - 无法长期稳定追踪单个神经元（电极漂移），因此编码期和巩固期无法直接比较同一细胞的spike偏好相位变化。
  - 记录仅限于背侧CA1和几个皮层区，未涉及腹侧HPC、丘脑、内嗅皮层等可能与系统巩固相关的区域。
- **实验局限性**：
  - 样本量中等（每组4-8只），尤其是药物实验组（n=3）统计效力较低。
  - 仅使用雄性Sprague-Dawley大鼠，性别和种系普遍性未知。
  - 行为范式仅为痕迹恐惧条件化，对空间记忆或其他类型记忆的普适性未验证。
- **潜在的混淆因素**：
  - 光遗传抑制可能引起非特异性效应（如诱发癫痫样活动），虽通过排除异常事件（振幅>2 mV）减轻，但未完全排除。
  - 闭环延迟20-40 ms，可能错过部分耦合事件。
- **结论推广性**：PAS在人类中是否存在尚未验证；系统巩固是否依赖完全相同的耦合序列仍需跨物种研究。

（完）
