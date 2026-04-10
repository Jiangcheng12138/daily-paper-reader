---
title: Decomposing representational drift across wake and sleep
title_zh: 分解觉醒与睡眠过程中的表征漂移
authors: "Harris, J. J., Schaefer, A. T., Kollo, M."
date: 2026-04-02
pdf: "https://www.biorxiv.org/content/10.64898/2026.03.31.715372v1.full.pdf"
tags: ["query:slp-ns"]
score: 10.0
evidence: 觉醒和睡眠周期中的神经表征漂移
tldr: 本研究探讨了觉醒时的在线经验与睡眠时的离线状态对神经表征漂移的贡献。通过记录小鼠嗅觉皮层的单细胞活动并使用低秩解码器，研究发现睡眠与觉醒驱动了截然不同的表征转换。睡眠并非在线学习的延续，而是通过去相关和旋转改变了漂移轨迹，并首次发现了伴随梨状皮层尖波的嗅觉重现现象，揭示了睡眠在感官表征演变中的独特作用。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-03-31-715372-v1/fig-001.webp\", \"caption\": \"Figure 1. Odour representations undergo distinct transformations during wake and sleep. (a) Decoder weight matrices for a single odour (odour 1 of sequence F, mouse 2), showing similar baseline weights and 𝑊₀ end-of-session weights . Their difference corresponds to a small change. Neuronal units sorted by mean per 𝑊 𝑒𝑛𝑑 ∆𝑊 ∆𝑊 brain area. The colour scale (blue-white-red) is for negative to positive weights (identical colour scale used for all matrices in the panel). (b) The total change decomposes into four different drift modes D1-4. (Identical colour scale used for all matrices in the panel). (c) Normalised sigmoid activations for each mode in four mice. D1 (blue) activates during early wake, D2 (orange) and D3 (green) during the wake-sleep transition and sleep, and D4 (red) in post-sleep. Blue shading indicates the main NREM sleep block, odour sequences were played to the mice before and after sleep. (d) Relative amplitude of each mode. Bars: mean ± SEM across 4 recordings. *p < 0.05, Holm-corrected paired t-tests between mode pairs. (e) Fraction of each mode's drift amplitude attributable to the familiar (F1) sequence odours. All modes affect both sequences approximately equally. (f) Readout gain: cosine similarity between each mode's weight change and the baseline weights. D1 is significantly aligned with , indicating it scales the existing readout pattern. Stars: 𝑊₀ one-sample t-test vs zero, Bonferroni-corrected across 4 modes. (g) Rotation angle between and , in 𝑊₀ 𝑊₀ + ∆𝑊 𝑖 degrees. All modes produce significant rotation (**p < 0.01). (h) Odour decorrelation: change in mean pairwise Pearson correlation between odour weight vectors when each mode is applied (positive = increased distinctness). (i) Drift trajectory through weight space for each recording across the session. The four weight vectors are projected into ∆𝑊(τ) 2D via SVD. The total drift direction is aligned horizontally. Coloured dots mark drift mode midpoints. Tick marks show τ values at 0.25 intervals. All mice show a similar path: D1 starts roughly along the baseline direction, then D2/D3 bend the trajectory during sleep, with D4 adding a minor late component.\", \"page\": 7, \"index\": 1, \"width\": 783, \"height\": 871}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-03-31-715372-v1/fig-002.webp\", \"caption\": \"Figure 2. Temporally compressed odour replay during NREM sleep. (a) Example stimulus presentations (left) and NREM replay events (right) for the novel (N, left pair) and familiar (F, right pair) odour sequences. Top rows: true odour identity; bottom rows: decoded probability P(odour) from the drift decoder, displayed as colour-coded RGBA heatmaps (2-bin boxcar smoothed). Each row corresponds to one odour in the sequence; rows are grouped by sequence (N1-N4, F1-F4). Dashed lines mark stimulus onset/offset (stim panels) or first/last detected replay peak (replay panels). During wake stimulation, the decoder produces sequential activations matching the presented odour order. During NREM, spontaneous reactivations recapitulate the learned sequence at compressed timescales. (b) Transition matrices showing the regression weight from each odour's decoded probability at time to every𝑡 other odour at time (ridge regression), computed at 2.5× temporal compression ( =400ms). Dashed𝑡 + ∆𝑡 ∆𝑡 boxes highlight forward transitions along the trained sequence order. NREM shows stronger within-sequence forward structure than wake or circular-shifted channel shuffle (mean of 50 shuffles). (c) Forward (filled circles) and backward (open circles) transition strengths per mouse at 2.5× compression, for F1 (red) and N1 (blue) sequences separately. Horizontal grey lines show the 95th percentile of the circular-shift null distribution (500 shuffles). Forward transitions consistently exceed backward and shuffle in all mice. (d) Sequenceness (forward − backward transition strength) across temporal compression factors (1×-10×) for both sequences (F red, N blue). Lines: individual mice; shading: SEM. Peak sequenceness occurs at 2-3× compression for both sequences, corresponding to replay timescales of 300-500 ms per odour (vs 1 s during wake presentation). (e) Statistical significance of sequential replay structure at 2.5× compression, shown for three levels of sequence analysis: pairwise transitions (adjacent odour pairs), 3-element subsequences, and full 4-element sequences. Each dot is one mouse × sequence combination.\", \"page\": 9, \"index\": 2, \"width\": 960, \"height\": 756}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-03-31-715372-v1/fig-003.webp\", \"caption\": \"Figure 3. Piriform sharp waves during NREM sleep are associated with odour replay. (a) Example piriform sharp waves (SPWs) detected during NREM sleep. Top: raw LFP from a piriform channel showing the sharp wave deflection (negative polarity, peak amplitude annotated in µV). Middle: 80-140 Hz filtered signal showing co-occurring fast gamma activity. Bottom: 160-190 Hz filtered signal showing ripple-band oscillations. (b) SPW rate across behavioural states. Box plots show the distribution across recordings (n = 3) for pre-sleep wake, NREM, and post-sleep wake. Paired lines connect the same recording. SPW rate is elevated during NREM relative to wake periods. (c) Peri-SPW triggered power in gamma (80-140 Hz, blue) and ripple (160-190 Hz, grey) frequency bands. Both gamma and ripple power peak sharply at the time of the SPW, with gamma showing a ~60% increase and ripple ~15% above baseline. (d) SPW-replay coupling. The probability of observing a replay event (decoder P(odour) > 0.05) within 0-500 ms following a sharp wave, compared between observed data and circular-shift null (500 shuffles). Each dot is one recording. Two of three mice show significant SPW-replay co-occurrence, comparing observed coupling rate against the null distribution. (M1 p = 0.033, M2 p < 0.001). (e) Peri-SPW replay PSTH for the recording with the strongest coupling (M2). Blue: observed replay rate in 150 ms bins around each sharp wave. Grey: shuffle expected rate with 95% CI envelope. The observed replay rate peaks in the 0-500 ms window following the SPW, exceeding shuffle expectations.\", \"page\": 11, \"index\": 3, \"width\": 850, \"height\": 661}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-03-31-715372-v1/fig-004.webp\", \"caption\": \"Table 1. Odour stimulus identities. IDs are arbitrary codes based on Canberra distances in chemical space (e.g. C3f = Cluster 3, far).\", \"page\": 21, \"index\": 4, \"width\": 673, \"height\": 448}]"
motivation: 探究神经表征随时间演变的机制，特别是觉醒经验与睡眠状态对表征漂移的相对贡献。
method: 记录小鼠嗅觉皮层在气味暴露与睡眠循环中的单神经元活动，并开发低秩解码器追踪表征漂移。
result: 识别出四种正交漂移模式，发现睡眠引发了表征轨迹的逆转（去相关与旋转），并首次观测到约2.5倍压缩的嗅觉重现。
conclusion: 神经表征漂移具有状态依赖性，睡眠在感官表征演变中起到了与觉醒截然不同且关键的重组作用。
---

