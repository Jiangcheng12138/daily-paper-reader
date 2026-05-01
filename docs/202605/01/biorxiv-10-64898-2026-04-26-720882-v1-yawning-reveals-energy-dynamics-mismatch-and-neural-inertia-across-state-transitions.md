---
title: Yawning reveals energy-dynamics mismatch and neural inertia across state transitions
title_zh: 打哈欠揭示了状态转换过程中的能量-动力学失配与神经惯性
authors: "Meng, X., Sun, Q., Li, M., Li, X., Liang, G., Qin, L., Tan, W."
date: 2026-04-29
pdf: "https://www.biorxiv.org/content/10.64898/2026.04.26.720882v1.full.pdf"
tags: ["query:slp-ns"]
score: 8.0
evidence: 觉醒状态转换过程中的神经动力学
tldr: 本研究通过比格犬模型和人类临床数据，结合EEG、EMG及EMD-HHT分析，探讨了打哈欠在觉醒状态转换中的神经动力学。研究发现打哈欠并非简单的反射，而是与“能量-动力学失配”（EDM）密切相关，即局部高频功率增加与全局网络灵活性下降的短暂解耦。这一发现揭示了打哈欠是克服“神经惯性”、维持信息整合的计算努力，为监测意识状态转换提供了新的生物标志物。
source: biorxiv
selection_source: fresh_fetch
motivation: 旨在探究打哈欠在脑网络组织大规模变化（如麻醉苏醒）过程中的精确神经动力学机制。
method: 采用比格犬模型进行同步电生理记录，并利用EMD-HHT分析及机器学习分类器，在人类队列中进行验证。
result: 发现打哈欠伴随着局部伽马频段功率上升与全局瞬时频率波动下降的“能量-动力学失配”特征。
conclusion: 打哈欠是与网络不稳定性紧密相关的动态标志，反映了在状态转换中克服神经惯性以维持信息整合的控制努力。
---

## 摘要
打哈欠是一种高度保守的行为，但其在觉醒状态转换过程中的神经动力学仍不为人所知。经典的反射模型无法解释在大脑网络组织发生大规模变化期间打哈欠的精确时机。在本研究中，我们利用同步脑电图（EEG）、肌电图（EMG）和运动学记录，研究了比格犬模型在清醒和丙泊酚麻醉期间打哈欠的神经特征。与丙泊酚相关的打哈欠表现出显著的时间不对称性，89.2% 的事件发生在麻醉苏醒期间。为了解析这些事件周围的快速神经动力学，我们应用了经验模态分解结合希尔伯特-黄变换（EMD-HHT）分析。在诱导、恢复和清醒过程中，打哈欠始终与局部和全局网络动力学之间的瞬时解耦相关：局部 γ 频段功率的短暂增加与网络灵活性的下降（通过瞬时频率波动性 IFV 量化）同时发生。我们将这种可重复的模式称为“能量-动力学失配”（EDM）。利用 EDM 特征的机器学习分类器可靠地解码了紧接打哈欠之前的大脑状态。我们进一步在麻醉诱导期间的一个独立人类队列中验证了这一特征的存在。这些发现表明，打哈欠并非一种被动反射，而是与状态转换期间网络不稳定的时刻紧密相关。从计算角度来看，EDM 可能反映了一种瞬时的“控制努力”，在存在“神经惯性”的情况下维持信息整合。这种动态特征可能为监测觉醒转换、脑机接口（BCI）状态预警提供一种定量的生物标志物。

## Abstract
Yawning is a highly conserved behavior, yet its neural dynamics across arousal state transitions remain poorly understood. Classical reflex models fail to account for the precise timing of yawns during large-scale changes in brain network organization. Here, we investigated the neural signatures of yawning using simultaneous electroencephalography (EEG), electromyography (EMG), and kinematic recordings in a beagle model during wakefulness and propofol anesthesia. Propofol-associated yawning exhibited marked temporal asymmetry, with 89.2% of events occurring during emergence from anesthesia. To resolve the fast neural dynamics surrounding these events, we applied empirical mode decomposition coupled with the Hilbert-Huang transform (EMD-HHT) analyses. Across induction, recovery, and wakefulness, yawning was consistently associated with a transient decoupling between local and global network dynamics: a brief increase in local {gamma}-band power coincided with a drop in network flexibility, quantified by instantaneous frequency volatility; IFV). We termed this reproducible motif as "Energy-Dynamics Mismatch" (EDM). A machine learning classifier leveraging EDM features reliably decoded the brain state immediately preceding yawning. We further validated the presence of this signature in an independent human cohort during anesthesia induction. These findings indicate that yawning is not a passive reflex, but is tightly linked to moments of network instability during state transitions. From a computational perspective, EDG may reflect a transient "control effort" that preserves information integration in the presence of "neural inertia." This dynamic signature may provide a quantitative biomarker for monitoring arousal transitions brain-computer interface (BCI) interface state-alerting.