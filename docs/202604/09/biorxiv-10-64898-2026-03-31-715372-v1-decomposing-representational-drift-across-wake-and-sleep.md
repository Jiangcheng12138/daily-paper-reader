---
title: Decomposing representational drift across wake and sleep
title_zh: 分解觉醒与睡眠过程中的表征漂移
authors: "Harris, J. J., Schaefer, A. T., Kollo, M."
date: 2026-04-02
pdf: "https://www.biorxiv.org/content/10.64898/2026.03.31.715372v1.full.pdf"
tags: ["query:slp-ns"]
score: 10.0
evidence: 觉醒和睡眠状态下的表征漂移
tldr: 本研究探讨了觉醒与睡眠对神经表征漂移的不同影响。通过记录小鼠嗅觉皮层的单细胞活动并使用低秩解码器，研究发现睡眠并非觉醒学习的延续，而是引发了表征轨迹的转向，表现为去相关和旋转。此外，研究首次发现了嗅觉重现现象，且与梨状皮层尖波相关。这揭示了表征漂移具有状态依赖性，明确了睡眠在感官表征演变中的独特作用。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-03-31-715372-v1/fig-001.webp\", \"caption\": \"Figure 1. Odour representations undergo distinct transformations during wake and sleep. (a) Decoder weight matrices for a single odour (odour 1 of sequence F, mouse 2), showing similar baseline weights and 𝑊₀ end-of-session weights . Their difference corresponds to a small change. Neuronal units sorted by mean per 𝑊 𝑒𝑛𝑑 ∆𝑊 ∆𝑊 brain area. The colour scale (blue-white-red) is for negative to positive weights (identical colour scale used for all matrices in the panel). (b) The total change decomposes into four different drift modes D1-4. (Identical colour scale used for all matrices in the panel). (c) Normalised sigmoid activations for each mode in four mice. D1 (blue) activates during early wake, D2 (orange) and D3 (green) during the wake-sleep transition and sleep, and D4 (red) in post-sleep. Blue shading indicates the main NREM sleep block, odour sequences were played to the mice before and after sleep. (d) Relative amplitude of each mode. Bars: mean ± SEM across 4 recordings. *p < 0.05, Holm-corrected paired t-tests between mode pairs. (e) Fraction of each mode's drift amplitude attributable to the familiar (F1) sequence odours. All modes affect both sequences approximately equally. (f) Readout gain: cosine similarity between each mode's weight change and the baseline weights. D1 is significantly aligned with , indicating it scales the existing readout pattern. Stars: 𝑊₀ one-sample t-test vs zero, Bonferroni-corrected across 4 modes. (g) Rotation angle between and , in 𝑊₀ 𝑊₀ + ∆𝑊 𝑖 degrees. All modes produce significant rotation (**p < 0.01). (h) Odour decorrelation: change in mean pairwise Pearson correlation between odour weight vectors when each mode is applied (positive = increased distinctness). (i) Drift trajectory through weight space for each recording across the session. The four weight vectors are projected into ∆𝑊(τ) 2D via SVD. The total drift direction is aligned horizontally. Coloured dots mark drift mode midpoints. Tick marks show τ values at 0.25 intervals. All mice show a similar path: D1 starts roughly along the baseline direction, then D2/D3 bend the trajectory during sleep, with D4 adding a minor late component.\", \"page\": 7, \"index\": 1, \"width\": 783, \"height\": 871}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-03-31-715372-v1/fig-002.webp\", \"caption\": \"Figure 2. Temporally compressed odour replay during NREM sleep. (a) Example stimulus presentations (left) and NREM replay events (right) for the novel (N, left pair) and familiar (F, right pair) odour sequences. Top rows: true odour identity; bottom rows: decoded probability P(odour) from the drift decoder, displayed as colour-coded RGBA heatmaps (2-bin boxcar smoothed). Each row corresponds to one odour in the sequence; rows are grouped by sequence (N1-N4, F1-F4). Dashed lines mark stimulus onset/offset (stim panels) or first/last detected replay peak (replay panels). During wake stimulation, the decoder produces sequential activations matching the presented odour order. During NREM, spontaneous reactivations recapitulate the learned sequence at compressed timescales. (b) Transition matrices showing the regression weight from each odour's decoded probability at time to every𝑡 other odour at time (ridge regression), computed at 2.5× temporal compression ( =400ms). Dashed𝑡 + ∆𝑡 ∆𝑡 boxes highlight forward transitions along the trained sequence order. NREM shows stronger within-sequence forward structure than wake or circular-shifted channel shuffle (mean of 50 shuffles). (c) Forward (filled circles) and backward (open circles) transition strengths per mouse at 2.5× compression, for F1 (red) and N1 (blue) sequences separately. Horizontal grey lines show the 95th percentile of the circular-shift null distribution (500 shuffles). Forward transitions consistently exceed backward and shuffle in all mice. (d) Sequenceness (forward − backward transition strength) across temporal compression factors (1×-10×) for both sequences (F red, N blue). Lines: individual mice; shading: SEM. Peak sequenceness occurs at 2-3× compression for both sequences, corresponding to replay timescales of 300-500 ms per odour (vs 1 s during wake presentation). (e) Statistical significance of sequential replay structure at 2.5× compression, shown for three levels of sequence analysis: pairwise transitions (adjacent odour pairs), 3-element subsequences, and full 4-element sequences. Each dot is one mouse × sequence combination.\", \"page\": 9, \"index\": 2, \"width\": 960, \"height\": 756}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-03-31-715372-v1/fig-003.webp\", \"caption\": \"Figure 3. Piriform sharp waves during NREM sleep are associated with odour replay. (a) Example piriform sharp waves (SPWs) detected during NREM sleep. Top: raw LFP from a piriform channel showing the sharp wave deflection (negative polarity, peak amplitude annotated in µV). Middle: 80-140 Hz filtered signal showing co-occurring fast gamma activity. Bottom: 160-190 Hz filtered signal showing ripple-band oscillations. (b) SPW rate across behavioural states. Box plots show the distribution across recordings (n = 3) for pre-sleep wake, NREM, and post-sleep wake. Paired lines connect the same recording. SPW rate is elevated during NREM relative to wake periods. (c) Peri-SPW triggered power in gamma (80-140 Hz, blue) and ripple (160-190 Hz, grey) frequency bands. Both gamma and ripple power peak sharply at the time of the SPW, with gamma showing a ~60% increase and ripple ~15% above baseline. (d) SPW-replay coupling. The probability of observing a replay event (decoder P(odour) > 0.05) within 0-500 ms following a sharp wave, compared between observed data and circular-shift null (500 shuffles). Each dot is one recording. Two of three mice show significant SPW-replay co-occurrence, comparing observed coupling rate against the null distribution. (M1 p = 0.033, M2 p < 0.001). (e) Peri-SPW replay PSTH for the recording with the strongest coupling (M2). Blue: observed replay rate in 150 ms bins around each sharp wave. Grey: shuffle expected rate with 95% CI envelope. The observed replay rate peaks in the 0-500 ms window following the SPW, exceeding shuffle expectations.\", \"page\": 11, \"index\": 3, \"width\": 850, \"height\": 661}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-03-31-715372-v1/fig-004.webp\", \"caption\": \"Table 1. Odour stimulus identities. IDs are arbitrary codes based on Canberra distances in chemical space (e.g. C3f = Cluster 3, far).\", \"page\": 21, \"index\": 4, \"width\": 673, \"height\": 448}]"
motivation: 旨在厘清觉醒时的在线经验与睡眠时的离线状态对神经表征随时间演变（表征漂移）的各自贡献。
method: 记录小鼠嗅觉皮层在气味暴露与睡眠循环中的单神经元活动，并开发低秩解码器来追踪和分解表征漂移。
result: 识别出四种正交漂移模式，发现睡眠引发了与觉醒截然不同的表征转向，并首次观测到伴随尖波的嗅觉重现。
conclusion: 神经表征漂移由状态依赖的组件构成，睡眠在感官表征的重组中发挥着与觉醒学习互补且独特的贡献。
---

