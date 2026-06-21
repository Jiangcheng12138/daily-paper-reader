---
title: BAYESIAN STATE-SPACE MODEL FOR JOINT INFERENCE OF OSCILLATORY DYNAMICS AND POINT-PROCESS COUPLING
title_zh: 振荡动态与点过程耦合的贝叶斯状态空间联合推断模型
authors: "Zheng, B., Brincat, S., Donoghue, J., Miller, E., Brown, E."
date: 2026-06-19
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.15.732402v1.full.pdf"
tags: ["query:slp-ns"]
score: 6.0
evidence: 神经振荡状态空间模型睡眠
tldr: 尖峰时间与神经振荡的相位耦合是理解信息处理的关键，但经典测量尖峰场相干（SFC）和锁相值（PLV）独立估计频谱与耦合，丢失了联合信息。本文提出Joint SSMT贝叶斯状态空间模型，联合推断局部场电位频谱和尖峰-场耦合强度，将窄带LFP动力学视为潜状态并通过伯努利-逻辑斯蒂克回归与点过程耦合。在模拟和丙泊酚麻醉、联想学习任务两个灵长类数据集上，该方法准确恢复频率特异性耦合，并利用尖峰时间提高局部场电位的时间分辨率，优于经典方法。相比尖峰场相干和锁相值，Joint SSMT提供更频率特异的耦合估计和贝叶斯不确定性量化。
source: biorxiv
selection_source: fresh_fetch
motivation: 经典耦合测量方法独立估计频谱与耦合，无法利用尖峰时间信息，联合模型可提供更频率特异性的估计。
method: 建立贝叶斯状态空间模型，将窄带LFP作为潜状态，通过Bernoulli-logistic模型与点过程耦合，联合推断频谱和耦合强度。
result: 在模拟和丙泊酚麻醉、联想学习任务数据集上，Joint SSMT准确恢复频率特异性耦合，优于SFC和PLV。
conclusion: Joint SSMT提供频率特异性耦合估计和贝叶斯不确定性量化，适用于多种实验范式。
---

## 摘要
在多种行为和生理条件下，尖峰时间与局部场电位（LFP）振荡在特定频带内表现出相位耦合。经典指标如尖峰-场相干性（SFC）和锁相值（PLV）可量化该耦合，但估计LFP频谱时独立于尖峰时间。我们提出联合SSMT，一种贝叶斯状态空间框架，可联合推断LFP频谱图与尖峰-场耦合强度。该模型将窄带LFP活动视为连续时间演化的潜在过程，尖峰序列通过伯努利-逻辑模型与复频谱状态相关联。模拟实验中，联合SSMT准确恢复耦合强度、去噪频谱图，并利用尖峰时间解析LFP中的精细时间结构。应用于丙泊酚麻醉数据时，模型识别出特定慢振荡频率处的耦合，而SFC和PLV仅报告宽泛的低频耦合。我们将联合SSMT扩展到试验结构化实验，并应用于联想学习任务中的灵长类记录，揭示了海马体和前额叶皮层中的频率特异性耦合。我们还推导了SFC和PLV作为生成模型参数函数的闭合表达式。在模拟实验和两个灵长类数据集中，联合SSMT比经典PLV和SFC提供更频率特异的耦合估计，并带有合理的不确定性量化。

## Abstract
Under a range of behavioral and physiological conditions, spike times and local field potential (LFP) oscillations exhibit phase coupling within specific frequency bands. Classical measures such as spike--field coherence (SFC) and the phase-locking value (PLV) quantify this coupling but estimate the LFP spectrum independently of spike timing. We introduce Joint SSMT, a Bayesian state-space framework that jointly infers LFP spectrograms and spike--field coupling strength. The model treats narrowband LFP activity as a latent process evolving in continuous time, with spike trains linked to the complex spectral state through a Bernoulli--logistic model. In simulations, Joint SSMT accurately recovers coupling strength, denoises the spectrogram, and uses spike timing to resolve fine temporal structure in the LFP. Applied to propofol anesthesia data, the model identifies coupling at a specific slow-oscillation frequency where SFC and PLV report only broad low-frequency coupling. We extend Joint SSMT to trial-structured experiments and apply it to primate recordings during an associative learning task, revealing frequency-specific coupling in hippocampus and prefrontal cortex. We also derive closed-form expressions for SFC and PLV as functions of the generative model parameters. Across simulations and two primate datasets, Joint SSMT provides more frequency-specific coupling estimates with principled uncertainty quantification than classical PLV and SFC.