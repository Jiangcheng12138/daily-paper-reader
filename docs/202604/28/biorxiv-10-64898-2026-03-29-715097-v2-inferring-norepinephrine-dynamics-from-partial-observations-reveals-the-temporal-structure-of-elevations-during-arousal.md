---
title: Inferring norepinephrine dynamics from partial observations reveals the temporal structure of elevations during arousal
title_zh: 从部分观测中推断去甲肾上腺素动力学揭示了觉醒期间升高的时间结构
authors: "Neyhart, E., Munn, B. R., Zhou, N., Yang, P., Feng, J., Li, Y., Shine, J., Reimer, J."
date: 2026-04-20
pdf: "https://www.biorxiv.org/content/10.64898/2026.03.29.715097v2.full.pdf"
tags: ["query:slp-ns"]
score: 7.0
evidence: 觉醒期间的去甲肾上腺素动态
tldr: 本研究针对双光子成像中血流动力学伪影干扰去甲肾上腺素（NE）信号的问题，提出了一套分层推断框架。通过结合双通道记录、基于LSTM的深度学习模型以及仅依赖行为变量的预测方法，实现了对NE动态的精确校正和推断。研究揭示了皮层NE信号与行为强度呈正相关，且NE水平反映了蓝斑核输出的时间累积效应而非瞬时放电，为理解觉醒状态下的神经调制提供了新工具和新视角。
source: biorxiv
selection_source: fresh_fetch
motivation: 旨在解决双光子荧光成像中血流动力学伪影与去甲肾上腺素传感器信号重叠且难以消除的挑战。
method: 开发了一套分层框架，包括双通道参考校正、基于LSTM的后验去噪模型以及仅利用行为变量推断NE动态的方法。
result: 成功提取了高精度的NE信号，发现其强度随运动和瞳孔变化缩放，且在时间上表现为对蓝斑核轴突活动的积分而非瞬时追踪。
conclusion: 准确的血流动力学校正对于解释神经调制动态至关重要，研究揭示了皮层去甲肾上腺素信号在觉醒过程中的时间累积特性。
---

## 摘要
血流动力学伪影对基因编码报告基因的双光子荧光成像构成了重大挑战，特别是当相关测量的尺度与血管动力学的尺度相匹配时。对于血流动力学伪影与目标生物信号量级相当的传感器来说，这是一个严峻的挑战。然而，标准的校正方法（如等吸收点记录或重复实验）通常是不切实际的。在这里，我们介绍了一个分层框架，用于在不同记录信息水平下推断去甲肾上腺素（NE）动力学。首先，我们验证了在神经调节剂指示剂的同时使用惰性荧光报告基因进行双通道记录，可以在同一记录会话中实现直接的血流动力学校正。对于没有专用参考通道的情况，我们训练了一个基于 LSTM 的模型，该模型可以从记录的 NE 信号和行为变量中事后预测并消除血流动力学贡献。最后，我们展示了仅从行为变量中就可以恢复 NE 动力学的关键特征，即使在荧光记录不可用时也能提供神经调节状态的估计。这些方法通过在同一视野中对蓝斑（LC）去甲肾上腺素能轴突和胞外 NE 进行同步双光子成像，实现了轴突活动和神经调节剂释放的同步多光谱测量。皮层 NE 信号随行为强度呈梯度变化，并随运动持续时间和瞳孔扩大幅度而缩放。正如预期的那样，轴突活动先于环境 NE 水平的增加，但 NE 在运动过程中达到峰值较晚，并在轴突活动消退后保持升高，这表明胞外 NE 随时间整合了 LC 输出，而不是追踪瞬时的 LC 放电。总之，这些发现表明准确的血流动力学校正对于解释 NE 动力学至关重要，并揭示了皮层去甲肾上腺素信号传导时间结构的更清晰视图。

## Abstract
Hemodynamic artifacts present a significant challenge for two-photon fluorescence imaging of genetically encoded reporters, particularly when the timescale of relevant measurements matches those of vascular dynamics. This is an acute challenge for sensors in which the hemodynamic artifact is of comparable magnitude to the biological signal of interest. However, standard correction methods, such as isobestic recording or repeated experiments, are often impractical. Here we introduce a tiered framework for inferring norepinephrine (NE) dynamics across varying levels of recording information. First, we verify that dual-channel recording using an inert fluorescent reporter alongside the neuromodulator indicator enables direct hemodynamic correction within the same recording session. For contexts in which a dedicated reference channel is unavailable, we trained an LSTM-based model that predicts and removes hemodynamic contributions post-hoc from the recorded NE signal and behavioral variables. Finally, we show that key features of NE dynamics can be recovered from behavioral variables alone, providing an estimate of neuromodulatory state even when fluorescence recordings are unavailable. These methods enabled simultaneous multi-spectral measurements of axonal activity and neuromodulator release via simultaneous two-photon imaging of LC noradrenergic axons and extracellular NE in the same field of view. Cortical NE signals are graded with respect to behavioral intensity, scaling with both locomotion duration and pupil dilation amplitude. As expected, axonal activity precedes increases in ambient NE levels, but NE peaks later within a run and remains elevated after axonal activity has subsided, suggesting that extracellular NE integrates LC output over time rather than tracking instantaneous LC firing. Together, these findings demonstrate that accurate hemodynamic correction is essential for interpreting NE dynamics, and reveal a clearer view of the temporal structure of cortical norepinephrine signaling.