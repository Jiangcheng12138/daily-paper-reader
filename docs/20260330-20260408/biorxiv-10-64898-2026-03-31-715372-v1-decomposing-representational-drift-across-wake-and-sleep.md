---
title: Decomposing representational drift across wake and sleep
title_zh: 分解觉醒与睡眠过程中的表征漂移
authors: "Harris, J. J., Schaefer, A. T., Kollo, M."
date: 2026-04-02
pdf: "https://www.biorxiv.org/content/10.64898/2026.03.31.715372v1.full.pdf"
tags: ["query:slp-ns"]
score: 10.0
evidence: 清醒与睡眠状态下的神经表征和表征漂移
tldr: 本研究探讨了觉醒体验与睡眠状态对神经表征漂移的相对贡献。通过记录小鼠嗅觉皮层的单细胞活动并利用低秩解码器追踪表征变化，研究发现睡眠与觉醒驱动了性质截然不同的表征转换。睡眠并非觉醒学习的延续，而是引发了表征轨迹的转向，表现为去相关与旋转。此外，研究首次发现了嗅觉重现现象，揭示了睡眠在感官表征演变中的独特作用。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-03-31-715372-v1/fig-001.webp\", \"caption\": \"Figure 1. Odour representations undergo distinct transformations during wake and sleep. (a) Decoder weight matrices for a single odour (odour 1 of sequence F, mouse 2), showing similar baseline weights and 𝑊₀ end-of-session weights . Their difference corresponds to a small change. Neuronal units sorted by mean per 𝑊 𝑒𝑛𝑑 ∆𝑊 ∆𝑊 brain area. The colour scale (blue-white-red) is for negative to positive weights (identical colour scale used for all matrices in the panel). (b) The total change decomposes into four different drift modes D1-4. (Identical colour scale used for all matrices in the panel). (c) Normalised sigmoid activations for each mode in four mice. D1 (blue) activates during early wake, D2 (orange) and D3 (green) during the wake-sleep transition and sleep, and D4 (red) in post-sleep. Blue shading indicates the main NREM sleep block, odour sequences were played to the mice before and after sleep. (d) Relative amplitude of each mode. Bars: mean ± SEM across 4 recordings. *p < 0.05, Holm-corrected paired t-tests between mode pairs. (e) Fraction of each mode's drift amplitude attributable to the familiar (F1) sequence odours. All modes affect both sequences approximately equally. (f) Readout gain: cosine similarity between each mode's weight change and the baseline weights. D1 is significantly aligned with , indicating it scales the existing readout pattern. Stars: 𝑊₀ one-sample t-test vs zero, Bonferroni-corrected across 4 modes. (g) Rotation angle between and , in 𝑊₀ 𝑊₀ + ∆𝑊 𝑖 degrees. All modes produce significant rotation (**p < 0.01). (h) Odour decorrelation: change in mean pairwise Pearson correlation between odour weight vectors when each mode is applied (positive = increased distinctness). (i) Drift trajectory through weight space for each recording across the session. The four weight vectors are projected into ∆𝑊(τ) 2D via SVD. The total drift direction is aligned horizontally. Coloured dots mark drift mode midpoints. Tick marks show τ values at 0.25 intervals. All mice show a similar path: D1 starts roughly along the baseline direction, then D2/D3 bend the trajectory during sleep, with D4 adding a minor late component.\", \"page\": 7, \"index\": 1, \"width\": 783, \"height\": 871}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-03-31-715372-v1/fig-002.webp\", \"caption\": \"Figure 2. Temporally compressed odour replay during NREM sleep. (a) Example stimulus presentations (left) and NREM replay events (right) for the novel (N, left pair) and familiar (F, right pair) odour sequences. Top rows: true odour identity; bottom rows: decoded probability P(odour) from the drift decoder, displayed as colour-coded RGBA heatmaps (2-bin boxcar smoothed). Each row corresponds to one odour in the sequence; rows are grouped by sequence (N1-N4, F1-F4). Dashed lines mark stimulus onset/offset (stim panels) or first/last detected replay peak (replay panels). During wake stimulation, the decoder produces sequential activations matching the presented odour order. During NREM, spontaneous reactivations recapitulate the learned sequence at compressed timescales. (b) Transition matrices showing the regression weight from each odour's decoded probability at time to every𝑡 other odour at time (ridge regression), computed at 2.5× temporal compression ( =400ms). Dashed𝑡 + ∆𝑡 ∆𝑡 boxes highlight forward transitions along the trained sequence order. NREM shows stronger within-sequence forward structure than wake or circular-shifted channel shuffle (mean of 50 shuffles). (c) Forward (filled circles) and backward (open circles) transition strengths per mouse at 2.5× compression, for F1 (red) and N1 (blue) sequences separately. Horizontal grey lines show the 95th percentile of the circular-shift null distribution (500 shuffles). Forward transitions consistently exceed backward and shuffle in all mice. (d) Sequenceness (forward − backward transition strength) across temporal compression factors (1×-10×) for both sequences (F red, N blue). Lines: individual mice; shading: SEM. Peak sequenceness occurs at 2-3× compression for both sequences, corresponding to replay timescales of 300-500 ms per odour (vs 1 s during wake presentation). (e) Statistical significance of sequential replay structure at 2.5× compression, shown for three levels of sequence analysis: pairwise transitions (adjacent odour pairs), 3-element subsequences, and full 4-element sequences. Each dot is one mouse × sequence combination.\", \"page\": 9, \"index\": 2, \"width\": 960, \"height\": 756}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-03-31-715372-v1/fig-003.webp\", \"caption\": \"Figure 3. Piriform sharp waves during NREM sleep are associated with odour replay. (a) Example piriform sharp waves (SPWs) detected during NREM sleep. Top: raw LFP from a piriform channel showing the sharp wave deflection (negative polarity, peak amplitude annotated in µV). Middle: 80-140 Hz filtered signal showing co-occurring fast gamma activity. Bottom: 160-190 Hz filtered signal showing ripple-band oscillations. (b) SPW rate across behavioural states. Box plots show the distribution across recordings (n = 3) for pre-sleep wake, NREM, and post-sleep wake. Paired lines connect the same recording. SPW rate is elevated during NREM relative to wake periods. (c) Peri-SPW triggered power in gamma (80-140 Hz, blue) and ripple (160-190 Hz, grey) frequency bands. Both gamma and ripple power peak sharply at the time of the SPW, with gamma showing a ~60% increase and ripple ~15% above baseline. (d) SPW-replay coupling. The probability of observing a replay event (decoder P(odour) > 0.05) within 0-500 ms following a sharp wave, compared between observed data and circular-shift null (500 shuffles). Each dot is one recording. Two of three mice show significant SPW-replay co-occurrence, comparing observed coupling rate against the null distribution. (M1 p = 0.033, M2 p < 0.001). (e) Peri-SPW replay PSTH for the recording with the strongest coupling (M2). Blue: observed replay rate in 150 ms bins around each sharp wave. Grey: shuffle expected rate with 95% CI envelope. The observed replay rate peaks in the 0-500 ms window following the SPW, exceeding shuffle expectations.\", \"page\": 11, \"index\": 3, \"width\": 850, \"height\": 661}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-03-31-715372-v1/fig-004.webp\", \"caption\": \"Table 1. Odour stimulus identities. IDs are arbitrary codes based on Canberra distances in chemical space (e.g. C3f = Cluster 3, far).\", \"page\": 21, \"index\": 4, \"width\": 673, \"height\": 448}]"
motivation: 旨在厘清觉醒时的在线经验与睡眠时的离线状态如何分别影响神经表征随时间的演变（即表征漂移）。
method: 记录小鼠嗅觉皮层在气味暴露与睡眠循环中的单神经元活动，并开发低秩解码器来分解和追踪不同时间尺度下的表征漂移模式。
result: 发现了四种正交的漂移模式，证实睡眠引发了与觉醒截然不同的表征转向，并首次观测到伴随皮层尖波的嗅觉重现现象。
conclusion: 神经表征漂移具有状态依赖性，睡眠通过独特的重组机制而非简单的学习延续，在感官表征的长期演变中发挥关键作用。
---

