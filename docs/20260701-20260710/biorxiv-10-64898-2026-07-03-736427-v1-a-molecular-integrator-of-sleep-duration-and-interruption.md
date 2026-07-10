---
title: A molecular integrator of sleep duration and interruption
title_zh: 睡眠时长与中断的分子整合器
authors: "Tilden, E. I., Fontenele, A. J., Goggans, K. M., Ma, S., Gorecki, D., Berriman-Rozen, Z. D., Oldenborg, A., Shew, W. L., Chen, Y."
date: 2026-07-08
pdf: "https://www.biorxiv.org/content/10.64898/2026.07.03.736427v1.full.pdf"
tags: ["query:slp-ns"]
score: 9.0
evidence: 编码单次睡眠时长和中断的分子机制
tldr: 睡眠调节涉及秒到小时的多时间尺度，但缺乏在单个睡眠回合内追踪睡眠历史的信号。本研究通过实时测量自由活动小鼠的蛋白激酶A底物磷酸化（PKA-SP），发现膜PKA-SP在每个睡眠回合中呈指数下降，动力学一致，整合睡眠时长和中断，并连续预测觉醒概率。该分子信号编码了睡眠回合内的历史信息，揭示了生化动力学如何桥接快速觉醒回路与慢速睡眠稳态。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-03-736427-v1/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1476, \"height\": 1742, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-03-736427-v1/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1723, \"height\": 1729, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-03-736427-v1/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1704, \"height\": 1294, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-03-736427-v1/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1836, \"height\": 1120, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-03-736427-v1/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1507, \"height\": 1725, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-03-736427-v1/fig-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 1236, \"height\": 1680, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-03-736427-v1/fig-007.webp\", \"caption\": \"\", \"page\": 0, \"index\": 7, \"width\": 1676, \"height\": 1739, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-03-736427-v1/fig-008.webp\", \"caption\": \"\", \"page\": 0, \"index\": 8, \"width\": 1553, \"height\": 1686, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-03-736427-v1/fig-009.webp\", \"caption\": \"\", \"page\": 0, \"index\": 9, \"width\": 1427, \"height\": 1236, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-03-736427-v1/fig-010.webp\", \"caption\": \"\", \"page\": 0, \"index\": 10, \"width\": 1505, \"height\": 1724, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-03-736427-v1/fig-011.webp\", \"caption\": \"\", \"page\": 0, \"index\": 11, \"width\": 1189, \"height\": 810, \"label\": \"Figure\"}]"
motivation: 睡眠调节涉及多时间尺度，但尚无信号能在单个睡眠回合内编码睡眠历史，故需探索下游生化信号的慢动力学作为潜在编码器。
method: 实时测量自由活动小鼠的PKA底物磷酸化（PKA-SP）水平，分析其在不同睡眠回合中的动态变化。
result: 膜PKA-SP在每个睡眠回合指数下降，动力学一致；整合睡眠时长与中断，连续预测清醒概率；睡眠剥夺后末端水平更低，与睡眠需求消散相关。
conclusion: 发现编码睡眠回合历史的分子信号，揭示生化动力学连接快速觉醒回路与慢速睡眠稳态机制。
---

## 摘要
睡眠在多个时间尺度上受到调控。睡眠与觉醒之间的转换在几秒内发生；单个睡眠片段持续数分钟到数小时；而稳态睡眠需求传统上是在多个睡眠片段中进行追踪。快速的睡眠到觉醒转换由已识别的神经元、回路和神经调节物驱动，而慢波活动则与数小时内的睡眠需求相关。然而，目前尚未有信号被证明能在单个睡眠片段内编码睡眠历史——这是大脑必须持续监测已发生睡眠量以及任何给定时刻唤醒可能性的时间尺度。睡眠/觉醒相关神经调节物下游的生化信号表现出比神经调节物本身更慢的动力学特性，使其成为片段内睡眠历史候选编码器。本文通过在自由行为的小鼠中实时测量蛋白激酶A底物磷酸化(PKA-SP)，显示膜PKA-SP在每个睡眠片段内呈指数下降，且动力学在不同片段间一致，整合了睡眠时长和睡眠中断，并持续预测逐时的觉醒概率。在睡眠剥夺后，PKA-SP在睡眠片段结束时达到更低水平，与增加的睡眠需求耗散相关。这些发现识别出一个编码片段内睡眠历史的分子信号，揭示了生化动力学如何连接快速觉醒回路与经典睡眠稳态的慢时间尺度。

