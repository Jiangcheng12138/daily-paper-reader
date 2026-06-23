---
title: Functional MRI signals at and beyond 1 Hz are coupled to brain states and predict spontaneous neural activity
title_zh: 1 Hz及以上的功能磁共振成像信号与脑状态耦合并预测自发神经活动
authors: "Jacob, L. P. L., Bailes, S. M., Williams, S. D., Stringer, C., Rosen, B. R., Polimeni, J. R., Lewis, L. D."
date: 2026-06-22
pdf: "https://www.biorxiv.org/content/10.1101/2025.10.13.681720v2.full.pdf"
tags: ["query:slp-ns"]
score: 8.0
evidence: 快速fMRI与EEG在睡眠-觉醒转换中的应用
tldr: 快速fMRI可毫秒级全脑成像，但其高频信号与自发神经活动的关系尚不明确。本研究结合快速fMRI（TR=378ms）与同步EEG，分析27名受试者在睡眠与清醒间的高频fMRI信号。发现NREM睡眠时高频fMRI功率（高达1.3 Hz）显著增加，且与EEG alpha和delta节律相关。机器学习可从高频fMRI信号解码EEG功率。结果揭示高频fMRI信号反映动态脑状态，可作为推断自发神经活动的有效工具。
source: biorxiv
selection_source: fresh_fetch
motivation: "探索快速fMRI中高频信号（>1 Hz）与自发神经活动及警觉状态的关系。"
method: 使用快速fMRI（TR=378ms）和同步EEG记录27名受试者在睡眠与清醒间的脑活动，分析高频fMRI功率与EEG节律的时空相关性，并训练机器学习模型解码EEG功率。
result: NREM睡眠时高频fMRI功率（高达1.3 Hz）上升；高频fMRI功率与alpha和delta节律显著相关；跨个体测试中可解码EEG alpha和delta功率。
conclusion: 高频fMRI信号含有神经耦合信息，能够动态追踪脑状态并预测自发神经活动，为快速fMRI的应用提供神经基础。
---

## 摘要
技术进步使得高时间分辨率的fMRI采集成为可能，能够在短短几百毫秒内实现全脑成像。然而，快速血流动力学信号与静息态下的自发神经活动之间的关系尚不明确，这限制了我们从这些快速数据中推断神经过程的能力。我们假设高频fMRI信号与警觉状态相关的自发神经活动有关，并且这些高频信号可用于推断由脑电神经节律指示的神经活动的动态变化。通过在27名在睡眠与清醒之间漂移的人类受试者中进行快速fMRI（TR=378毫秒）和同步脑电图记录，我们发现，在NREM睡眠期间（与清醒相比），高达1.3 Hz频率范围内的fMRI功率增加。高频fMRI功率还与经典的与警觉性相关的脑电节律（alpha和delta）相关，其时空互相关模式既反映了共享的警觉性动态，也反映了节律特异性特征。通过机器学习，我们发现，在训练集中排除的受试者中，可以从高频fMRI信号中解码出EEG alpha和delta功率，表明fMRI信号的高频成分包含足够稳健的神经耦合信息，能够跨个体推广。这些结果表明，高频fMRI信号与动态变化的脑状态耦合，并且快速fMRI能够对自发神经活动进行时间精确的量化。

## Abstract
Technological advances have enabled fMRI acquisition with high temporal resolution, enabling brainwide imaging in just a few hundreds of milliseconds. However, the relationship between fast hemodynamic signals and spontaneous neural activity in the resting state is not yet well understood, limiting our ability to infer neural processes from these fast data. We hypothesized that high-frequency fMRI signals are linked to spontaneous neural activity tied to vigilance states, and that these high-frequency signals could be used to infer the dynamic variations in neuronal activity indexed by EEG neural rhythms. Using fast fMRI (TR=378 ms) and simultaneous EEG in 27 humans drifting between sleep and wakefulness, we found that fMRI power increased during NREM sleep (compared to wakefulness) in frequencies up to 1.3 Hz. High-frequency fMRI power was also correlated to canonical arousal-linked EEG rhythms (alpha and delta), with spatiotemporal cross-correlation patterns reflecting both shared arousal dynamics and rhythm-specific signatures. Using machine learning, we found that EEG alpha and delta power can be decoded from high-frequency fMRI signals in subjects held-out from the training set, showing that the high-frequency components of fMRI signals contain neurally-coupled information robust enough to generalize across individuals. These results reveal that high-frequency fMRI signals are coupled to dynamically varying brain states, and that fast fMRI allows for temporally precise quantification of spontaneous neural activity.

---

## 论文详细总结（自动生成）

# 详细中文总结

## 1. 论文的核心问题与整体含义（研究动机和背景）

