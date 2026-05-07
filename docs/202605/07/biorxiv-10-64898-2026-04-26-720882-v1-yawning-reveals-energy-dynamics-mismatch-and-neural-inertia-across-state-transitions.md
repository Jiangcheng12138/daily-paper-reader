---
title: Yawning reveals energy-dynamics mismatch and neural inertia across state transitions
title_zh: 打哈欠揭示了状态转换过程中的能量-动力学失配与神经惯性
authors: "Meng, X., Sun, Q., Li, M., Li, X., Liang, G., Qin, L., Tan, W."
date: 2026-04-29
pdf: "https://www.biorxiv.org/content/10.64898/2026.04.26.720882v1.full.pdf"
tags: ["query:slp-ns"]
score: 7.0
evidence: 觉醒状态转换过程中的神经动力学
tldr: 本研究通过对比格犬和人类在清醒及麻醉状态下的神经记录，探讨了打哈欠的神经动力学机制。研究发现打哈欠并非简单的被动反射，而是与一种被称为“能量-动力学失配”（EDM）的瞬态脑态特征紧密相关，表现为局部高频活动增加与全局网络灵活性下降。这一发现揭示了打哈欠在克服神经惯性、维持信息整合中的补偿作用，为监测意识状态转换和脑机接口应用提供了潜在的生物标志物。
source: biorxiv
selection_source: fresh_fetch
motivation: 旨在探究打哈欠在意识状态转换过程中的神经动力学特征，以理解其在脑网络组织变化中的作用。
method: 采用比格犬模型和人类临床数据，通过同步EEG/EMG记录及希尔伯特-黄变换（EMD-HHT）分析打哈欠前后的神经信号动态。
result: 识别出打哈欠时特有的“能量-动力学失配”特征，即局部伽马频段功率上升与全局网络灵活性下降并存，并据此实现了脑态解码。
conclusion: 打哈欠是应对网络不稳定性、克服神经惯性以维持大脑信息整合的一种主动补偿性神经过程，而非被动反射。
---

## 摘要
打哈欠是一种高度保守的行为，但其在觉醒状态转换过程中的神经动力学仍不为人所知。经典的反射模型无法解释在大规模脑网络组织变化期间打哈欠的精确时机。在本研究中，我们利用同步脑电图 (EEG)、肌电图 (EMG) 和运动学记录，研究了比格犬模型在清醒和丙泊酚麻醉期间打哈欠的神经特征。与丙泊酚相关的打哈欠表现出显著的时间不对称性，89.2% 的事件发生在麻醉苏醒期间。为了解析这些事件周围的快速神经动力学，我们应用了经验模态分解结合希尔伯特-黄变换 (EMD-HHT) 分析。在诱导、恢复和清醒过程中，打哈欠始终与局部和全局网络动力学之间的瞬时解耦相关：局部 γ 频段功率的短暂增加与网络灵活性的下降（通过瞬时频率波动性 IFV 量化）同时发生。我们将这种可重复的模式称为“能量-动力学失配”(EDM)。利用 EDM 特征的机器学习分类器能够可靠地解码打哈欠之前的脑状态。我们在麻醉诱导期间的一个独立人类队列中进一步验证了这一特征的存在。这些发现表明，打哈欠并非一种被动反射，而是与状态转换期间网络不稳定的时刻紧密相关。从计算角度来看，EDM 可能反映了一种瞬时的“控制努力”，旨在“神经惯性”存在的情况下保持信息整合。这种动态特征可能为监测觉醒转换、脑机接口 (BCI) 状态预警提供一种定量的生物标志物。

意义声明：打哈欠是一种普遍且在进化上保守的行为，但其神经基础仍然难以捉摸。通过在跨物种模型中使用高分辨率神经记录，我们证明了打哈欠并非被动反射，而是可靠地与一种独特的、瞬时的脑状态特征相吻合。具体而言，当局部高频皮层活动短暂增加而全局网络灵活性降低时，就会发生打哈欠——我们将这种模式称为“能量-动力学失配”(EDM)。我们认为 EDM 反映了在网络不稳定时刻参与的补偿性神经过程，这与克服神经惯性以保持信息整合相一致。通过识别这一保守的神经标记，本研究推进了对打哈欠的生物学理解，并为未来 BCI 中检测关键脑状态提供了一种潜在的生物标志物。

## Abstract
Yawning is a highly conserved behavior, yet its neural dynamics across arousal state transitions remain poorly understood. Classical reflex models fail to account for the precise timing of yawns during large-scale changes in brain network organization. Here, we investigated the neural signatures of yawning using simultaneous electroencephalography (EEG), electromyography (EMG), and kinematic recordings in a beagle model during wakefulness and propofol anesthesia. Propofol-associated yawning exhibited marked temporal asymmetry, with 89.2% of events occurring during emergence from anesthesia. To resolve the fast neural dynamics surrounding these events, we applied empirical mode decomposition coupled with the Hilbert-Huang transform (EMD-HHT) analyses. Across induction, recovery, and wakefulness, yawning was consistently associated with a transient decoupling between local and global network dynamics: a brief increase in local {gamma}-band power coincided with a drop in network flexibility, quantified by instantaneous frequency volatility; IFV). We termed this reproducible motif as "Energy-Dynamics Mismatch" (EDM). A machine learning classifier leveraging EDM features reliably decoded the brain state immediately preceding yawning. We further validated the presence of this signature in an independent human cohort during anesthesia induction. These findings indicate that yawning is not a passive reflex, but is tightly linked to moments of network instability during state transitions. From a computational perspective, EDG may reflect a transient "control effort" that preserves information integration in the presence of "neural inertia." This dynamic signature may provide a quantitative biomarker for monitoring arousal transitions brain-computer interface (BCI) interface state-alerting.

Significance StatementYawning is a ubiquitous and evolutionarily conserved behavior, yet its neural basis remains elusive. Using high-resolution neural recordings in a cross-species model, we show that yawning is not a passive reflex, but reliably coincides with a distinct, transient brain-state signature. Specifically, yawning occurs when local high-frequency cortical activity briefly increases while global network flexibility decreases - a pattern we term an "Energy-Dynamics Mismatch" (EDM). We propose that EDM reflects a compensatory neural process engaged during moments of network instability, consistent with overcoming neural inertia to preserve information integration. By identifying this conserved neural marker, this work advances the biological understanding of yawning and suggests a potential biomarker for detecting critical brain states in future BCI.