## 摘要
神经表征随时间演变，但在线经验与如睡眠等离线状态的相对贡献仍不清楚。在本研究中，我们记录了小鼠在觉醒气味暴露与睡眠循环中嗅觉皮层的单单元活动，并开发了一种低秩解码器来追踪表征漂移。我们识别出在不同时间尺度上运行的四个正交漂移模式，揭示了睡眠和觉醒驱动着性质截然不同的转换，这表明离线重组并非在线学习的简单延续。相反，睡眠引发了整体漂移轨迹的转向，其独特特征是气味表征的去相关与旋转的结合。我们还提供了嗅觉重现（replay）的首个证据，该现象以约 2.5 倍的时间压缩发生，并与局部产生的梨状皮层锐波相关。总之，这些发现证明了表征漂移包含状态依赖的成分，并揭示了觉醒和睡眠对感觉表征变化的独特贡献。

## Abstract
Neural representations evolve over time, yet the relative contributions of online experience and offline states such as sleep remain unclear. Here, we recorded single-unit activity in the olfactory cortex of mice across cycles of awake odour exposure and sleep, and developed a low-rank decoder to track representational drift. We identified four orthogonal drift modes operating on distinct timescales, revealing that sleep and wake drive qualitatively different transformations, which indicates that offline reorganisation is not a simple continuation of online learning. Rather, sleep initiates an about-turn in the overall drift trajectory, which is uniquely characterised by a combination of decorrelation and rotation of odour representations. We also provide the first evidence for olfactory replay, occurring at ~2.5x temporal compression and associated with locally generated piriform cortex sharp waves. Together, these findings demonstrate that representational drift comprises state-dependent components, and reveal distinct contributions of wake and sleep to sensory representational change.

---

## 论文详细总结（自动生成）

这是一份关于论文《Decomposing representational drift across wake and sleep》（分解觉醒与睡眠过程中的表征漂移）的结构化总结：

