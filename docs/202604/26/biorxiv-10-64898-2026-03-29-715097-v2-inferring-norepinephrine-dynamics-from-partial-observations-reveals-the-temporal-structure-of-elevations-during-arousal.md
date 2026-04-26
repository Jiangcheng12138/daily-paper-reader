---
title: Inferring norepinephrine dynamics from partial observations reveals the temporal structure of elevations during arousal
title_zh: 从部分观测中推断去甲肾上腺素动力学，揭示了觉醒期间其升高的时域结构
authors: "Neyhart, E., Munn, B. R., Zhou, N., Yang, P., Feng, J., Li, Y., Shine, J., Reimer, J."
date: 2026-04-20
pdf: "https://www.biorxiv.org/content/10.64898/2026.03.29.715097v2.full.pdf"
tags: ["query:slp-ns"]
score: 7.0
evidence: 觉醒过程中的去甲肾上腺素动态
tldr: 本研究针对双光子成像中去甲肾上腺素（NE）传感器易受血流动力学伪影干扰的问题，提出了一套分层推断框架。该框架包含双通道直接校正、基于LSTM模型的后期去噪以及仅凭行为变量预测NE动态的方法。通过这些技术，研究揭示了皮层NE信号与行为强度的相关性，并发现NE水平是对蓝斑核轴突活动的随时间累积而非瞬时追踪，为理解唤醒状态下的神经调节提供了新视角。
source: biorxiv
selection_source: fresh_fetch
motivation: 解决双光子成像中血流动力学伪影对去甲肾上腺素传感器信号的干扰，尤其是在缺乏标准校正手段的情况下。
method: 提出包含双通道记录校正、LSTM深度学习模型去噪以及基于行为变量推断NE动态的分层分析框架。
result: 发现皮层NE水平随运动时长和瞳孔扩大程度分级变化，且NE信号表现为对蓝斑核轴突活动的随时间积分而非实时同步。
conclusion: 准确的血流动力学校正对解析神经递质动态至关重要，研究揭示了去甲肾上腺素在唤醒期间独特的时域特征。
---

## 摘要
血流动力学伪影对基因编码报告基因的双光子荧光成像构成了重大挑战，特别是当相关测量的尺度与血管动力学的尺度相匹配时。对于那些血流动力学伪影与目标生物信号强度相当的传感器来说，这是一个严峻的挑战。然而，标准的校正方法（如等吸收点记录或重复实验）通常是不切实际的。在此，我们介绍了一个分层框架，用于在不同记录信息水平下推断去甲肾上腺素（NE）动力学。首先，我们验证了在神经调节物质指示剂的同时使用惰性荧光报告基因进行双通道记录，能够在同一记录会话中实现直接的血流动力学校正。对于没有专用参考通道的情况，我们训练了一个基于 LSTM 的模型，该模型可以从记录的 NE 信号和行为变量中事后预测并移除血流动力学贡献。最后，我们展示了仅从行为变量中即可恢复 NE 动力学的关键特征，即使在荧光记录不可用时也能提供神经调节状态的估计。这些方法通过在同一视野内对蓝斑（LC）去甲肾上腺素能轴突和胞外 NE 进行同步双光子成像，实现了轴突活动和神经调节物质释放的同步多光谱测量。皮层 NE 信号随行为强度呈梯度变化，并随运动持续时间和瞳孔扩大幅度而缩放。正如预期的那样，轴突活动先于环境 NE 水平的升高，但 NE 在运动过程中达到峰值的时间较晚，并在轴突活动消退后仍保持高水平，这表明胞外 NE 是随时间整合了 LC 的输出，而非追踪瞬时的 LC 放电。总之，这些研究结果表明，准确的血流动力学校正对于解释 NE 动力学至关重要，并揭示了皮层去甲肾上腺素信号传导时域结构的更清晰视图。

## Abstract
Hemodynamic artifacts present a significant challenge for two-photon fluorescence imaging of genetically encoded reporters, particularly when the timescale of relevant measurements matches those of vascular dynamics. This is an acute challenge for sensors in which the hemodynamic artifact is of comparable magnitude to the biological signal of interest. However, standard correction methods, such as isobestic recording or repeated experiments, are often impractical. Here we introduce a tiered framework for inferring norepinephrine (NE) dynamics across varying levels of recording information. First, we verify that dual-channel recording using an inert fluorescent reporter alongside the neuromodulator indicator enables direct hemodynamic correction within the same recording session. For contexts in which a dedicated reference channel is unavailable, we trained an LSTM-based model that predicts and removes hemodynamic contributions post-hoc from the recorded NE signal and behavioral variables. Finally, we show that key features of NE dynamics can be recovered from behavioral variables alone, providing an estimate of neuromodulatory state even when fluorescence recordings are unavailable. These methods enabled simultaneous multi-spectral measurements of axonal activity and neuromodulator release via simultaneous two-photon imaging of LC noradrenergic axons and extracellular NE in the same field of view. Cortical NE signals are graded with respect to behavioral intensity, scaling with both locomotion duration and pupil dilation amplitude. As expected, axonal activity precedes increases in ambient NE levels, but NE peaks later within a run and remains elevated after axonal activity has subsided, suggesting that extracellular NE integrates LC output over time rather than tracking instantaneous LC firing. Together, these findings demonstrate that accurate hemodynamic correction is essential for interpreting NE dynamics, and reveal a clearer view of the temporal structure of cortical norepinephrine signaling.