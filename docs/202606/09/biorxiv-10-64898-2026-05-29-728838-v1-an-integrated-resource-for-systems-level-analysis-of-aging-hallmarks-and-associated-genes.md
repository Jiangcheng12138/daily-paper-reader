---
title: An integrated resource for systems-level analysis of aging hallmarks and associated genes
title_zh: 用于衰老标志和相关基因系统级分析的综合资源
authors: "Tiwari, R., Balaji, M., Chivukula, N., Sil, P., Samal, A."
date: 2026-06-02
pdf: "https://www.biorxiv.org/content/10.64898/2026.05.29.728838v1.full.pdf"
tags: ["query:qll"]
score: 6.0
evidence: 衰老标志系统级资源，与卵巢衰老研究相关
tldr: 衰老涉及细胞功能障碍和组织衰退，其标志性特征为系统理解提供了框架。本研究构建AgingHallmarksDB平台，从7个资源中筛选出3111个衰老相关基因，通过功能注释将其映射到11个衰老标志，其中2593个有实验证据支持，1089个为共识基因。平台整合组织特异性、外泌体、调控互作等信息，支持标志富集分析与网络邻近分析。应用于11种慢性老年病和PM2.5相关皮肤转录组，揭示了衰老标志与疾病机制、环境衰老信号的关联。该资源有助于推动以衰老标志为中心的长寿研究。
source: biorxiv
selection_source: fresh_fetch
motivation: 现有资源缺乏系统性分析衰老标志相关基因集的能力，需要整合平台以支持老年病机制研究与干预发现。
method: 从7个衰老资源中筛选基因，取至少2个资源共有的共识集；通过GO、KEGG、Reactome功能注释将3111个基因映射到11个衰老标志，并补充组织特异性、外泌体及调控互作数据，构建交互式分析平台。
result: 获得3111个基因映射到11个衰老标志，其中2593个有实验或人工证据，1089个为共识基因；平台支持标志富集分析和网络邻近分析，并成功应用于11种慢性疾病和PM2.5皮肤转录组。
conclusion: AgingHallmarksDB提供了以衰老标志为中心的系统分析资源，有助于揭示衰老相关疾病机制和环境因素的影响，支持长寿研究。
---

## 摘要
衰老是一个复杂的生物过程，涉及渐进性的细胞功能障碍、组织衰退以及对多种慢性疾病的易感性增加。通过已建立的衰老标志对衰老进行系统性观察，为理解这种复杂性并推动治疗发现提供了结构化框架。为此，我们提出了AgingHallmarksDB，一个交互式网络平台，能够对标志相关基因集进行系统级分析。首先从七个已知资源中整理了衰老相关基因，并将至少在两个资源中出现的基因视为共识衰老相关基因。利用GO、KEGG和Reactome的功能注释，共将3111个基因映射到11个衰老标志，其中2593个有额外的实验或人工整理证据支持，其中1089个组成共识集。此外，AgingHallmarksDB通过组织或细胞类型类别特异性、外泌体谱和调控相互作用补充了基因注释。该平台允许用户交互地对多个条件相关基因集进行系统级标志富集分析，同时无缝整合功能注释和复杂的调控相互作用，以阐明机制性标志-基因关联。通过对应11种慢性年龄相关疾病和PM2.5相关皮肤转录组的基因集的标志富集和网络邻近分析，探讨了衰老标志与疾病机制或环境衰老相关特征之间的关系，从而验证了该资源的实用性。总体而言，AgingHallmarksDB将通过支持以衰老标志为中心的分析来促进长寿研究，该资源可通过https://cb.imsc.res.in/aginghallmarksdb/访问。

## Abstract
Aging is a complex biological process involving progressive cellular dysfunction, tissue decline, and increased susceptibility to multiple chronic diseases. A systemic view of aging through its established hallmarks provides a structured framework to understand this complexity and drive therapeutic discovery. Towards this, we present AgingHallmarksDB, an interactive web platform that enables systems-level analysis of hallmark-associated gene sets. Aging-related genes were first curated from seven established resources, and those present in at least 2 of these resources were considered as consensus aging-related genes. Using functional annotations derived from GO, KEGG, and Reactome, a total of 3111 genes were mapped to the 11 aging hallmarks, of which 2593 were supported by additional experimental or manually curated evidence, with 1089 of these forming the consensus set. Further, AgingHallmarksDB supplements gene annotations with tissue or cell type class specificity, exosomal profiles, and regulatory interactions. The platform allows users to interactively perform systems-level hallmark enrichment analysis across multiple condition-associated gene sets, while seamlessly integrating functional annotations and complex regulatory interactions to elucidate mechanistic hallmark-gene associations. The utility of the resource was explored through hallmark enrichment and network proximity analysis of gene sets corresponding to 11 chronic age-related diseases and PM2.5-associated skin transcriptome to explore relationships between aging hallmarks and disease mechanisms or environmental aging-related signatures. Overall, AgingHallmarksDB will support longevity research by enabling aging hallmark centered analysis, and the resource is accessible at https://cb.imsc.res.in/aginghallmarksdb/.