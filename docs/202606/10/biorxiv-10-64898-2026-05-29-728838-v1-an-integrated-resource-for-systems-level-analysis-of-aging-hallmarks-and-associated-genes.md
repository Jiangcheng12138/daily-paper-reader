---
title: An integrated resource for systems-level analysis of aging hallmarks and associated genes
title_zh: 用于衰老标志及相关基因系统级分析的综合资源
authors: "Tiwari, R., Balaji, M., Chivukula, N., Sil, P., Samal, A."
date: 2026-06-02
pdf: "https://www.biorxiv.org/content/10.64898/2026.05.29.728838v1.full.pdf"
tags: ["query:qll"]
score: 6.0
evidence: 衰老标志综合分析资源
tldr: 衰老是一个复杂的生物学过程，涉及多种标志性特征。为了系统分析衰老相关基因与这些标志的关联，研究者构建了AgingHallmarksDB平台。该平台从7个资源中筛选出3111个基因，映射到11个衰老标志，其中2593个有实验支持，1089个为共识基因。平台整合了组织特异性、外泌体和调控网络信息，支持富集分析和网络邻近分析，应用于11种慢性年龄相关疾病和PM2.5致皮肤衰老的机制探索，为长寿研究提供了重要资源。
source: biorxiv
selection_source: fresh_fetch
motivation: 提供系统级分析衰老标志和相关基因的平台，以理解衰老复杂性并推动治疗发现。
method: 从7个资源中筛选衰老相关基因，取至少两个资源共有的作为共识基因，并通过功能注释映射到11个衰老标志，补充组织特异性和调控信息。
result: 共3111个基因映射到衰老标志，2593个有实验证据，1089个为共识基因；平台支持富集分析并验证了与慢性疾病和环境因素的关联。
conclusion: AgingHallmarksDB为衰老研究提供了标志性基因集分析工具，有助于揭示疾病机制和环境影响。
---

## 摘要
衰老是一个复杂的生物过程，涉及进行性的细胞功能障碍、组织衰退以及对多种慢性疾病的易感性增加。通过已建立的衰老标志对衰老进行系统性审视，为理解这一复杂性并推动治疗发现提供了结构化框架。为此，我们推出了AgingHallmarksDB，一个交互式网络平台，能够对标志相关基因集进行系统级分析。首先从七个已建立的资源中整理了衰老相关基因，并将出现在至少两个资源中的基因视为共识衰老相关基因。利用来自GO、KEGG和Reactome的功能注释，总共将3111个基因映射到11个衰老标志，其中2593个基因有额外的实验或人工整理证据支持，其中1089个构成了共识集。此外，AgingHallmarksDB补充了基因的组织或细胞类型特异性、外泌体谱和调控相互作用注释。该平台允许用户交互地对多个状况相关基因集进行系统级标志富集分析，同时无缝整合功能注释和复杂的调控相互作用，以阐明机制性的标志-基因关联。通过对11种慢性年龄相关疾病和PM2.5相关皮肤转录组的基因集进行标志富集和网络邻近分析，探索了衰老标志与疾病机制或环境衰老相关特征之间的关系，从而验证了该资源的实用性。总之，AgingHallmarksDB通过支持以衰老标志为中心的分析，将促进长寿研究，该资源可通过https://cb.imsc.res.in/aginghallmarksdb/访问。

## Abstract
Aging is a complex biological process involving progressive cellular dysfunction, tissue decline, and increased susceptibility to multiple chronic diseases. A systemic view of aging through its established hallmarks provides a structured framework to understand this complexity and drive therapeutic discovery. Towards this, we present AgingHallmarksDB, an interactive web platform that enables systems-level analysis of hallmark-associated gene sets. Aging-related genes were first curated from seven established resources, and those present in at least 2 of these resources were considered as consensus aging-related genes. Using functional annotations derived from GO, KEGG, and Reactome, a total of 3111 genes were mapped to the 11 aging hallmarks, of which 2593 were supported by additional experimental or manually curated evidence, with 1089 of these forming the consensus set. Further, AgingHallmarksDB supplements gene annotations with tissue or cell type class specificity, exosomal profiles, and regulatory interactions. The platform allows users to interactively perform systems-level hallmark enrichment analysis across multiple condition-associated gene sets, while seamlessly integrating functional annotations and complex regulatory interactions to elucidate mechanistic hallmark-gene associations. The utility of the resource was explored through hallmark enrichment and network proximity analysis of gene sets corresponding to 11 chronic age-related diseases and PM2.5-associated skin transcriptome to explore relationships between aging hallmarks and disease mechanisms or environmental aging-related signatures. Overall, AgingHallmarksDB will support longevity research by enabling aging hallmark centered analysis, and the resource is accessible at https://cb.imsc.res.in/aginghallmarksdb/.