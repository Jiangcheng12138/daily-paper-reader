---
title: "Beyond the Forest and the Trees: Overlooking the Overlooked Terrain of Neural State Dynamics"
title_zh: 超越森林与树木：忽视被忽略的神经状态动力学地形
authors: "Asai, T., Kashihara, S., Chiyohara, S."
date: 2026-06-09
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.04.729738v1.full.pdf"
tags: ["query:slp-ns"]
score: 7.0
evidence: 神经状态动力学脑电微状态分析
tldr: 传统EEG微状态分析依赖从GFP峰值聚类的模板，但模板定义高度敏感，影响可重复性。本文提出拓扑几何视角，将模板重新定义为嵌入全局状态空间中的地标，保留极性关系。实验表明基于地标的定义比传统模板更好地捕获状态结构，提升分析性能。该工作为微状态分析提供更原则且稳定的基础，有助于跨数据集比较。
source: biorxiv
selection_source: fresh_fetch
motivation: 传统EEG微状态模板基于GFP峰值聚类，定义高度敏感，导致可重复性差，难以跨研究比较。
method: 将模板视为全局状态空间中的地标，保留极性几何关系，利用拓扑结构定义状态，而非聚类质心。
result: 基于地标的状态定义优于传统模板，更准确捕获状态结构，提升分析性能。
conclusion: 从模板到地标的转变提供了更稳定、更原则性的状态定义基础，适用于EEG和fMRI，促进跨数据集统一比较。
---

## 摘要
状态转换方法，包括EEG微状态分析和相关的fMRI方法如隐马尔可夫模型（HMM）和共激活模式（CAP）分析，为将神经动力学粗粒度化为少量准稳定状态提供了广泛使用的工具。其效用已在静息态和任务范式中得到验证，应用范围从认知神经科学到精神与神经疾病的候选生物标志物。然而，一个根本性局限依然存在：几乎所有下游时间测量都依赖于最初定义的模板图。在传统流程中，模板源自全局场功率（GFP）峰值处电压图的极性不变聚类，这使得最终的状态定义对预处理、采样、初始化、聚类算法以及聚类数量的选择敏感。因此，该方法捕捉了EEG动力学中的粗粒度规律，而对生成这些状态的更大几何组织约束较弱。这种模板依赖性对跨研究和EEG帽的可重复性及比较构成了重大挑战。这里，我们从拓扑几何角度重新审视这一问题。我们不将模板视为从GFP峰值图中提取的聚类质心，而是将其视为嵌入在由头皮电压图之间相互相似性构建的状态空间全局结构中的地标。在此表述中，微状态模板被重新发现为组织连续神经状态地形学的主轴离散代表。这种重构保留了极性作为一种有意义的几何关系，而不是一开始就将其作为分析冗余消除。它还将注意力从孤立的状态标签转移到状态空间本身的地形：即局部状态变得可解释的更广泛关系结构。通过这种方法，我们展示了基于地标的状态定义在捕捉状态结构和提高分析性能方面优于传统模板。这些发现表明，EEG微状态分析的核心问题比聚类优化更广泛：它涉及如何定义有效的节点以粗粒度化连续动力学，而不丢弃组织它们的拓扑结构。通过将微状态分析的概念基础从模板转向地标，本方法为状态定义提供了更原理化且可能更稳定的基础，包括在fMRI中。这种拓扑几何重评估扩展了传统微状态分析，并为跨数据集、范式和记录系统的更统一比较开辟了路径。

## Abstract
State-transition approaches, including EEG microstate analysis and related fMRI methods such as hidden Markov models (HMMs) and co-activation pattern (CAP) analysis, provide widely used tools for coarse-graining neural dynamics into a small set of quasi-stable states. Its utility has been demonstrated across resting-state and task paradigms, with broad applications ranging from cognitive neuroscience to candidate biomarkers for psychiatric and neurological disorders. A fundamental limitation remains, however: nearly all downstream temporal measures are conditional on the template maps defined at the outset. In the conventional pipeline, templates are derived from polarity-invariant clustering of voltage maps at global field power (GFP) peaks, making the resulting state definitions sensitive to preprocessing, sampling, initialization, clustering algorithms, and the choice of cluster number. Consequently, the method captures coarse regularities in EEG dynamics, while only weakly constraining the larger geometric organization from which those states emerge. This template dependence poses a major challenge for reproducibility and for comparisons across studies and EEG caps. Here, we revisit this problem from a topological-geometric perspective. We treat templates not as cluster centroids extracted from GFP-peak maps, but as landmarks embedded in the global structure of a state space constructed from mutual similarities among scalp voltage maps. In this formulation, microstate templates are rediscovered as discrete representatives of dominant axes that organize continuous neural-state topography. This reformulation preserves polarity as a meaningful geometric relation instead of eliminating it at the outset as analytical redundancy. It also shifts attention from isolated state labels to the terrain of the state space itself: the broader relational structure within which local states become interpretable. Using this approach, we show that landmark-based state definitions outperform conventional templates in capturing state structure and improving analytical performance. These findings suggest that the central problem in EEG microstate analysis is broader than clustering optimization: it concerns how to define valid nodes for coarse-graining continuous dynamics without discarding the topology that organizes them. By shifting the conceptual basis of microstate analysis from templates to landmarks, the present approach provides a more principled and potentially more stable foundation for state definition, including in fMRI. This topolo-geometric reappraisal extends conventional microstate analysis and opens a path toward more unified comparisons across datasets, paradigms, and recording systems.