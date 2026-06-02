---
title: An LLM-driven pipeline for proteomics-based detection and structural modeling of post-translational modifications
title_zh: 基于LLM的蛋白质组学翻译后修饰检测与结构建模流程
authors: "George, A., Mejia-Rodriguez, D., Li, X., Rigor, P., Cheung, M. S., Bilbao, A."
date: 2026-05-06
pdf: "https://www.biorxiv.org/content/10.64898/2026.05.01.722279v1.full.pdf"
tags: ["query:qll"]
score: 7.0
evidence: 提供LLM驱动的翻译后修饰检测与结构建模流程，可用于衰老相关PTM研究
tldr: 翻译后修饰(PTM)动态调控蛋白质功能，但基于质谱的检测和结构建模之间缺乏集成管道。本文提出生成式AI管道，包含PTMdiscoverer（利用LLM从开放搜索质谱数据中鉴定注释PTM）和PTM-Psi（建模PTM对蛋白质动力学和相互作用的影响）。在蓝细菌蛋白质组学数据上验证，用于研究氧化还原调控的“暗复合体”形成机制。贡献在于将PTM发现与结构层面的机械解释联系起来。
source: biorxiv
selection_source: fresh_fetch
motivation: 现有PTM检测和结构建模工具分离，难以解释PTM的生物学意义。
method: 提出集成管道：PTMdiscoverer用LLM从开放搜索质谱结果中鉴定PTM，PTM-Psi建模结构动态后果。
result: 在蓝细菌数据上成功演示，揭示了氧化还原调控的“暗复合体”形成的潜在分子机制。
conclusion: 该管道桥梁了PTM发现与结构解释，推进了对微生物系统中PTM介导调控的理解。
---

## 摘要
蛋白质上的翻译后修饰（PTMs）动态调控其功能，进而影响细胞生理。尽管在PTM检测和建模方面取得了显著进展：基于质谱的蛋白质组学已成为复杂样本中PTM检测的基石，而新兴的结构预测框架能够对PTM依赖的构象变化进行建模。然而，许多PTM的生物学意义在很大程度上仍未得到探索，部分原因在于连接PTM检测与结构建模的集成流程仍然有限。我们提出了一种基于生成式AI的流程，将PTM检测与其对蛋白质动力学和相互作用影响的结构建模相结合。该流程包含两个互补工具：PTMdiscoverer和PTM-Psi。首先，PTMdiscoverer利用大语言模型从开放搜索蛋白质组学结果中识别、注释和解读候选PTM，解决了传统蛋白质组学工具的局限性。接着，PTM-Psi对这些空间感知修饰在蛋白质动力学上的结构、功能和动态后果进行建模。这两个组件将PTM发现与结构层面的机制解释连接起来。我们通过使用蓝藻蛋白质组学数据来研究碳代谢中氧化还原调控的“暗复合物”形成的潜在分子机制，展示了我们的流程，从而提升了我们解读微生物系统中PTM介导调控的能力。

## Abstract
Post-translational modifications (PTMs) on proteins dynamically regulate their functions and subsequently cellular physiology. Significant advances have been made in their detection and modeling: mass spectrometry-based proteomics has become the cornerstone for PTM detection in complex samples, while emerging structure-prediction frameworks enable modeling of PTM-dependent conformational changes. However, the biological significance of many PTMs remains largely unexplored, in part because integrated pipelines that bridge PTM detection with structural modeling remain limited. We present a generative AI-driven pipeline that integrates PTM detection with structural modeling of their effects on protein dynamics and interactions. The pipeline comprises two complementary tools: PTMdiscoverer and PTM-Psi. First, PTMdiscoverer leverages large language models to identify, annotate, and interpret candidate PTMs from open-search proteomics results, addressing limitations of conventional proteomics tools. Next, PTM-Psi models the structural, functional, and dynamic consequences of these spatially aware modifications on protein dynamics. These two components bridge PTM discovery with mechanistic interpretation at the structural level. We demonstrate our pipeline by using cyanobacterial proteomics data to study potential molecular mechanisms of redox-regulated "dark complex" formation in carbon metabolism, advancing our ability to interpret PTM-mediated regulation in microbial systems.