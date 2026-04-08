---
title: Decomposing representational drift across wake and sleep
title_zh: 分解觉醒与睡眠过程中的表征漂移
authors: "Harris, J. J., Schaefer, A. T., Kollo, M."
date: 2026-04-02
pdf: "https://www.biorxiv.org/content/10.64898/2026.03.31.715372v1.full.pdf"
tags: ["query:slp-ns"]
score: 10.0
evidence: 觉醒和睡眠期间的神经表征和表征漂移
tldr: 本研究探讨了神经表征漂移在清醒与睡眠状态下的演变差异。通过记录小鼠嗅觉皮层的单细胞活动并利用低秩解码器追踪表征变化，研究发现睡眠并非清醒学习的简单延续，而是引发了表征轨迹的逆转，表现为去相关和旋转。此外，研究首次发现了嗅觉重现现象。这一发现揭示了睡眠在感官表征重组中的独特作用，证明了表征漂移具有状态依赖性。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-03-31-715372-v1/fig-001.webp\", \"caption\": \"Figure 1. Odour representations undergo distinct transformations during wake and sleep. (a) Decoder weight matrices for a single odour (odour 1 of sequence F, mouse 2), showing similar baseline weights and 𝑊₀ end-of-session weights . Their difference corresponds to a small change. Neuronal units sorted by mean per 𝑊 𝑒𝑛𝑑 ∆𝑊 ∆𝑊 brain area. The colour scale (blue-white-red) is for negative to positive weights (identical colour scale used for all matrices in the panel). (b) The total change decomposes into four different drift modes D1-4. (Identical colour scale used for all matrices in the panel). (c) Normalised sigmoid activations for each mode in four mice. D1 (blue) activates during early wake, D2 (orange) and D3 (green) during the wake-sleep transition and sleep, and D4 (red) in post-sleep. Blue shading indicates the main NREM sleep block, odour sequences were played to the mice before and after sleep. (d) Relative amplitude of each mode. Bars: mean ± SEM across 4 recordings. *p < 0.05, Holm-corrected paired t-tests between mode pairs. (e) Fraction of each mode's drift amplitude attributable to the familiar (F1) sequence odours. All modes affect both sequences approximately equally. (f) Readout gain: cosine similarity between each mode's weight change and the baseline weights. D1 is significantly aligned with , indicating it scales the existing readout pattern. Stars: 𝑊₀ one-sample t-test vs zero, Bonferroni-corrected across 4 modes. (g) Rotation angle between and , in 𝑊₀ 𝑊₀ + ∆𝑊 𝑖 degrees. All modes produce significant rotation (**p < 0.01). (h) Odour decorrelation: change in mean pairwise Pearson correlation between odour weight vectors when each mode is applied (positive = increased distinctness). (i) Drift trajectory through weight space for each recording across the session. The four weight vectors are projected into ∆𝑊(τ) 2D via SVD. The total drift direction is aligned horizontally. Coloured dots mark drift mode midpoints. Tick marks show τ values at 0.25 intervals. All mice show a similar path: D1 starts roughly along the baseline direction, then D2/D3 bend the trajectory during sleep, with D4 adding a minor late component.\", \"page\": 7, \"index\": 1, \"width\": 783, \"height\": 871}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-03-31-715372-v1/fig-002.webp\", \"caption\": \"Figure 2. Temporally compressed odour replay during NREM sleep. (a) Example stimulus presentations (left) and NREM replay events (right) for the novel (N, left pair) and familiar (F, right pair) odour sequences. Top rows: true odour identity; bottom rows: decoded probability P(odour) from the drift decoder, displayed as colour-coded RGBA heatmaps (2-bin boxcar smoothed). Each row corresponds to one odour in the sequence; rows are grouped by sequence (N1-N4, F1-F4). Dashed lines mark stimulus onset/offset (stim panels) or first/last detected replay peak (replay panels). During wake stimulation, the decoder produces sequential activations matching the presented odour order. During NREM, spontaneous reactivations recapitulate the learned sequence at compressed timescales. (b) Transition matrices showing the regression weight from each odour's decoded probability at time to every𝑡 other odour at time (ridge regression), computed at 2.5× temporal compression ( =400ms). Dashed𝑡 + ∆𝑡 ∆𝑡 boxes highlight forward transitions along the trained sequence order. NREM shows stronger within-sequence forward structure than wake or circular-shifted channel shuffle (mean of 50 shuffles). (c) Forward (filled circles) and backward (open circles) transition strengths per mouse at 2.5× compression, for F1 (red) and N1 (blue) sequences separately. Horizontal grey lines show the 95th percentile of the circular-shift null distribution (500 shuffles). Forward transitions consistently exceed backward and shuffle in all mice. (d) Sequenceness (forward − backward transition strength) across temporal compression factors (1×-10×) for both sequences (F red, N blue). Lines: individual mice; shading: SEM. Peak sequenceness occurs at 2-3× compression for both sequences, corresponding to replay timescales of 300-500 ms per odour (vs 1 s during wake presentation). (e) Statistical significance of sequential replay structure at 2.5× compression, shown for three levels of sequence analysis: pairwise transitions (adjacent odour pairs), 3-element subsequences, and full 4-element sequences. Each dot is one mouse × sequence combination.\", \"page\": 9, \"index\": 2, \"width\": 960, \"height\": 756}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-03-31-715372-v1/fig-003.webp\", \"caption\": \"Figure 3. Piriform sharp waves during NREM sleep are associated with odour replay. (a) Example piriform sharp waves (SPWs) detected during NREM sleep. Top: raw LFP from a piriform channel showing the sharp wave deflection (negative polarity, peak amplitude annotated in µV). Middle: 80-140 Hz filtered signal showing co-occurring fast gamma activity. Bottom: 160-190 Hz filtered signal showing ripple-band oscillations. (b) SPW rate across behavioural states. Box plots show the distribution across recordings (n = 3) for pre-sleep wake, NREM, and post-sleep wake. Paired lines connect the same recording. SPW rate is elevated during NREM relative to wake periods. (c) Peri-SPW triggered power in gamma (80-140 Hz, blue) and ripple (160-190 Hz, grey) frequency bands. Both gamma and ripple power peak sharply at the time of the SPW, with gamma showing a ~60% increase and ripple ~15% above baseline. (d) SPW-replay coupling. The probability of observing a replay event (decoder P(odour) > 0.05) within 0-500 ms following a sharp wave, compared between observed data and circular-shift null (500 shuffles). Each dot is one recording. Two of three mice show significant SPW-replay co-occurrence, comparing observed coupling rate against the null distribution. (M1 p = 0.033, M2 p < 0.001). (e) Peri-SPW replay PSTH for the recording with the strongest coupling (M2). Blue: observed replay rate in 150 ms bins around each sharp wave. Grey: shuffle expected rate with 95% CI envelope. The observed replay rate peaks in the 0-500 ms window following the SPW, exceeding shuffle expectations.\", \"page\": 11, \"index\": 3, \"width\": 850, \"height\": 661}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-03-31-715372-v1/fig-004.webp\", \"caption\": \"Table 1. Odour stimulus identities. IDs are arbitrary codes based on Canberra distances in chemical space (e.g. C3f = Cluster 3, far).\", \"page\": 21, \"index\": 4, \"width\": 673, \"height\": 448}]"
motivation: 旨在厘清清醒经验与睡眠状态对神经表征随时间漂移的相对贡献及其定性差异。
method: 记录小鼠嗅觉皮层在气味暴露与睡眠循环中的单神经元活动，并开发低秩解码器来分解和追踪表征漂移模式。
result: 识别出四种正交漂移模式，发现睡眠通过去相关和旋转使表征轨迹发生逆转，并首次观测到伴随尖波的嗅觉重现。
conclusion: 神经表征漂移具有状态依赖性，睡眠在感官表征的离线重组中发挥着与清醒学习截然不同的关键作用。
---

