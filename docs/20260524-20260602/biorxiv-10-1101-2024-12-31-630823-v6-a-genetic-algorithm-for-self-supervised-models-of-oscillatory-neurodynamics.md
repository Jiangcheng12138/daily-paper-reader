---
title: A genetic algorithm for self-supervised models of oscillatory neurodynamics
title_zh: 用于振荡神经动力学自监督模型的遗传算法
authors: "Nejat, H., Sherfey, J., Bastos, A. M."
date: 2026-05-29
pdf: "https://www.biorxiv.org/content/10.1101/2024.12.31.630823v6.full.pdf"
tags: ["query:slp-ns"]
score: 8.0
evidence: 用于振荡神经动力学的遗传算法，与睡眠节律相关
tldr: 预测处理理论认为大脑通过减少预测与感觉信号的差异构建内部模型，这与伽马和α/β振荡相关。现有抽象模型虽能实现自监督计算但缺乏振荡尖峰动力学，而生物物理约束模型需大量手动调参。本文提出遗传随机增量规则（GSDR）进化优化框架，可拟合非线性神经模型到电生理目标，如放电率、β/γ谱比和猕猴视觉皮层刺激诱发伽马振荡。GSDR能搜索约束参数空间、减少手动调参，并重现预测路由相关表型，且不限于Hodgkin-Huxley模型，为自动多目标探索振荡神经模型提供了通用方法。
source: biorxiv
selection_source: fresh_fetch
motivation: 现有模型要么缺乏振荡尖峰动力学，要么需要大量手动调参，难以兼顾生物合理性与可训练性。
method: 提出遗传随机增量规则（GSDR），结合目标引导搜索、随机探索、遗传选择与活动依赖更新，进化优化非线性神经模型。
result: GSDR能调谐尖峰网络达到β/γ谱目标，并重现猕猴视觉皮层刺激诱发伽马振荡的动态特征。
conclusion: GSDR可作为自动多目标探索振荡神经模型的通用框架，减少手动调参并支持多种神经元模型。
---

## 摘要
预测处理理论认为，大脑通过减少内部生成的预测与外部感觉信号之间的差异来建立其环境内部模型。以往的研究将这些过程与伽马（40-100赫兹）和α/β（10-30赫兹）频段的振荡活动联系起来。当前的计算方法面临一个权衡：抽象的预测处理模型可以实现自监督计算，但通常省略振荡尖峰动力学，而生物物理约束的尖峰模型可以生成神经节律，但通常需要大量手动调整。在此，我们引入了遗传随机增量规则（GSDR），这是一种进化优化框架，用于将非线性神经模型拟合到电生理目标。我们首先在简化优化设置中评估GSDR，然后将其应用于涉及放电率、β/γ频谱比率以及来自视觉皮层的经验性猕猴刺激诱发伽马动力学的尖峰网络目标。我们表明，GSDR可以搜索约束的突触参数空间，减少对手动调整的依赖，并再现与预测路由相关的频谱和回路水平表型。我们还使用Izhikevich模拟作为模型类别鲁棒性分析，表明该方法不限于原始的Hodgkin-Huxley风格实现。这些结果将GSDR定位为一种用于自动、多目标探索振荡神经模型的方法框架，其中预测路由作为一个激励案例研究，而非作为完成的功能证明。

作者总结：在预测处理理论中，假设大脑建立其环境的内部模型。经验和理论研究暗示神经元振荡是这一过程的重要组分，异常振荡也与精神分裂症等疾病相关。为了研究这类机制，计算神经科学需要能够表达生物上有意义的尖峰和振荡动力学，同时可以在无需大量手动调整的情况下进行训练的模型。我们开发了遗传随机增量规则（GSDR），这是一种自监督的进化优化框架，用于将非线性神经模型拟合到目标。GSDR结合了目标引导搜索、随机探索、遗传选择/去选择以及活动依赖的MCDP更新项。我们展示了GSDR可以将尖峰网络调整至β/γ频谱目标和经验性刺激诱发的伽马动力学。结果并未证明预测路由或确定唯一的生物回路；相反，它们表明GSDR可以识别候选回路配置，并能够从原始的Hodgkin-Huxley风格模型泛化到Izhikevich模拟。

## Abstract
Predictive processing theories propose that the brain builds internal models of its environment by reducing the discrepancy between internally generated predictions and external sensory signals. Prior work has linked these processes to oscillatory activity in gamma (40-100 Hz) and alpha/beta (10-30 Hz) frequency ranges. Current computational approaches face a trade-off: abstract predictive-processing models can implement self-supervised computations but often omit oscillatory spiking dynamics, whereas biophysically constrained spiking models can generate neural rhythms but often require extensive manual tuning. Here, we introduce the Genetic Stochastic Delta Rule (GSDR), an evolutionary optimization framework for fitting nonlinear neural models to electrophysiological objectives. We first evaluate GSDR in simplified optimization settings, then apply it to spiking-network objectives involving firing rates, beta/gamma spectral ratios, and empirical macaque stimulus-evoked gamma dynamics from visual cortex. We show that GSDR can search constrained synaptic parameter spaces, reduce reliance on manual tuning, and reproduce spectral and circuit-level phenotypes associated with predictive routing. We also used Izhikevich simulations as a model-class robustness analysis, showing that the approach is not limited to the original Hodgkin-Huxley-style implementation. These results position GSDR as a methodological framework for automated, multi-objective exploration of oscillatory neural models, with predictive routing serving as a motivating case study rather than as a completed functional proof.

Author summaryIn predictive processing theories, the brain is hypothesized to build internal models of its environment. Empirical and theoretical studies suggest that neuronal oscillations are important components of this process, and abnormal oscillations are also linked to disorders such as schizophrenia. To study such mechanisms, computational neuroscience needs models that can express biologically meaningful spiking and oscillatory dynamics while also being trainable without extensive manual tuning. We developed the Genetic Stochastic Delta Rule (GSDR), a self-supervised evolutionary optimization framework for fitting nonlinear neural models to objectives. GSDR combines objective-guided search, stochastic exploration, genetic selection/deselection, and an activity-dependent MCDP update term. We show that GSDR can tune spiking networks toward beta/gamma spectral objectives and empirical stimulus-evoked gamma dynamics. The results do not prove predictive routing or identify a unique biological circuit; rather, they show that GSDR can identify candidate circuit configurations and can generalize beyond the original Hodgkin-Huxley-style model to Izhikevich simulations.