## 摘要
神经表征随时间演变，但在线经验与睡眠等离线状态的相对贡献仍不明确。在本研究中，我们记录了小鼠在觉醒气味暴露与睡眠循环中嗅觉皮层的单单元活动，并开发了一种低秩解码器来追踪表征漂移。我们识别出四种在不同时间尺度上运行的正交漂移模式，揭示了睡眠和觉醒驱动着性质截然不同的转换，这表明离线重组并非在线学习的简单延续。相反，睡眠引发了整体漂移轨迹的转向，其独特特征是气味表征的去相关与旋转的结合。我们还提供了嗅觉重现（olfactory replay）的首个证据，该现象发生在大约 2.5 倍的时间压缩下，并与局部产生的梨状皮层尖波相关。总之，这些发现证明了表征漂移包含状态依赖的成分，并揭示了觉醒和睡眠对感觉表征变化的独特贡献。

## Abstract
Neural representations evolve over time, yet the relative contributions of online experience and offline states such as sleep remain unclear. Here, we recorded single-unit activity in the olfactory cortex of mice across cycles of awake odour exposure and sleep, and developed a low-rank decoder to track representational drift. We identified four orthogonal drift modes operating on distinct timescales, revealing that sleep and wake drive qualitatively different transformations, which indicates that offline reorganisation is not a simple continuation of online learning. Rather, sleep initiates an about-turn in the overall drift trajectory, which is uniquely characterised by a combination of decorrelation and rotation of odour representations. We also provide the first evidence for olfactory replay, occurring at ~2.5x temporal compression and associated with locally generated piriform cortex sharp waves. Together, these findings demonstrate that representational drift comprises state-dependent components, and reveal distinct contributions of wake and sleep to sensory representational change.

---

## 论文详细总结（自动生成）

这是一份关于论文《Decomposing representational drift across wake and sleep》（分解觉醒与睡眠过程中的表征漂移）的深度学术总结：