## 摘要
神经表征随时间演变，但在线经验与睡眠等离线状态的相对贡献仍不清楚。在本研究中，我们记录了小鼠在觉醒气味暴露和睡眠循环过程中嗅觉皮层的单单元活动，并开发了一种低秩解码器来追踪表征漂移。我们识别出四种在不同时间尺度上运行的正交漂移模式，揭示了睡眠和觉醒驱动着性质截然不同的转换，这表明离线重组并非在线学习的简单延续。相反，睡眠引发了整体漂移轨迹的转向，其独特特征是气味表征的去相关和旋转的结合。我们还提供了嗅觉重现（olfactory replay）的首个证据，其发生在大约 2.5 倍的时间压缩下，并与局部产生的梨状皮层尖波相关。总之，这些发现证明了表征漂移包含状态依赖的成分，并揭示了觉醒和睡眠对感觉表征变化的独特贡献。

## Abstract
Neural representations evolve over time, yet the relative contributions of online experience and offline states such as sleep remain unclear. Here, we recorded single-unit activity in the olfactory cortex of mice across cycles of awake odour exposure and sleep, and developed a low-rank decoder to track representational drift. We identified four orthogonal drift modes operating on distinct timescales, revealing that sleep and wake drive qualitatively different transformations, which indicates that offline reorganisation is not a simple continuation of online learning. Rather, sleep initiates an about-turn in the overall drift trajectory, which is uniquely characterised by a combination of decorrelation and rotation of odour representations. We also provide the first evidence for olfactory replay, occurring at ~2.5x temporal compression and associated with locally generated piriform cortex sharp waves. Together, these findings demonstrate that representational drift comprises state-dependent components, and reveal distinct contributions of wake and sleep to sensory representational change.

---

## 论文详细总结（自动生成）

这是一份关于论文《Decomposing representational drift across wake and sleep》（分解觉醒与睡眠过程中的表征漂移）的深度结构化总结：

