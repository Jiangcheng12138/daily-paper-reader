---
title: Compressed Cortical Input Separates Control from Dynamics in Striatum
title_zh: 压缩的皮层输入将纹状体中的控制与动力学分离
authors: "Kumar, S., Le Cauchois, M. B., Mathis, A., Duncker, L., Howlett, J. R., Mattar, M. G."
date: 2026-04-30
pdf: "https://www.biorxiv.org/content/10.1101/2025.09.05.674585v2.full.pdf"
tags: ["query:slp-ns"]
score: 6.0
evidence: 皮层纹状体控制与动力学的神经网络模型
tldr: 本研究探讨了背外侧纹状体（DLS）如何支持动作分块、时长估计和运动计时等多种时间敏感行为。作者提出皮层向纹状体的大规模投射汇聚（压缩）是关键机制，并构建了一个包含皮层和纹状体模块、通过低维噪声瓶颈连接的强化学习神经网络模型。研究发现，这种压缩导致了功能分离：皮层提供低维控制信号，而纹状体生成稳定的时间编码动力学。该模型统一了信息论与动力系统视角，解释了多种DLS相关的感觉运动行为。
source: biorxiv
selection_source: fresh_fetch
motivation: 旨在寻找一个统一的计算框架，以解释背外侧纹状体在动作分块、时长估计和运动计时等多种时间敏感行为中的作用。
method: 开发了一个皮层-纹状体神经网络模型，通过低维、有噪声的瓶颈连接两个循环模块，并利用强化学习进行训练。
result: 压缩机制使得皮层负责低维控制信号，而纹状体负责生成稳定的时间编码动力学，从而复现了多种DLS相关的行为特征。
conclusion: 研究表明皮层输入的解剖学压缩是实现控制与动力学分离的关键，为理解基底神经节的功能提供了统一的视角。
---

## 摘要
背外侧纹状体 (DLS) 支持多种时间敏感型行为——动作组块 (action chunking)、时长估计和运动计时——然而目前尚无统一框架能够解释所有这些现象。在此，我们提出皮层投射到纹状体的大规模汇聚提供了这样一个框架。我们开发了一个皮层-纹状体神经网络模型，其中循环皮层模块通过一个低维、有噪声的瓶颈与循环纹状体模块进行通信，整个系统通过强化学习进行训练。在三项与 DLS 相关的任务中，压缩产生了一种一致的计算基序 (computational motif)，即皮层提供低维控制信号，而纹状体生成稳定的时间编码动力学。这种分离产生了带有动作滑移 (action slipping) 的组块行为、具有刺激调制时间编码的强度偏向时长判断，以及定型的运动计时程序。对压缩皮层信号的扰动会因果性地改变行为，同时保留纹状体活动中的序列结构。总之，我们的结果统一了基底神经节功能的信息论和动力系统视角，将解剖学上的压缩与 DLS 中涉及的各种时间敏感型感觉运动行为联系起来。

## Abstract
The dorsolateral striatum (DLS) supports diverse time-sensitive behaviors--action chunking, duration estimation, and motor timing--yet no single framework is able to explain all of these phenomena. Here, we propose that the massive convergence of cortical projections onto the striatum provides such a framework. We develop a corticostriatal neural network model in which a recurrent cortical module communicates with a recurrent striatal module through a low-dimensional, noisy bottleneck, with the whole system trained via reinforcement learning. Across three DLS-associated tasks, compression produces a consistent computational motif whereby cortex provides low-dimensional control signals while the striatum generates stable, time-encoding dynamics. This separation gives rise to chunking behavior with action slipping, intensity-biased duration judgements with stimulus-modulated time coding, and stereotyped motor timing programs. Perturbation of the compressed cortical signal causally shifts behavior while preserving sequential structure in striatum activity. In sum, our results unify information-theoretic and dynamical systems perspectives of basal ganglia function to link anatomical compression to a variety of temporally-sensitive sensorimotor behaviors implicated in the DLS.