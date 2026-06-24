---
title: BAYESIAN STATE-SPACE MODEL FOR JOINT INFERENCE OF OSCILLATORY DYNAMICS AND POINT-PROCESS COUPLING
title_zh: 贝叶斯状态空间模型用于振荡动力学与点过程耦合的联合推断
authors: "Zheng, B., Brincat, S., Donoghue, J., Miller, E., Brown, E."
date: 2026-06-19
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.15.732402v1.full.pdf"
tags: ["query:slp-ns"]
score: 6.0
evidence: 贝叶斯状态空间模型联合推断振荡动力学和尖峰场耦合，可用于睡眠神经科学研究
tldr: 尖峰时间与局部场电位振荡的相位耦合分析常受限于经典方法独立估计频谱。本文提出贝叶斯状态空间框架Joint SSMT，联合推断LFP谱图和尖峰-场耦合强度，通过潜在过程建模窄带振荡并利用伯努利-逻辑斯蒂模型耦合尖峰。仿真和麻醉数据表明模型能精确恢复耦合、去噪谱图并识别特定慢振荡频率。该方法提供更频率特异性的耦合估计和不确定性量化，优于经典PLV和SFC。
source: biorxiv
selection_source: fresh_fetch
motivation: 经典度量独立估计LFP频谱，未能利用尖峰时间信息提升耦合推断精度和频率特异性。
method: 提出贝叶斯状态空间模型，将窄带LFP视为连续时间潜在过程，并用伯努利-逻辑斯蒂模型连接尖峰序列。
result: 仿真中准确恢复耦合强度并去噪谱图；在麻醉数据中识别慢振荡频率耦合，在联想学习任务中揭示海马和前额叶的频率特异性耦合。
conclusion: Joint SSMT提供更频率特异的耦合估计和置信度量化，优于经典PLV和SFC。
---

## 摘要
在一系列行为和生理条件下，尖峰时间和局部场电位（LFP）振荡在特定频带内表现出相位耦合。经典测量如尖峰-场相干性（SFC）和相位锁定值（PLV）量化了这种耦合，但独立于尖峰时间估计LFP频谱。我们提出了Joint SSMT，一种贝叶斯状态空间框架，用于联合推断LFP频谱图和尖峰-场耦合强度。该模型将窄带LFP活动视为在连续时间中演化的潜在过程，通过伯努利-逻辑斯蒂模型将尖峰序列与复频谱状态联系起来。在模拟中，Joint SSMT准确恢复耦合强度，对频谱图进行去噪，并利用尖峰时间解析LFP中的精细时间结构。应用于丙泊酚麻醉数据时，该模型识别出特定慢振荡频率下的耦合，而SFC和PLV仅报告广泛的低频耦合。我们将Joint SSMT扩展到试验结构实验，并应用于联想学习任务期间的灵长类动物记录，揭示了海马和前额叶皮层中频率特定的耦合。我们还推导了SFC和PLV作为生成模型参数的闭式表达式。在模拟和两个灵长类数据集中，Joint SSMT提供了比经典PLV和SFC更频率特异性的耦合估计，并具有原理性的不确定性量化。

## Abstract
Under a range of behavioral and physiological conditions, spike times and local field potential (LFP) oscillations exhibit phase coupling within specific frequency bands. Classical measures such as spike-field coherence (SFC) and the phase-locking value (PLV) quantify this coupling but estimate the LFP spectrum independently of spike timing. We introduce Joint SSMT, a Bayesian state-space framework that jointly infers LFP spectrograms and spike-field coupling strength. The model treats narrowband LFP activity as a latent process evolving in continuous time, with spike trains linked to the complex spectral state through a Bernoulli-logistic model. In simulations, Joint SSMT accurately recovers coupling strength, denoises the spectrogram, and uses spike timing to resolve fine temporal structure in the LFP. Applied to propofol anesthesia data, the model identifies coupling at a specific slow-oscillation frequency where SFC and PLV report only broad low-frequency coupling. We extend Joint SSMT to trial-structured experiments and apply it to primate recordings during an associative learning task, revealing frequency-specific coupling in hippocampus and prefrontal cortex. We also derive closed-form expressions for SFC and PLV as functions of the generative model parameters. Across simulations and two primate datasets, Joint SSMT provides more frequency-specific coupling estimates with principled uncertainty quantification than classical PLV and SFC.