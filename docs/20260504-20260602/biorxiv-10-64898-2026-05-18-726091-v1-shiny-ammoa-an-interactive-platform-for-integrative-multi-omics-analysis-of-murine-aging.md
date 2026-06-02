---
title: "Shiny AMMOA: an interactive platform for integrative multi-omics analysis of murine aging"
title_zh: Shiny AMMOA：用于小鼠衰老整合多组学分析的交互式平台
authors: "Ninomiya Kanda, M."
date: 2026-05-20
pdf: "https://www.biorxiv.org/content/10.64898/2026.05.18.726091v1.full.pdf"
tags: ["query:qll"]
score: 7.0
evidence: 用于衰老的多组学平台，可应用于卵巢翻译后修饰研究
tldr: 衰老伴随多组学复杂变化，但整合分析存在计算门槛。Shiny AMMOA基于R Shiny框架，提供图形界面集成小鼠转录组、蛋白组和代谢组公开数据，支持差异表达、通路富集及跨组学可视化。平台成功复现衰老相关通路（如未折叠蛋白反应、细胞外基质）并揭示组织特异性特征。通过降低技术壁垒，使实验生物学家能交互探索大规模数据，加速系统级假说生成和转化。
source: biorxiv
selection_source: fresh_fetch
motivation: 降低多组学数据整合分析的技术门槛，让实验研究人员能交互探索衰老分子变化。
method: 构建R Shiny图形界面，集成小鼠转录组、蛋白组和代谢组数据，提供差异表达、通路富集和跨组学可视化。
result: 复现关键衰老通路（未折叠蛋白反应、细胞外基质等），并识别组织与组学层特异性特征。
conclusion: 为实验生物学家提供易用、严谨的多组学分析资源，助力衰老研究假说生成与验证。
---

## 摘要
衰老伴随跨多个生物层的复杂、组织特异性分子变化，然而由于技术和计算障碍，整合分析多组学数据集对许多实验研究人员仍具挑战。在此，我提出Shiny Aging Murine Multi-Omic Analyzer（Shiny AMMOA），一个基于图形用户界面（GUI）、用户友好的分析平台，可交互式探索小鼠衰老相关的批量转录组、蛋白质组和代谢组数据集。Shiny AMMOA在统一的R Shiny框架内整合了公开可用的多组学资源，并支持端到端分析，包括差异表达检验、通路富集分析以及跨单个和多个组学层的通路级可视化。

通过代表性用例，我证明Shiny AMMOA重现了原始研究的关键发现，并有助于直观发现组织、通路和模态特异性的衰老特征，包括特定组织和组学层中未折叠蛋白反应、细胞外基质组织和代谢通路等的年龄相关变化。该平台进一步支持在京都基因与基因组百科全书（KEGG）通路图上跨组学层可视化分子变化，从而在系统层面促进假设生成。

通过降低整合多组学分析的访问门槛同时保持分析严谨性，Shiny AMMOA为实验生物学家和衰老研究人员提供了一个可扩展的资源，用于查询大规模公共数据集、优先考虑生物通路，并加速将多组学见解转化为可检验的实验假设。Shiny AMMOA可通过https://github.com/M-Ninomiya-Kanda/Shiny_AMMOA_local获取，一个功能有限的轻量级网络演示版本可通过https://m-ninomiya-kanda.shinyapps.io/shiny_ammoa_web/访问。

## Abstract
Aging is accompanied by complex, tissue-specific molecular changes across multiple biological layers, yet integrative analysis of multi-omics datasets remains challenging for many experimental researchers due to technical and computational barriers. Here, I present Shiny Aging Murine Multi-Omic Analyzer (Shiny AMMOA), a graphical user interface (GUI)-based, user-friendly analytical platform that enables interactive exploration of murine aging-associated bulk transcriptomic, proteomic, and metabolomic datasets. Shiny AMMOA integrates publicly available multi-omics resources within a unified R Shiny framework and supports end-to-end analyses, including differential expression testing, pathway enrichment analysis, and pathway-level visualization across individual and multiple omics layers.

Using representative use cases, I demonstrate that Shiny AMMOA recapitulates key findings from original source studies and facilitates intuitive discovery of tissue-, pathway-, and modality-specific aging signatures, including age-associated alterations in unfolded protein response, extracellular matrix organization, and metabolic pathways across specific tissues and omics layers. The platform further enables integrated visualization of molecular changes across omics layers on Kyoto Encyclopedia of Genes and Genomes (KEGG) pathway diagrams, supporting hypothesis generation at the systems level.

By democratizing access to integrative multi-omics analysis while preserving analytical rigor, Shiny AMMOA provides an extensible resource for experimental biologists and aging researchers to interrogate large-scale public datasets, prioritize biological pathways, and accelerate translation of multi-omics insights into testable experimental hypotheses. Shiny AMMOA is available at https://github.com/M-Ninomiya-Kanda/Shiny_AMMOA_local, and a lightweight web-based demonstration version with limited functionality is available at https://m-ninomiya-kanda.shinyapps.io/shiny_ammoa_web/.