传统功能磁共振成像（fMRI）时间分辨率较低（秒级），通常用于分析低频（<0.1 Hz）的血氧水平依赖（BOLD）信号，并假设其对神经事件的响应是缓慢的。近年来，快速fMRI技术（如多频段EPI）使全脑成像时间缩短至几百毫秒，能够检测亚秒级的刺激诱发神经活动。然而，静息态下的自发神经活动（如睡眠-觉醒转换中的脑电节律）是否也能在快速fMRI的高频信号（>1 Hz）中得到体现，仍不清楚。本研究的核心动机是：**探索快速fMRI中高频BOLD信号（高达1.3 Hz）是否与脑状态（尤其是在睡眠与清醒之间动态变化的警觉状态）耦合，并能否用于预测自发神经活动（EEG alpha和delta功率）**。整体含义：揭示快速fMRI信号的神经基础，为利用快速fMRI高时间分辨率优势研究自发神经活动提供依据。

## 2. 论文提出的方法论：核心思想、关键技术细节、公式或算法流程

### 核心思想
高频fMRI信号（0.3–1.3 Hz）包含与EEG神经节律（alpha、delta）相关的信息，这些信息可以被线性相关分析和非线性机器学习解码方法捕捉。

### 关键技术细节

#### 数据采集与预处理
- **快速fMRI**：3T Siemens Prisma，2.5 mm各向同性体素，TR=378 ms，多频段因子8，40层。
- **同步EEG**：32通道MR兼容EEG，5000 Hz采样，碳线环去除梯度伪影和心电伪影。
- **预处理**：切片时间校正、运动校正、基于谐波回归的自回归噪声模型（HRAN）去除生理噪声。
- **脑区划分**：Desikan-Killiany图谱，每半球31个皮层区、7个皮层下区、8个非灰质区（白质、脑室）。

#### 主要分析方法
1. **状态依赖的频谱分析**：在60秒稳定清醒或NREM睡眠片段上，用多锥度谱估计计算fMRI功率，比较睡眠与清醒的功率差异，采用配对t检验和Benjamini-Hochberg校正。
2. **交叉相关分析**：用5秒滑动窗计算EEG alpha（8.5–12 Hz）和delta（1.1–4 Hz）功率，以及高频fMRI功率（0.3–1.3 Hz，5秒窗），计算最大滞后40 TR的交叉相关。通过随机移位生成零分布，计算p值并Bonferroni校正。
3. **机器学习解码方法**：
   - **模型架构**：一维时序卷积层（Conv1d，核大小21，滤波器数量可调） → ReLU → 全连接层（隐藏层大小可调） → ReLU → 输出层（单标量，预测中心时刻的EEG功率）。
   - **输入**：60个TR（约22秒）的脑区平均fMRI时间序列，步长1 TR。
   - **训练**：Adam优化器（学习率0.001，每epoch衰减10倍），L2正则化（0.001–0.01），早停（最多5 epochs），批量32。
   - **评估**：留出法（每次留出3个受试者作为测试集），用剩下的受试者进行5折交叉验证调参（迭代50次），最终在留出受试者上计算预测值与真实值的 Pearson相关系数。每个折叠重复10次随机种子取平均。
   - **控制条件**：时间随机移位的fMRI数据。

## 3. 实验设计：数据集、基准、对比方法

### 数据集
- **来源**：27名健康成年人（18–39岁，15女，12男），在两个站点（波士顿大学、MIT）进行夜间睡眠MRI扫描。
- **采集内容**：每个受试者1–3个run（每个run 25分钟），同步EEG-fMRI，同时记录瞳孔、脉搏、呼吸、皮肤电导。
- **睡眠分期**：双人根据AASM标准对30秒epoch进行睡眠评分（清醒、N1、N2、N3）。
- **排除标准**：无稳定清醒片段的受试者（n=23用于频谱分析）；无静息alpha节律的受试者（n=24用于alpha分析，n=27用于delta分析）。

### 基准与对比方法
- **频谱分析**：比较NREM睡眠 vs 清醒，关注0–1.3 Hz各频段功率变化。
- **交叉相关**：与随机移位控制的对比。
- **机器学习解码**：
  - 输入变体：全频谱fMRI、低通滤过（<0.1 Hz）、高通滤过（>0.1 Hz）；控制条件（时间随机移位）。
  - 不同频段建模：高通截止频率从0.3 Hz到0.9 Hz逐步变化。
  - 不同窗口长度：0.378 s（单TR）到22 s（60 TR）。
  - 不同脑区：每个灰质区域单独建模；全局信号（所有皮层平均） vs 局部信号。
  - 对比了白质、脑室等非灰质区域。