## 摘要
神经表征随时间演变，但在线经验与睡眠等离线状态的相对贡献仍不清楚。在本研究中，我们记录了小鼠在觉醒气味暴露和睡眠循环过程中嗅觉皮层的单单元活动，并开发了一种低秩解码器来追踪表征漂移。我们识别出在不同时间尺度上运行的四个正交漂移模式，揭示了睡眠和觉醒驱动着性质截然不同的转换，这表明离线重组并非在线学习的简单延续。相反，睡眠引发了整体漂移轨迹的转向，其独特特征是气味表征的去相关和旋转的结合。我们还提供了嗅觉重现（olfactory replay）的首个证据，其发生在大约 2.5 倍的时间压缩下，并与局部产生的梨状皮层尖波相关。总之，这些发现表明表征漂移包含状态依赖的成分，并揭示了觉醒和睡眠对感觉表征变化的独特贡献。

## Abstract
Neural representations evolve over time, yet the relative contributions of online experience and offline states such as sleep remain unclear. Here, we recorded single-unit activity in the olfactory cortex of mice across cycles of awake odour exposure and sleep, and developed a low-rank decoder to track representational drift. We identified four orthogonal drift modes operating on distinct timescales, revealing that sleep and wake drive qualitatively different transformations, which indicates that offline reorganisation is not a simple continuation of online learning. Rather, sleep initiates an about-turn in the overall drift trajectory, which is uniquely characterised by a combination of decorrelation and rotation of odour representations. We also provide the first evidence for olfactory replay, occurring at ~2.5x temporal compression and associated with locally generated piriform cortex sharp waves. Together, these findings demonstrate that representational drift comprises state-dependent components, and reveal distinct contributions of wake and sleep to sensory representational change.

---

## 论文详细总结（自动生成）