### 1. 核心问题与整体含义（研究动机和背景）
论文探讨了**神经表征漂移（Representational Drift）**的动态机制。虽然已知神经元对相同刺激的反应会随时间缓慢变化，但科学界尚不清楚这种变化是由于觉醒时的持续学习（在线经验）驱动的，还是由睡眠时的离线巩固（离线状态）驱动的。
*   **研究动机**：揭示觉醒和睡眠在感觉表征演变中扮演的独特角色。
*   **背景**：梨状皮层（嗅觉皮层）的表征在数周内会发生漂移，但这种长期漂移是由哪些短期过程（如突触稳态、重现等）累积而成的，此前缺乏精细的时间尺度分解。

### 2. 方法论：核心思想与关键技术
研究者开发了一种创新的**低秩漂移解码器（Low-rank drift decoder）**，用于追踪和分解表征变化。
*   **核心思想**：将随时间演变的解码权重矩阵 $W(\tau)$ 分解为一个基准权重 $W_0$ 和四个正交的低秩扰动矩阵（漂移模式 $\Delta W_i$）的总和。
*   **公式逻辑**：$W(\tau) = W_0 + \sum_{i=1}^{4} \alpha_i(\tau) \cdot \Delta W_i$。其中 $\alpha_i(\tau)$ 是学习到的 Sigmoid 激活函数，代表不同模式在不同阶段的贡献。
*   **关键技术**：
    *   使用 **Neuropixels 2.0** 探针记录小鼠嗅觉皮层的单单元活动。
    *   **TDLM（时间延迟线性建模）**：用于检测自发活动中是否存在与觉醒时气味序列一致的“重现”现象。
    *   **LFP 分析**：识别梨状皮层局部的锐波（Sharp Waves, SPWs），并分析其与重现事件的关联。

### 3. 实验设计
*   **实验场景**：采用“觉醒气味暴露（前）— 自然睡眠（约1小时）— 觉醒气味暴露（后）”的范式。
*   **刺激物**：包含“熟悉”和“新颖”两种四元素气味序列。
*   **Benchmark/对比**：
    *   对比了**漂移解码器**与**静态解码器**（固定基准权重）的预测准确率。
    *   对比了觉醒阶段与睡眠阶段的漂移轨迹几何特征（旋转角度、去相关程度）。
    *   通过对解码结果进行时间洗牌（Shuffle）建立零假设分布，验证重现的显著性。

### 4. 资源与算力
*   论文**未明确说明**具体的 GPU 型号、数量或训练时长。
*   文中提到使用了 **Kilosort 4** 进行尖峰分拣（Spike sorting），这通常需要高性能 GPU 支持。数据分析使用了 Python 环境下的 SpikeInterface、Bonsai 等工具。

### 5. 实验数量与充分性
*   **实验规模**：记录了 4 只小鼠，共计 636 个在整个实验周期内保持稳定的神经元单元。
*   **充分性评价**：
    *   **数据深度高**：单神经元级别的长期追踪和多维度（EEG/EMG/LFP/Spike）同步记录提供了丰富的信息。
    *   **分析全面**：不仅分析了表征漂移，还深入探讨了重现的压缩倍数、空间几何轨迹以及局部场电位的关联。
    *   **统计严谨**：使用了多种洗牌检验（Circular-shift null）和交叉验证来确保发现的可靠性。
    *   **局限性**：样本量（4只鼠）在系统神经科学中属于标准范围，但若能增加更多动物样本将更具普适性。

### 6. 主要结论与发现
*   **漂移模式分解**：识别出 4 种正交模式。D1 对应初始暴露（适配），D2/D3 对应睡眠转换，D4 对应睡眠后暴露。
*   **睡眠的独特贡献**：睡眠引发了漂移轨迹的“掉头”（About-turn）。睡眠期间的表征变化以**旋转（Rotation）**和**去相关（Decorrelation）**为特征，这有助于提高气味辨别力。
*   **首次发现嗅觉重现**：在睡眠期间观测到气味序列的自发重现，具有约 **2.5 倍的时间压缩**。
*   **局部协调**：嗅觉重现与梨状皮层自发产生的锐波（SPW）在时间上高度耦合，表明嗅觉巩固可能在局部完成，不一定依赖海马体。

### 7. 优点与亮点
*   **模型创新**：低秩漂移解码器为研究神经群体活动的非平稳性提供了一个强大的数学框架。
*   **科学突破**：填补了嗅觉领域关于“睡眠中是否存在重现”的空白，并挑战了“睡眠只是觉醒学习的简单延续”这一传统观点。
*   **几何视角**：通过高维空间的轨迹分析，直观地展示了不同行为状态如何改变神经编码的结构。

### 8. 不足与局限
*   **任务复杂度较低**：实验采用被动气味暴露，缺乏复杂的行为决策或强化学习任务，可能限制了对“巩固”功能意义的全面理解。
*   **睡眠时长限制**：实验中的睡眠时间较短（约1小时），且主要为 NREM 睡眠，缺乏对 REM 睡眠贡献的探讨。
*   **因果性验证不足**：目前的研究主要是相关性分析，未来需要通过闭环干预（如抑制锐波）来证明重现对表征漂移的因果作用。

（完）
