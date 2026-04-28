---
title: "Deep-learning-assisted simulation of a cortical circuit: integrating anatomy, physiology and function"
title_zh: 深度学习辅助的皮层环路模拟：整合解剖学、生理学与功能
authors: "Ito, S., Haufler, D., Fraile, J. G., Dai, K., Aman, J., Chen, G., Mirasso, C. R., Maass, W., Arkhipov, A."
date: 2026-04-23
pdf: "https://www.biorxiv.org/content/10.64898/2026.03.13.711751v2.full.pdf"
tags: ["query:slp-ns"]
score: 7.0
evidence: 整合皮层回路的解剖、生理和功能
tldr: 本研究开发了一个可微分模拟器，构建了包含约6.7万个神经元的小鼠初级视觉皮层模型。该模型整合了电镜连接组学、突触生理学及大规模神经记录等多模态数据。通过端到端训练，模型不仅能复现细胞类型特异性的基准表现，还能泛化至自然场景。研究揭示了抑制性连接在网络活动中的核心控制作用，并强调了生物学先验对涌现布线规则的重要性，为研究生物约束下的脑回路功能提供了高效的计算框架。
source: biorxiv
selection_source: fresh_fetch
motivation: 旨在构建一个整合解剖学、生理学和功能活动的多约束皮层回路模型，以探索大脑的运作机制。
method: 利用可微分模拟技术，将电子显微镜连接组学、细胞电生理和神经像素记录数据整合进大规模神经元网络模型中进行端到端训练。
result: 模型在单GPU上仅需6.5小时即可完成训练，展现出强大的泛化能力，并揭示了抑制性连接对网络活动的显著控制作用。
conclusion: 该研究证明了可微分模拟是研究受生物约束的大脑回路功能和机制的一种高效且实用的计算框架。
---

## 摘要
对大脑的机制性理解需要受解剖学、生理学和功能活动约束的模型。我们提出了一个可微分模拟器和一个包含约 67,000 个神经元的小鼠初级视觉皮层模型，该模型整合了多模态数据，包括电子显微镜连接组学、多电极片钳突触生理学、细胞类型解析的内禀电生理学，以及来自多种细胞类型的大规模 Neuropixels 记录。在保留生物学约束的前提下，端到端训练在单个 GPU 上约 6.5 小时内即可完成。仅在简短的漂移光栅响应上训练的网络即可重现细胞类型特异性的基准指标，并能泛化到新的对比度和自然场景。我们揭示了异质的、依赖于细胞类型和调谐特性的突触组织，并表明训练会优先将抑制性连接塑造为不同的群体，从而对网络活动发挥巨大的控制作用。定向消融实验表明，移除突触权重分布的生物学先验虽然可以维持功能活动，但会破坏涌现的布线规则。免费共享的模型和代码使可微分模拟成为一种计算上可行的框架，用于在生物学约束下研究大脑环路的功能和机制。

## Abstract
Mechanistic understanding of the brain requires models constrained by anatomy, physiology, and functional activity. We present a differentiable simulator and a ~67,000-neuron model of mouse primary visual cortex that integrates multimodal data, including electron-microscopy connectomics, multipatch synaptic physiology, cell-type-resolved intrinsic electrophysiology, and large-scale Neuropixels recordings from diverse cell types. End-to-end training completes on a single GPU in ~6.5 hours while preserving biological constraints. Networks trained only on brief drifting-grating responses reproduce cell-type-specific benchmarks and generalize to new contrasts and natural scenes. We uncover heterogeneous cell-type- and tuning-dependent synaptic organization and show that training preferentially sculpts inhibitory connectivity into distinct cohorts that exert outsized control over network activity. Targeted ablations show that removing biological priors on synaptic weight distributions can preserve functional activity yet disrupt emergent wiring rules. The freely shared models and code facilitate differentiable simulations as a computationally practical framework for studying brain circuit function and mechanisms under biological constraints.