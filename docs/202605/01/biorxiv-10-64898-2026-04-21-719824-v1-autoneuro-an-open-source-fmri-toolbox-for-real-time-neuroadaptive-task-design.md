---
title: "AutoNeuro: An Open-Source fMRI Toolbox for Real-Time Neuroadaptive Task Design"
title_zh: AutoNeuro：用于实时神经自适应任务设计的开源 fMRI 工具箱
authors: "Haydock, D., Sherwood, O., Razin, R., Dick, F., Leech, R."
date: 2026-04-23
pdf: "https://www.biorxiv.org/content/10.64898/2026.04.21.719824v1.full.pdf"
tags: ["query:slp-ns"]
score: 7.0
evidence: 用于实时神经自适应任务设计的fMRI工具箱
tldr: AutoNeuro是一个开源的实时fMRI框架，旨在解决现有闭环神经影像系统复杂且缺乏灵活性等问题。该系统集成了数据采集、预处理、特征提取及自适应实验控制，通过贝叶斯优化算法动态调整任务参数，以最大化用户定义的脑活动目标函数。实验证明，AutoNeuro能在实时约束下稳定运行，支持假设驱动的优化和大规模实验空间的探索，为神经自适应任务设计提供了灵活的工具。
source: biorxiv
selection_source: fresh_fetch
motivation: 现有的实时fMRI方法受限于复杂的硬件需求和缺乏灵活的闭环框架，且大多仅侧重于神经反馈设计。
method: 开发了AutoNeuro开源框架，利用低延迟模块化流水线处理fMRI数据，并结合贝叶斯优化代理在实验空间内动态选择任务条件。
result: 实验表明系统能在实时处理约束下稳定运行，并成功通过自适应采样获得了脑部反应的连续映射。
conclusion: AutoNeuro为闭环神经影像研究提供了一个灵活且高效的平台，支持对复杂实验空间进行假设驱动的优化和探索。
---

## 摘要
实时功能磁共振成像 (fMRI) 为自适应研究脑功能提供了一种强大的手段，能够根据持续的神经活动动态更新实验参数。然而，目前的方法仍受限于复杂的基础设施要求、定制化实现以及缺乏灵活的闭环神经影像框架，且许多方法主要集中在神经反馈实验设计上。在此，我们介绍了 AutoNeuro，这是一个用于实时 fMRI 数据获取、预处理、特征提取和自适应实验控制的开源框架。AutoNeuro 直接连接到 MRI 扫描仪，在重建切片生成后立即接收，并将其流式传输到专为低延迟处理设计的模块化分析流水线中。神经特征在采集的时间分辨率下进行估计，并传递给贝叶斯优化智能体，该智能体通过选择任务条件来最大化用户定义的目标函数。实验条件在有界的“实验空间”内表示，允许在统一坐标系下探索异质条件。我们在实时 fMRI 实验中演示了 AutoNeuro，在该实验中，系统自适应地采样任务条件，以获取大脑对实验空间内一系列条件的反应连续图谱。该系统在实时预处理和分析的时间约束内运行，在迭代过程中保持稳定的模型估计，并收敛至与测量的脑指标最相关的实验条件。这些结果确立了 AutoNeuro 作为一个灵活的闭环神经影像平台，支持假设驱动的优化以及跨大型实验空间的脑指标探索性映射。

## Abstract
Real-time functional magnetic resonance imaging (fMRI) offers a powerful means of studying brain function adaptively, enabling experimental parameters to be updated dynamically in response to ongoing neural activity. However, current approaches remain limited by complex infrastructure requirements, bespoke implementations, and a lack of flexible frameworks for closed-loop neuroimaging, with many primarily focusing on neurofeedback experimental designs. Here we present AutoNeuro, an open-source framework for real-time fMRI acquisition, preprocessing, feature extraction, and adaptive experimental control. AutoNeuro connects directly to the MRI scanner, receiving reconstructed slices as soon as they become available, and streams them into a modular analysis pipeline designed for low-latency processing. Neural features are estimated at the temporal resolution of acquisition and are passed to a Bayesian optimisation agent that selects task conditions to maximise a user-defined objective function.

Experimental conditions are represented within a bounded "experiment space", allowing heterogeneous conditions to be explored within a common coordinate system. We demonstrate AutoNeuro in a real-time fMRI experiment in which the system adaptively sampled task conditions to obtain a continuous map of brain response to the range of conditions contained within the experimental space. The system operated within the temporal constraints of real-time preprocessing and analysis, maintaining stable model estimates across iterations, converging on experimental conditions most relevant to the measured brain metric. These results establish AutoNeuro as a flexible platform for closed-loop neuroimaging, supporting hypothesis-driven optimisation as well as exploratory mapping of brain metrics across large experimental spaces.