## Abstract
Sleep is regulated across multiple timescales. Transitions between sleep and wake happen within seconds; individual sleep bouts last minutes to hours; and homeostatic sleep need has classically been tracked across multiple bouts. Rapid sleep-to-wake transitions are driven by identified neurons, circuits, and neuromodulators, while slow wave activity correlates with sleep need across hours. However, no signal has been shown to encode sleep history within individual sleep bouts, the timescale at which the brain must continuously monitor how much sleep has occurred and how likely waking is at any given moment. Biochemical signals downstream of sleep/wake-associated neuromodulators display slower dynamics than the neuromodulators themselves, making them candidate encoders of within-bout sleep history. Here, by measuring protein kinase A substrate phosphorylation (PKA-SP) in real time in freely behaving mice, we show that membrane PKA-SP decreases exponentially within each sleep bout with consistent kinetics across bouts, integrates sleep duration and sleep interruption, and continuously forecasts moment-to-moment waking probability. Following sleep deprivation, PKA-SP reaches lower levels at the end of sleep bouts, correlating with increased sleep need dissipation. These findings identify a molecular signal encoding within-bout sleep history, revealing how biochemical dynamics bridge fast arousal circuits and the slow timescale of classical sleep homeostasis.

---

## 论文详细总结（自动生成）

### 1. 论文的核心问题与整体含义（研究动机和背景）

睡眠调节涉及多个时间尺度：秒级的睡眠-觉醒转换、分钟到小时的睡眠片段、以及跨片段的稳态睡眠需求。尽管已发现驱动快速转换的神经元和回路，以及慢波活动（SWA）与数小时睡眠需求相关，但**尚无信号被证明能在单个睡眠片段（bout）内部追踪已发生的睡眠时长和当前觉醒概率**。作者假设，睡眠/觉醒相关神经调质（如去甲肾上腺素、5-羟色胺）下游的生化信号（如蛋白激酶A底物磷酸化，PKA-SP）具有较慢的动力学，可能作为片段内睡眠历史的编码器。该研究旨在发现首个在体分子信号，整合睡眠时长和中断，连续预测觉醒概率，从而桥接快速觉醒回路与慢速睡眠稳态。

### 2. 论文提出的方法论：核心思想、关键技术细节、公式或算法流程

**核心思想**：利用荧光寿命光度法（FLiP）实时测量自由活动小鼠特定脑区（海马CA1、前额叶皮层mPFC、运动皮层M1、视觉皮层V1）兴奋性神经元中PKA-SP的动态变化。特别地，**膜定位的PKA-SP（FLIM-AKARm）** 呈现与胞内PKA-SP不同的睡眠-觉醒相关动力学，是本研究的主要对象。

**关键技术细节**：
- **传感器**：使用Cre依赖的FLIM-AKAR（胞内）或FLIM-AKARm（膜靶向）病毒载体（AAV1-FLEX），在Tg(CamKIIα-Cre)小鼠中表达。
- **同时记录**：1 Hz FLiP + 400 Hz EEG/EMG + 25 fps视频，持续24-48小时，自动睡眠分期（NREM、REM、微觉醒、觉醒）。
- **数学建模**：将膜PKA-SP动力学建模为三个状态（下降相、上升相、稳态）。下降相和上升相用指数方程描述：
  \[
  B(t) = (1 - \frac{1}{\tau}) B(t-1) + \frac{B^*}{\tau}
  \]
  其中 \(\tau\) 为时间常数，\(B^*\) 为渐近值。参数通过滑动窗口拟合、贝叶斯信息准则（BIC）优化，并发现参数在两天内稳定。
- **概率预测**：采用Cox比例风险模型（含时变协变量：PKA-SP、微觉醒计数、昼夜节律时间）评估PKA-SP对瞬间觉醒概率的预测能力；逻辑回归模型比较PKA-SP与睡眠时长的预测效力。

### 3. 实验设计：使用了哪些数据集/场景，benchmark是什么，对比了哪些方法

**数据集/场景**：
- **基线记录**：24-48小时自由行为小鼠（n=15只）的FLiP + EEG/EMG数据，涵盖多个脑区（海马CA1、mPFC、M1、V1）。
- **对照实验**：
  - 非磷酸化突变体FLIM-AKAR T391A（对照PKA特异性）。
  - 表达PKA抑制肽PKI（验证信号特异性）。
  - 光激活腺苷酸环化酶biPAC刺激（排除传感器天花板效应）。
  - 毒蕈碱受体拮抗剂东莨菪碱注射（验证动力学上限）。
  - 声音诱发觉醒实验（证明PKA-SP响应觉醒转换而非听觉输入）。
  - 药理阻断实验（去甲肾上腺素β受体拮抗剂普萘洛尔、5-HT2A拮抗剂MDL100907、α受体拮抗剂哌唑嗪、腺苷受体拮抗剂DPCPX、毒蕈碱受体拮抗剂东莨菪碱）以探究上游调节物。
  - **睡眠剥夺实验**：4小时新异物体干预（ZT0-ZT4），比较与 circadian匹配基线的差异。

**benchmark**：
- **慢波活动（SWA）**：作为经典睡眠需求指标，与膜PKA-SP在片段内变化进行对比。
- **随机打乱数据（shuffled）**：作为验证预测特异性的零假设。

**对比方法**：
- 线性模型 vs 指数模型（通过BIC比较拟合优度）。
- 包含/不包含微觉醒计数、包含/不包含昼夜节律时间的Cox模型比较。
- 逻辑回归中睡眠时长 vs PKA-SP的预测能力比较。

### 4. 资源与算力

