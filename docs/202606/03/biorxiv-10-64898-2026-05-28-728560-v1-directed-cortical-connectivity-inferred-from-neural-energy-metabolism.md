---
title: Directed cortical connectivity inferred from neural energy metabolism
title_zh: 从神经能量代谢推断的有向皮层连接
authors: "Belenya, R., Epp, S., Bose, A., Hechler, A., Fraticelli, L., Ashrafi, M., Ranft, A., Yakushev, I., Kurcyus, K., Castrillon, G., Riedl, V."
date: 2026-05-29
pdf: "https://www.biorxiv.org/content/10.64898/2026.05.28.728560v1.full.pdf"
tags: ["query:slp-ns"]
score: 7.0
evidence: 利用能量代谢推断有向连接，与睡眠-觉醒调控相关
tldr: "功能连接无法揭示神经信号方向，而有效连接对理解皮层层次和能量约束至关重要。本文扩展代谢连接映射(MCM)，基于突触前后神经元能量消耗差异，从[18F]FDG PET测量的区域能量比直接推断有向连接。新全皮层实现可应用于多模态及仅有fMRI的数据，成功再现视觉和感觉运动系统的层次化信号传递，并发现感知-认知梯度的方向不对称性。MCM指标与线粒体密度和皮层细胞构筑独立相关，为统计连接与神经能量机制之间搭建了可解释的桥梁。"
source: biorxiv
selection_source: fresh_fetch
motivation: 确定有效连接对于理解皮层层次结构和能量约束至关重要，但现有功能连接无法提供方向信息。
method: 基于突触前后神经元能量消耗差异，利用代谢连接映射从区域间葡萄糖代谢率比直接估计有向连接。
result: MCM模型成功再现视觉和感觉运动系统的层次化信号，并发现感知-认知梯度的方向不对称性，指标与线粒体密度和细胞结构相关。
conclusion: MCM是连接统计功能连接与神经能量机制的可扩展、生物可解释模型，可应用于多模态神经影像数据。
---

## 摘要
静息态功能磁共振成像（fMRI）的功能连接（FC）捕捉大脑区域间的时间相关性，但无法揭示神经信号传导的方向。确定有效连接（即一个神经系统对另一个神经系统的影响）对于理解皮层层级结构及其能量限制至关重要。我们扩展了代谢连接映射（MCM；Riedl 等，2016）——一个基于生物学原理的框架，通过整合FC与[18F]氟代脱氧葡萄糖正电子发射断层扫描（[18F]FDG PET）测量的葡萄糖代谢来推断方向性。MCM基于如下原则：突触后神经元比突触前神经元消耗更多能量（Attwell 和 Laughlin，2001；Attwell 和 Gibb，2005），从而将较高的局部代谢与传入输入联系起来。在此，我们提出一种新的全皮层实现方法，直接根据区域间能量比率估计有向连接，从而能够通过平均脑葡萄糖代谢率（CMRGlc）图应用于多模态和仅fMRI数据集。该模型再现了视觉和感觉运动系统内的层级信号传导，并识别出沿感觉-认知梯度的新型方向不对称性。MCM导出的指标与独立的生物学标志物相关，包括线粒体密度（Mosharov 等，2025）和由细胞层轮廓索引的皮层细胞结构（Amunts 和 Zilles，2015；Wagstyl 等，2020）。通过将功能连接分解为受代谢约束的有向和无向成分，该框架弥合了统计连接与神经能量机制之间的差距。我们的结果将MCM定位为一种可扩展且生物学可解释的模型，用于从人类神经影像数据推断有向脑连接。

## Abstract
Functional connectivity (FC) from resting-state fMRI captures temporal correlations between brain regions but cannot reveal the direction of neural signalling. Determining effective connectivity, the influence of one neural system over another, is essential for understanding cortical hierarchy and its energetic constraints. We extend Metabolic Connectivity Mapping (MCM; Riedl et al., 2016), a biologically grounded framework that infers directionality by integrating FC with glucose metabolism measured via [18F]fluorodeoxyglucose positron emission tomography ([18F]FDG PET). MCM builds on the principle that postsynaptic neurons consume more energy than presynaptic ones (Attwell and Laughlin, 2001; Attwell and Gibb, 2005), linking higher local metabolism to afferent input. Here, we present a new whole-cortex implementation that estimates directed connectivity directly from inter-regional energy ratios, enabling application to multimodal and fMRI-only datasets using an average cerebral metabolic rate of glucose (CMRGlc) map. The model reproduces hierarchical signalling within visual and sensorimotor systems and identifies novel directional asymmetries along sensory-cognitive gradients. MCM-derived metrics correlate with independent biological markers, including mitochondrial density (Mosharov et al., 2025) and cortical cytoarchitecture indexed by cell layer profiles (Amunts and Zilles, 2015; Wagstyl et al., 2020). By decomposing functional connectivity into metabolically constrained directed and undirected components, this framework bridges the gap between statistical connectivity and neuroenergetic mechanisms. Our results position MCM as a scalable and biologically interpretable model for inferring directed brain connectivity from human neuroimaging data.