### 1. 核心问题与整体含义
*   **研究动机**：神经表征（即大脑对特定刺激的反应模式）并非固定不变，而是会随时间发生“表征漂移”（Representational Drift）。科学界一直存在争议：这种漂移是由于觉醒时的持续学习引起的，还是睡眠等离线状态下的主动重组过程？
*   **核心问题**：睡眠对感官表征演变的贡献是否仅仅是觉醒状态下学习过程的延续，还是具有其独特的转换逻辑？
*   **整体含义**：本研究通过分解不同状态下的漂移模式，揭示了睡眠在神经表征演化中扮演着与觉醒截然不同的角色，并非简单的“离线备份”，而是通过去相关和旋转等手段对信息进行重塑。

### 2. 方法论：核心思想与技术细节
*   **低秩解码器（Low-rank Decoder）**：研究者开发了一种线性解码器来追踪神经元群体的活动。其核心思想是利用权重矩阵 $W$ 的变化来量化表征的演变。
*   **漂移分解算法**：
    *   将总的权重变化 $\Delta W$ 分解为四个正交的漂移模式（$D_1$ 到 $D_4$）。
    *   通过逻辑回归和时间常数拟合，识别出这些模式在不同行为状态（早起觉醒、觉醒-睡眠过渡、睡眠中、睡眠后）的激活权重。
*   **重现（Replay）检测**：利用训练好的解码器在非快速眼动（NREM）睡眠期间检测自发活动。通过计算转移矩阵和“序列性”（Sequenceness）指标，评估神经活动是否以压缩的时间尺度重现了觉醒时的气味序列。
*   **尖波（Sharp Wave）分析**：在梨状皮层（Piriform Cortex）检测局部场电位（LFP）的尖波，并分析其与重现事件的时间相关性。

### 3. 实验设计
*   **实验对象与场景**：对 4 只小鼠的嗅觉皮层进行单单元电生理记录。实验流程包括：初始气味暴露（熟悉序列 F 和新序列 N）、长达数小时的睡眠观察、睡眠后的再次气味暴露。
*   **Benchmark 与对比**：
    *   **状态对比**：对比了觉醒（Wake）与睡眠（NREM/REM）状态下的漂移特征。
    *   **序列对比**：对比了熟悉序列与新序列在重现强度上的差异。
    *   **零假设检验**：使用循环偏移（Circular-shift）等洗牌算法（Shuffle）作为基准，验证重现现象和尖波耦合的统计显著性。

### 4. 资源与算力
*   **算力说明**：论文中未明确提及具体的 GPU 型号或大规模集群计算。考虑到其方法论涉及单单元记录处理、线性解码器训练和统计模拟，通常使用高性能工作站（配备标准 CPU 和中等内存）即可完成。
*   **软件工具**：使用了标准的神经科学分析工具链（如 Python/MATLAB 相关的电生理处理库）。

### 5. 实验数量与充分性
*   **实验规模**：研究基于 4 只小鼠的深度记录，虽然样本量（动物数）在生物学实验中属于标准范围，但其单神经元记录的数量和时间跨度提供了高分辨率的数据支持。
*   **充分性评价**：
    *   **多维度验证**：实验不仅观察了漂移，还通过重现分析和 LFP 耦合分析从多个层面验证了睡眠的功能。
    *   **消融与对照**：通过分解出四个正交模式，有效地隔离了不同时间段的贡献，实验逻辑严密。
    *   **局限性**：样本量相对较小，且主要集中在嗅觉系统，其结论在其他感官系统（如视觉、听觉）中的普适性仍需进一步验证。

### 6. 主要结论与发现
*   **漂移模式的异质性**：识别出四种模式。$D_1$ 主要在觉醒早期激活，表现为现有表征的缩放；而 $D_2$ 和 $D_3$ 在睡眠期间激活。
*   **睡眠引发轨迹转向**：睡眠并非延续觉醒时的漂移方向，而是引发了表征轨迹的“转向”。这种转向通过**去相关（Decorrelation）**和**旋转（Rotation）**增强了不同气味表征之间的区分度。
*   **首次发现嗅觉重现**：在 NREM 睡眠中观测到了气味序列的自发重现，时间压缩比约为 2.5 倍。
*   **尖波耦合**：梨状皮层的尖波（Sharp Waves）与重现事件高度相关，暗示了嗅觉皮层具有类似于海马体的离线信息处理机制。

### 7. 优点
*   **创新性方法**：提出的低秩解码器分解法为研究表征漂移提供了一个量化且可解释的框架。
*   **科学突破**：填补了嗅觉系统是否存在“重现”现象的空白，并明确了睡眠对表征漂移的独特贡献。
*   **动态视角**：将神经表征视为一个动态演化的轨迹，而非静态的快照，更符合大脑工作的本质。

### 8. 不足与局限
*   **因果性缺失**：研究主要基于相关性分析（如尖波与重现的相关），尚未通过光遗传学等手段证明干扰睡眠或尖波会直接阻碍表征的去相关过程。
*   **行为关联模糊**：虽然观察到了表征的去相关，但未直接测试这种神经层面的变化如何转化为小鼠辨别气味行为能力的提升。
*   **状态分类简化**：对睡眠阶段的划分主要集中在 NREM，对 REM 睡眠在漂移中的具体作用探讨较少。

（完）