这篇论文对神经科学中一个关键问题——“表征漂移（Representational Drift）”在不同生理状态下的演变进行了深入探讨。以下是对该研究的结构化总结：

### 1. 核心问题与整体含义
*   **核心问题**：神经元对相同刺激的反应会随时间发生变化（即表征漂移），但这种变化究竟是清醒时经验的简单延续，还是在睡眠期间经历了性质不同的重组？
*   **整体含义**：研究揭示了睡眠并非仅仅是清醒学习过程的“离线回放”或被动维持，而是对感官表征进行了主动的、定性的转换（如去相关和旋转）。这为理解大脑如何平衡记忆稳定性和灵活性提供了新的视角。

### 2. 核心方法论
*   **核心思想**：通过开发一种**低秩解码器（Low-rank decoder）**，将复杂的神经群体活动降维，从而能够定量追踪和分解表征随时间变化的轨迹。
*   **关键技术细节**：
    *   **漂移分解**：研究者将总的权重变化（$\Delta W$）分解为四个正交的漂移模式（D1-D4）。
    *   **模式识别**：利用奇异值分解（SVD）等数学手段，识别出在不同时间窗口（早起觉醒、觉醒-睡眠过渡、睡眠中、睡眠后）占主导地位的特定模式。
    *   **重现检测**：利用针对漂移校准后的解码器，在非快速眼动（NREM）睡眠期间搜索自发产生的、与气味刺激相关的神经序列。
    *   **时间压缩分析**：通过调整时间窗口，计算“序列性（Sequenceness）”，以确定重现事件相对于实际刺激的压缩倍数。

### 3. 实验设计
*   **实验对象与场景**：对小鼠嗅觉皮层（梨状皮层）进行单单元电生理记录。实验流程包括：清醒时的气味序列暴露（熟悉序列 F 和新异序列 N） $\rightarrow$ NREM 睡眠循环 $\rightarrow$ 睡眠后的气味暴露。
*   **对比基准（Benchmark）**：
    *   将睡眠期间的漂移轨迹与清醒期间的轨迹进行对比。
    *   使用**随机打乱（Shuffle）数据**作为零假设分布，验证嗅觉重现（Replay）的显著性。
    *   对比了熟悉序列与新异序列在漂移模式上的差异。

### 4. 资源与算力
*   论文中**未明确说明**具体的计算资源（如 GPU 型号或训练时长）。此类神经科学研究通常涉及大规模电生理数据的离线处理，重点在于信号处理算法和统计建模，而非大规模深度学习模型的训练。

### 5. 实验数量与充分性
*   **实验规模**：研究记录了 4 只小鼠（4 次深度记录）的单神经元活动。
*   **充分性评价**：
    *   虽然动物数量（N=4）在生物学实验中属于标准范围，但研究在每只动物身上都捕捉到了高度一致的四种漂移模式。
    *   **统计严谨性**：采用了 Holm 校正的配对 t 检验、Bonferroni 校正以及 500 次以上的循环打乱（Circular-shift）检验，确保了发现（尤其是嗅觉重现）的统计显著性。
    *   **多维度验证**：不仅分析了表征漂移，还结合了局部场电位（LFP）中的尖波（Sharp Waves）分析，增强了结论的可信度。

### 6. 主要结论与发现
*   **漂移的状态依赖性**：识别出四种模式。D1 与清醒相关；D2 和 D3 在睡眠期间激活，导致表征轨迹发生“U型转弯”或逆转。
*   **睡眠的独特作用**：睡眠引发了气味表征的**去相关（Decorrelation）**和**旋转（Rotation）**，使不同气味的神经表征变得更加独特，这证明睡眠在优化感官编码空间。
*   **首次发现嗅觉重现**：在 NREM 睡眠中观测到了气味序列的自发重现，其速度比实际呈现快约 **2.5 倍**。
*   **生理关联**：嗅觉重现与梨状皮层产生的**尖波（Sharp Waves）**在时间上高度耦合，类似于海马体中的重现机制。

### 7. 优点
*   **方法创新**：提出了一种分解表征漂移的新框架，能够区分“在线”和“离线”对神经元变化的贡献。
*   **科学突破**：填补了嗅觉系统是否存在“重现”现象的空白，并证明了睡眠对感官图谱的主动重组作用。
*   **分析深入**：不仅观察到了漂移，还通过几何视角（旋转、增益、相关性）解释了漂移的生物学意义。

### 8. 不足与局限
*   **样本量限制**：4 只小鼠的样本量虽然足以支持统计结论，但可能存在个体差异未被完全覆盖的风险。
*   **因果关系缺失**：研究主要是观察性的，尚未通过光遗传学等手段证明“抑制尖波”或“干扰睡眠”是否会直接阻止表征的去相关过程。
*   **区域局限性**：研究集中在嗅觉皮层，这种睡眠驱动的表征逆转模式是否普遍存在于视觉或听觉皮层尚待验证。

（完）