- **无外部基准方法**，主要基于自身对照和不同过滤/窗口条件。

## 4. 资源与算力

论文未明确说明训练所用的GPU型号、数量及训练总时长。仅提到模型训练在PyTorch中实现，使用早停（最多5 epochs），超参数调优迭代50次，每个折叠重复10次随机种子。可以推测算力需求不高（模型规模小），但具体资源未披露。

## 5. 实验数量与充分性

### 实验组数
- **频谱分析**：1组主要结果（全局皮层、第四脑室、多个子区域），附多张补充图。
- **交叉相关**：分别对alpha和delta，呈现全脑各区域不同滞后下的相关模式；并比较高低频段（0.1–0.3 Hz与0.3–1.3 Hz）；还进行了HRF卷积后的分析。
- **机器学习解码**：
  - 主要解码性能对比（全频谱、低通、高通、控制）。
  - 各脑区单独解码（图5）。
  - 不同窗口长度（图6，5种以上窗口）。
  - 不同高通截止频率（图5）。
  - 非灰质区域解码（补充图）。
- 总计：约10余组主要实验，每组都有统计检验（配对t检验、置换检验、Benjamini-Hochberg校正）。

### 充分性评价
- **充分**：实验覆盖了主要假设的各个维度（频率范围、空间分布、时间窗口、个体泛化性）。
- **客观公平**：使用留出受试者进行模型评估，避免了过拟合；控制条件（随机移位）证实了结果并非偶然；多重比较校正合理。
- **可能不足**：数据仅来自两个站点，样本量27中等；未在独立数据集上验证泛化性（但跨个体留出已提供一定泛化证据）。

## 6. 论文的主要结论与发现

1. **高频fMRI功率在NREM睡眠中增加**：清醒到NREM睡眠，fMRI功率在0–1.3 Hz宽带内显著增加，尤其在视觉皮层（楔叶）可达1.3 Hz。
2. **高频fMRI功率与EEG节律相关**：alpha和delta功率与0.3–1.3 Hz fMRI功率在多个脑区呈现显著交叉相关，峰值接近0 lag，但两种节律呈现不同时空模式：alpha的负相关（6–10 s后）在枕叶更强；delta的正相关（0–6 s后）从额叶向枕叶传播。
3. **机器学习解码成功**：可从高频fMRI（>0.1 Hz）解码alpha和delta功率，且在留出受试者上表现显著。解码alpha时低、高频信息冗余；解码delta时高频信息提供额外信息（低通后性能下降）。
4. **快速窗口解码**：短至3.8 s的fMRI窗即可有效解码alpha和delta，单TR（0.378 s）也能解码alpha（保留空间信息时）。
5. **非灰质信号包含信息**：白质和第四脑室的fMRI信号同样与EEG节律相关，但解码性能低于灰质。
6. **全局信号贡献显著**：全局皮层信号包含大量与警觉性相关的信息。

## 7. 优点：方法或实验设计上的亮点

- **高时间分辨率采集**：TR=378 ms，能够解析高达1.3 Hz的BOLD信号，避免了心脏/呼吸伪影的混叠。
- **同步EEG验证**：直接使用EEG作为神经活动金标准，验证快速fMRI的神经耦合性。
- **跨个体泛化性**：留出受试者评估，证明解码模型具有跨个体推广能力，而非只适用于训练集。
- **多维度分析**：既用线性交叉相关揭示动态关系，又用非线性神经网络进行解码，互补性强。
- **系统对比**：比较不同频段、不同窗口长度、不同脑区、不同输入类型，全面刻画高频fMRI信息的特性。
- **控制实验充分**：随机移位控制、多种过滤条件、独立超参数调优，确保结果可靠。

## 8. 不足与局限

- **样本量限制**：27名受试者（部分分析更少），年龄范围18–39岁，可能无法代表更广泛人群（如老年人、儿童、患者）。
- **频率上限受限**：TR=378 ms使奈奎斯特频率为1.3 Hz，无法研究更高频BOLD信号（论文指出楔叶可能仍有更高频效应）。
- **场强限制**：3T扫描，信噪比低于7T，可能遗漏微弱的高频神经血管耦合信号。
- **缺乏独立验证集**：尽管有留出受试者，但训练和测试数据来自同一采集条件，未在独立实验室/设备上验证。
- **建模假设**：机器学习模型是非因果的（使用中心时刻的周围窗口），不适用于在线或实时应用。
- **生理噪声影响未完全排除**：低频率的心率、呼吸变异性未回归（可能包含神经相关信息），但可能引入部分非神经成分。
- **神经元机制不确定**：高频BOLD信号的产生机制（微血管响应、全局血流动力学、脑脊液流动等）未直接阐明，需未来工作。

（完）
