---
title: "Neural Population Models for EEG: From Canonical Models to Alternative Model Structures"
title_zh: 脑电图神经群体模型：从经典模型到替代模型结构
authors: "Omejc, N., Roman, S., Todorovski, L., Dzeroski, S."
date: 2026-04-14
pdf: "https://www.biorxiv.org/content/10.64898/2026.04.10.717643v1.full.pdf"
tags: ["query:slp-ns"]
score: 7.0
evidence: 用于解释脑电图数据的神经群体模型
tldr: 本研究系统探讨了脑电图（EEG）神经群体模型的结构多样性。通过对比17种经典模型并利用新开发的ENEEGMA框架进行基于语法的模型自动生成，研究者在静息态和稳态视觉诱发电位数据上评估了各模型表现。结果发现，低维振荡器模型在拟合效果与简洁性间达到了最佳平衡，且新生成的模型展现出极强的竞争力。该研究揭示了EEG数据对神经机制的约束性而非唯一性，为模型发现提供了新路径。
source: biorxiv
selection_source: fresh_fetch
motivation: 旨在理清经典神经群体模型间的关系，并探究EEG数据是否能唯一确定特定的群体水平产生机制。
method: 整合17种经典模型并开发ENEEGMA框架，利用概率语法生成候选模型，并将其拟合至多套EEG独立成分频谱数据进行对比。
result: 低维多项式振荡器（如MPR、FHN和SL模型）表现最优，且自动生成的模型在SSVEP拟合中达到了最强的集群水平表现。
conclusion: EEG频谱虽能限制合理的神经群体机制，但不足以唯一确定单一模型，基于语法的自动化探索是发现神经模型的重要手段。
---

## 摘要
神经群体模型被广泛用于解释脑电图（EEG），但与单神经元模型相比，它们之间的关系在系统性理解上仍显不足。更根本的是，目前尚不清楚 EEG 是否能支持一种唯一合理的群体级机制，或者是否多种结构迥异的模型能同样出色地解释数据。为解决这一问题，我们将经典模型家族的比较分析与基于语法的候选架构生成相结合。我们汇集了 17 种经典的神经质量模型和现象学模型，并将它们嵌入到一个共享的结构空间中。基于它们的共同过程，我们定义了一套关于可解释动力学组件的概率语法，并开发了 ENEEGMA（探索神经 EEG 模型架构），这是一个基于 Julia 的框架，用于基于语法的模型生成、模拟和参数优化，以生成额外的候选模型。随后，我们通过将经典模型和生成的模型拟合到两种实验条件下（静息态和稳态视觉诱发电位）的四个数据集的 EEG 独立成分谱中，对它们进行了评估。经典模型形成了六个结构簇。在不同条件下，紧凑的低维多项式振荡器总体表现最佳，其中 Montbrio-Pazo-Roxin、FitzHugh-Nagumo 和 Stuart-Landau 模型在拟合质量、稳定性和简洁性之间提供了最佳平衡。基于语法的探索进一步表明，可行的 EEG 节点模型空间超出了经典公式的范畴：即使是在 1,000 个生成的模型中进行受限搜索，也产生了能与几乎所有经典家族竞争的紧凑替代方案，并实现了最强的簇级 SSVEP 拟合。总之，这些发现表明 EEG 谱约束了合理的神经群体机制，但并未唯一地确定它们。此外，基于语法的模型探索为受 EEG 约束的模型发现提供了一个有原则的、数据驱动的框架。

作者总结：脑电图（EEG）使我们能够以非侵入性的方式测量大脑活动，但由于信号是间接的，我们依赖数学模型来解释神经群体是如何产生这些信号的。尽管存在许多此类模型，但尚不清楚标准模型是否涵盖了 EEG 数据所有合理的解释范围，或者几种截然不同的模型是否能同样好地解释同一信号。在本研究中，我们比较了一系列广泛的既定神经群体模型，然后使用基于语法的方程发现框架，从可解释的构建模块中自动生成新的候选模型。我们发现，简单的低维振荡器模型通常比更复杂的经典模型能更好地匹配 EEG 谱。我们还发现，新生成的模型表现几乎与既定模型一样好，有时甚至更好，特别是在刺激驱动的反应方面。这些结果表明，仅凭 EEG 谱可能不足以识别唯一的底层神经机制。更广泛地说，我们的工作展示了自动化的、具有生物学启发意义的模型生成如何帮助比较、理解、扩展和测试候选神经群体模型的空间。

## Abstract
Neural population models are widely used to interpret electroencephalography (EEG), yet their relationships remain far less systematically understood than those among single-neuron models. More fundamentally, it remains unclear whether EEG can support a uniquely plausible population-level mechanism, or whether multiple structurally distinct models can explain the data equally well. To address this question, we combine comparative analysis of canonical model families with grammar-based generation of new candidate architectures. We assembled 17 canonical neural mass and phenomenological models and embedded them in a shared structural space. From their common processes, we defined a probabilistic grammar over interpretable dynamical components and developed ENEEGMA (Exploring Neural EEG Model Architectures), a Julia-based framework for grammar-based model generation, simulation, and parameter optimization, to generate additional candidate models. We then assessed both canonical and generated models by fitting them to EEG independent-component spectra from four datasets for each condition: resting state and steady-state visual evoked potentials. Canonical models formed six structural clusters. Across conditions, compact low-dimensional polynomial oscillators performed best overall, with Montbrio-Pazo-Roxin, FitzHugh-Nagumo, and Stuart-Landau models offering the best balance of fit quality, stability, and simplicity. Grammar-based exploration further showed that the space of viable EEG node models extends beyond canonical formulations: even a restricted search over 1,000 generated models produced compact alternatives competitive with nearly all canonical families and achieving the strongest cluster-level SSVEP fits. Together, these findings suggest that EEG spectra constrain plausible neural population mechanisms without uniquely determining them. Beyond this, grammar-based model exploration provides a principled, data-driven framework for EEG-constrained model discovery.

Author summaryElectroencephalography (EEG) lets us measure brain activity non-invasively, but the signals are indirect, so we rely on mathematical models to explain how neural populations generate them. Many such models exist, yet it is unclear whether standard models cover the full range of plausible explanations for EEG data, or whether several very different models can explain the same signal equally well. In this study, we compared a broad set of established neural population models and then used a grammar-based equation discovery framework to automatically generate new candidate models from interpretable building blocks. We found that simple low-dimensional oscillator models often matched EEG spectra better than more complex canonical models. We also found that newly generated models could perform nearly as well as, and sometimes better than, established ones, especially for stimulus-driven responses. These results suggest that EEG spectra alone may not be enough to identify a unique underlying neural mechanism. More broadly, our work shows how automated, biologically informed model generation can help to compare, understand, expand, and test the space of candidate neural population models.