论文中**未明确说明**使用的GPU型号、数量或训练时长。所有分析基于Python和R在标准工作站上完成，未提及大规模并行计算。主要的计算负载在于指数模型参数优化（局部L-BFGS-B优化）、Cox模型拟合等，属于中等计算量，未使用深度学习或大规模GPU集群。

### 5. 实验数量与充分性

**主要实验组数**：
- 基线记录：n=15只小鼠（mPFC），共21次实验；其他脑区各n=3。
- 突变体/对照：FLIM-AKAR T391A n=4；PKI n=4。
- 药理阻断：每组n=4~7只（普萘洛尔n=7、MDL100907 n=4、DPCPX n=5、东莨菪碱n=5、哌唑嗪n=5）。
- 声音试验：n=3。
- 睡眠剥夺：n=6（自身对照，前一天作为baseline）。

**充分性**：
- 实验设计较为全面：包含多种对照（突变、抑制、打乱、天花板测试）、多种干预（药理、睡眠剥夺、声音）、多脑区验证。
- **公平性**：主要统计采用非参数检验（Wilcoxon signed-rank、paired t-test等），层级分析控制个体差异（每只动物先聚合到稳健均值）。Cox模型含随机效应和昼夜节律协变量，逻辑回归有固定效应（个体和ZT bin）。对照shuffled数据排除了假阳性。
- **局限**：样本量较小（尤其多脑区每组仅3只），但主要结论（mPFC）基于15只，尚可接受。部分药理实验未报告完整统计细节（仅在补充图中给出定性结论）。睡眠剥夺实验仅有6只。

### 6. 论文的主要结论与发现

- **膜PKA-SP在睡眠片段内呈指数下降**，下降时间常数约212秒，上升（觉醒/微觉醒）约19秒，**参数在两天内稳定**，可准确拟合全时段数据（R²中位数0.97）。
- **膜PKA-SP整合睡眠时长和微觉醒中断**：微觉醒导致PKA-SP短暂上升，从而区分相同睡眠时长但不同中断史的状态，比单独睡眠时长更准确地预测觉醒概率。
- **膜PKA-SP连续预测觉醒概率**：Cox模型显示，每个标准差增加的膜PKA-SP对应瞬间觉醒概率降低19.9%，该效应独立于昼夜节律和睡眠时长。
- **高睡眠需求（睡眠剥夺后）** 使每个睡眠片段末端PKA-SP相对于觉醒水平下降更多，表明膜PKA-SP追踪**片段内睡眠需求的相对耗散**，而非绝对需求水平。
- 膜PKA-SP动力学在多个皮质-海马区域（海马、mPFC、M1、V1）**一致**，符合睡眠调节的全局性。
- 上游由**去甲肾上腺素和5-羟色胺**（而非腺苷或乙酰胆碱）调节。
- EEG功率变化**先于**膜PKA-SP变化，表明PKA-SP是状态转换的下游结果而非驱动因素。

### 7. 优点：方法或实验设计上的亮点

- **技术创新**：利用FLiP实现自由活动小鼠中毫秒级精度的PKA-SP实时测量，首次在体解析睡眠片段内的生化动力学。
- **多层次验证**：从突变传感器（T391A）、PKI抑制、刺激（biPAC）到药理和睡眠剥夺，建立了因果性与特异性证据链。
- **数学模型**：基于指数动力学的三状态模型简洁且准确，参数稳定，具有预测力。
- **统计分析严谨**：采用层级分析、稳健估计、Cox比例风险模型（含时变协变量和随机效应），排除混杂变量（昼夜节律、睡眠时长、个体差异）。
- **多脑区比较**：证实膜PKA-SP动力学在全脑兴奋性神经元中一致，增强了结论的普适性。
- **与经典理论衔接**：提出膜PKA-SP作为片段级睡眠需求耗散的分子底物，补充了SWA在长时程表征方面的不足。

### 8. 不足与局限

- **因果关系未确立**：论文明确承认，膜PKA-SP是否**驱动**睡眠需求耗散尚未证明。仅通过PKI抑制PKA间接支持，缺乏闭环实时扰动实验。
- **样本量偏小**：部分实验（多脑区、声音、药理）仅3-4只小鼠，统计效力有限。睡眠剥夺实验仅6只。
- **缺乏女性小鼠单独分析**：虽然使用了26只雄性和16只雌性，但未检验性别差异对主要结果的影响。
- **技术局限**：FLiP仅测量单一脑区的群体平均PKA-SP，无法区分细胞类型特异性或亚细胞精确定位；纤维记录的空间分辨率较低。
- **外推限制**：实验仅在小鼠中进行，结论向人类睡眠的转化尚待验证。光周期固定12:12，未在暗期或自由运行条件下验证。
- **部分分析依赖于手动定义阈值**：微觉醒时长阈值（默认12-44秒）对结果影响较大，虽进行了敏感性分析，但缺乏生理依据。
- **开放数据与复现**：论文声明数据可提供，但未附完整开放数据集或独立验证。
- **模型假设**：指数模型假定固定的上升/下降时间常数，但个体间存在适度变异（IQR较宽），且REM睡眠期间斜率略有不同，可能生物学意义不明确。

（完）