### 1. 核心问题与整体含义
*   **核心问题**：神经表征（Neural Representations）会随时间发生自发演变，这种现象被称为“表征漂移”。研究旨在厘清：这种漂移是由**觉醒时的在线经验**驱动的，还是由**睡眠时的离线处理**驱动的？睡眠是仅仅延续了觉醒时的学习过程，还是引入了独特的变换？
*   **整体含义**：该研究揭示了睡眠在感官系统（嗅觉皮层）中并非被动的数据存储，而是主动的表征重组过程。它首次证明了睡眠和觉醒对神经轨迹的贡献在性质上是不同的，并发现了嗅觉领域的“重现”（Replay）现象。

### 2. 方法论：核心思想与技术细节
*   **低秩解码器（Low-rank Decoder）**：研究者开发了一种新型解码框架，用于在不假设漂移形式的情况下追踪神经活动的变化。
*   **漂移分解（Drift Decomposition）**：
    *   通过对解码器权重矩阵随时间的变化进行奇异值分解（SVD），将总漂移分解为四个正交的“漂移模式”（Modes D1-D4）。
    *   **D1**：主要在早期觉醒阶段激活，表现为现有读出模式的缩放（Gain control）。
    *   **D2 & D3**：在觉醒向睡眠过渡及睡眠期间激活，导致表征轨迹的显著转向。
    *   **D4**：在睡眠后的觉醒阶段激活。
*   **重现检测算法**：利用训练好的解码器在睡眠期间的自发活动中寻找与气味序列匹配的概率峰值，并使用岭回归（Ridge Regression）计算转移矩阵，以评估序列的压缩重现。

### 3. 实验设计
*   **实验对象与场景**：对小鼠的梨状皮层（Piriform Cortex）进行单单元电生理记录。实验流程包括：初始气味暴露（熟悉序列 F 和新异序列 N）→ 长时间睡眠（NREM/REM）→ 睡眠后气味暴露。
*   **对比基准（Benchmark）**：
    *   **状态对比**：对比觉醒（Wake）与非快速眼动睡眠（NREM）。
    *   **序列对比**：对比熟悉序列与新序列的漂移差异。
    *   **统计基准**：使用“循环位移混淆测试”（Circular-shift null distribution）作为评估重现显著性的基准。
*   **关键指标**：余弦相似度（衡量旋转）、皮尔逊相关系数（衡量去相关）、序列性（Sequenceness，前向减去后向转移强度）。

### 4. 资源与算力
*   **算力说明**：论文中未明确提及具体的 GPU 型号、数量或训练时长。
*   **数据规模**：实验涉及 4 只小鼠的深度电生理记录，包含数百个单神经元在数小时内的连续活动数据。计算压力主要集中在解码器的迭代训练和大规模重现检测的置换检验（Shuffle tests）上。

### 5. 实验数量与充分性
*   **实验规模**：研究基于 4 组高质量的长期记录（每组包含完整的觉醒-睡眠循环）。
*   **充分性评估**：
    *   **多维度分析**：不仅分析了宏观的漂移轨迹，还深入到了局部场电位（LFP）中的尖波（Sharp Waves）与重现的关联。
    *   **统计严谨性**：采用了 Holm 校正、Bonferroni 校正以及大量的 Shuffle 检验，确保发现的模式非随机产生。
    *   **一致性**：所有 4 只小鼠在漂移模式的演变轨迹上表现出高度的一致性，增强了结论的可信度。

### 6. 主要结论与发现
*   **睡眠驱动独特变换**：睡眠并非觉醒学习的简单延续，而是引发了表征轨迹的“转向”。睡眠期间的漂移（D2/D3）表现为气味表征的**去相关**（增强区分度）和**旋转**。
*   **首次发现嗅觉重现**：在 NREM 睡眠中观测到了气味序列的自发重现，其时间压缩比约为 **2.5 倍**（每种气味约 300-500ms，觉醒时为 1s）。
*   **皮层尖波关联**：梨状皮层会产生类似于海马体的尖波（SPWs），且这些尖波与嗅觉重现事件在时间上高度耦合。

### 7. 优点
*   **创新性工具**：开发的低秩解码分解方法为研究神经群体动力学提供了一个强大的通用框架。
*   **科学突破**：打破了“重现主要存在于海马体/空间导航系统”的局限，将其扩展到了感觉皮层和嗅觉领域。
*   **精细分解**：成功将复杂的表征漂移拆解为具有生物学意义的时间模式，使抽象的“漂移”变得可量化、可解释。

### 8. 不足与局限
*   **样本量限制**：虽然单细胞记录数据量大，但动物个体数量（n=4）相对较少，可能存在个体差异风险。
*   **因果性验证缺失**：研究主要基于相关性观察（如尖波与重现的相关），尚未通过光遗传学等手段干扰睡眠或尖波来验证其对表征漂移的因果影响。
*   **区域局限**：研究集中在梨状皮层，尚不清楚其他感觉皮层（如视觉、听觉）是否遵循相同的睡眠漂移逻辑。

（完）
