---
title: Inferring norepinephrine dynamics from partial observations reveals the temporal structure of elevations during arousal
title_zh: 从部分观测中推断去甲肾上腺素动态揭示了觉醒期间升高的时间结构
authors: "Neyhart, E., Munn, B. R., Zhou, N., Yang, P., Feng, J., Li, Y., Shine, J., Reimer, J."
date: 2026-04-20
pdf: "https://www.biorxiv.org/content/10.64898/2026.03.29.715097v2.full.pdf"
tags: ["query:slp-ns"]
score: 8.0
evidence: 觉醒过程中的去甲肾上腺素动力学
tldr: 针对双光子成像中去甲肾上腺素（NE）传感器受血流动力学伪影干扰的问题，本研究提出了一套分层推断框架。该框架包括双通道直接校正、基于LSTM的后期模型校正以及仅依赖行为变量的动态恢复方法。通过这些方法，研究揭示了皮层NE信号与行为强度成比例，且NE水平在时间上整合了蓝斑（LC）轴突的活动，而非仅仅追踪瞬时放电，为理解唤醒状态下的神经调制提供了更精确的视角。
source: biorxiv
selection_source: fresh_fetch
motivation: 旨在解决双光子成像中血流动力学伪影对去甲肾上腺素传感器信号的严重干扰，尤其是在缺乏标准校正手段的情况下。
method: 开发了一套分层框架，结合双通道记录、基于LSTM的深度学习模型以及行为变量分析来推断和校正NE动态。
result: 发现皮层NE信号强度与行为强度相关，且NE水平在时间上滞后于LC轴突活动并持续更久，表现出对神经输出的整合特性。
conclusion: 研究证明了精确的血流动力学校正对解释NE动态的必要性，并揭示了皮层去甲肾上腺素信号在唤醒过程中的时域结构。
---

## 摘要
血流动力学伪影对基因编码指示剂的双光子荧光成像构成了重大挑战，特别是当相关测量的尺度与血管动力学的尺度相匹配时。对于那些血流动力学伪影与目标生物信号量级相当的传感器来说，这是一个严峻的挑战。然而，标准的校正方法（如等吸收点记录或重复实验）通常难以实施。在这里，我们介绍了一个分层框架，用于在不同记录信息水平下推断去甲肾上腺素（

## Abstract
Hemodynamic artifacts present a significant challenge for two-photon fluorescence imaging of genetically encoded reporters, particularly when the timescale of relevant measurements matches those of vascular dynamics. This is an acute challenge for sensors in which the hemodynamic artifact is of comparable magnitude to the biological signal of interest. However, standard correction methods, such as isobestic recording or repeated experiments, are often impractical. Here we introduce a tiered framework for inferring norepinephrine (NE) dynamics across varying levels of recording information. First, we verify that dual-channel recording using an inert fluorescent reporter alongside the neuromodulator indicator enables direct hemodynamic correction within the same recording session. For contexts in which a dedicated reference channel is unavailable, we trained an LSTM-based model that predicts and removes hemodynamic contributions post-hoc from the recorded NE signal and behavioral variables. Finally, we show that key features of NE dynamics can be recovered from behavioral variables alone, providing an estimate of neuromodulatory state even when fluorescence recordings are unavailable. These methods enabled simultaneous multi-spectral measurements of axonal activity and neuromodulator release via simultaneous two-photon imaging of LC noradrenergic axons and extracellular NE in the same field of view. Cortical NE signals are graded with respect to behavioral intensity, scaling with both locomotion duration and pupil dilation amplitude. As expected, axonal activity precedes increases in ambient NE levels, but NE peaks later within a run and remains elevated after axonal activity has subsided, suggesting that extracellular NE integrates LC output over time rather than tracking instantaneous LC firing. Together, these findings demonstrate that accurate hemodynamic correction is essential for interpreting NE dynamics, and reveal a clearer view of the temporal structure of cortical norepinephrine signaling.