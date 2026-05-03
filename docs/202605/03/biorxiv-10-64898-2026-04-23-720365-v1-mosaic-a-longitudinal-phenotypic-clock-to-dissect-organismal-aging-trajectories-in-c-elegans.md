---
title: "MOSAIC: a longitudinal phenotypic clock to dissect organismal aging trajectories in C. elegans"
title_zh: MOSAIC：一种用于剖析秀丽隐杆线虫个体衰老轨迹的纵向表型时钟
authors: "Vaudano, A. P., Pierron, M., Stojkovic, L., Membrez, M., Bourgeois, M., Neal, C., Chimen, M., Verbakel, L., Cornaglia, M., Solari, F., Mouchiroud, L."
date: 2026-04-27
pdf: "https://www.biorxiv.org/content/10.64898/2026.04.23.720365v1.full.pdf"
tags: ["query:qll"]
score: 7.0
evidence: 生物衰老时钟与生物体衰老轨迹
tldr: 针对寿命延长不一定等同于健康期延长的问题，本研究开发了MOSAIC，一种基于秀丽隐杆线虫的非侵入性纵向表型时钟。通过对约3750只线虫进行高频成像并结合机器学习，MOSAIC利用29个表型特征在单体分辨率下精确预测生物年龄。该工具不仅能分解生理模块的贡献，还揭示了不同长寿干预措施通过各异的动态轨迹而非统一的减速来重塑衰老过程，为量化健康衰老提供了新框架。
source: biorxiv
selection_source: fresh_fetch
motivation: 现有的生物衰老时钟多依赖侵入性或单点测量，难以捕捉个体在衰老过程中的动态生理变化和健康轨迹。
method: 结合高频成像技术与机器学习，开发了包含29个表型特征的MOSAIC系统，实现对线虫全生命周期的非侵入性纵向监测。
result: 研究发现长寿干预措施（如饮食限制、基因突变）会产生截然不同的生物年龄轨迹和生理权衡，而非简单的衰老速度均匀减慢。
conclusion: MOSAIC为量化生物年龄提供了可扩展的非侵入性框架，有助于深入理解干预措施如何通过重塑表型轨迹来影响健康寿命。
---

## 摘要
延长寿命的干预措施并不一定能维持健康寿命（即处于良好健康状态的生命阶段）。这种脱节增强了人们对生物衰老时钟作为生物体健康定量指标的兴趣。然而，大多数现有的时钟依赖于侵入性或终点测量，提供的是捕捉单一时间点生物年龄的静态估计，对衰老轨迹（即个体生理韧性和功能能力随时间变化的动态模式）的洞察有限。在本研究中，我们将秀丽隐杆线虫全生命周期的标准化、高频个体成像与机器学习相结合，开发了 MOSAIC（秀丽隐杆线虫模块化生物体衰老特征），这是一种非侵入性表型时钟，能够以单体分辨率纵向估计生物年龄。利用约 3750 只动物、约 230,000 次观察和 29 个表型特征，MOSAIC 能以高准确度预测生物年龄，并以高时间分辨率解析全生物体的衰老轨迹。除了年龄预测，MOSAIC 还将生物年龄分解为来自不同生理模块的贡献，从而实现了对生物体衰退的机制性解释。将 MOSAIC 应用于自然寿命变异、饮食限制、长寿突变体和药物干预研究，结果表明，寿命的延长可能通过不同的、随时间变化的表型轨迹实现，而非统一的衰老减缓。对长寿具有相似效果的干预措施会产生迥异的生物年龄轨迹以及年轻和衰老特征的不同组合，突显了上下文相关的生理权衡。MOSAIC 提供了一个可扩展的、非侵入性的框架，用于在整个生命周期内重复量化生物年龄，并根据干预措施如何重塑衰老轨迹来对其进行比较。

## Abstract
Interventions that extend lifespan do not necessarily preserve healthspan, the portion of life spent in good health. This disconnect has intensified interest in biological aging clocks as quantitative proxies of organismal health. However, most existing clocks rely on invasive or endpoint measurements, providing static estimates that capture biological age at a single time point and offer limited insight into aging trajectories - the dynamic patterns through which physiological resilience and functional capacity change within individuals over time.

Here we combine standardized, high-frequency imaging of individual Caenorhabditis elegans across the lifespan with machine learning to develop MOSAIC (Modular Organismal Signature of Aging In C. elegans), a non-invasive phenotypic clock that estimates biological age longitudinally at single-organism resolution. Leveraging [~]3750 animals, [~]230000 observations and 29 phenotypic features, MOSAIC predicts biological age with high accuracy and resolves organism-wide aging trajectories at high temporal resolution. Beyond age prediction, MOSAIC decomposes biological age into contributions from distinct physiological modules, enabling mechanistic interpretation of organismal decline.

Applying MOSAIC to natural lifespan variation, dietary restriction, longevity mutants and pharmacological interventions reveals that lifespan extension can emerge through distinct, time-dependent phenotypic trajectories rather than a uniform slowing of aging. Interventions with similar effects on longevity produce divergent biological-age trajectories and distinct combinations of younger and older traits, highlighting context-dependent physiological trade-offs. MOSAIC provides a scalable, non-invasive framework to repeatedly quantify biological age across the lifespan and to compare interventions based on how they reshape aging trajectories.