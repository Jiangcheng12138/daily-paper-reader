---
title: "SenNet Portal: Build, Optimization and Usage"
title_zh: SenNet 门户：构建、优化与应用
authors: "Borner, K., Blood, P. D., Silverstein, J. C., Ruffalo, M., Satija, R., Gehlenborg, N., Honick, B., Bueckle, A., Jain, Y., Qaurooni, D., Shirey, B., Sibilla, M., Metis, K., Bisciotti, J., Morgan, R. S., Betancur, D., Sablosky, G. R., Turner, M. L., Kim, S.-J., Lee, P. J., Bartz, J., Domanskyi, S., Peters, S. T., Enninful, A., Farzad, N., Fan, R., SenNet Team,, Herr, B. W."
date: 2026-05-04
pdf: "https://www.biorxiv.org/content/10.64898/2026.02.06.704469v2.full.pdf"
tags: ["query:qll"]
score: 7.0
evidence: 提供跨寿命细胞衰老的多组织数据集平台
tldr: 细胞衰老是衰老的核心特征，但其异质性给系统研究带来了挑战。SenNet计划通过建立SenNet数据门户，整合了来自人类和老鼠的多种组织、多模态数据集（如单细胞、空间组学等）。该门户采用混合云微服务架构，提供标准化的数据处理流程、生物标志物目录和分析工具，旨在为全球研究者提供一个全面识别和表征衰老细胞的公共平台，推动衰老机制及相关疾病的研究。
source: biorxiv
selection_source: fresh_fetch
motivation: 针对细胞衰老的异质性和背景依赖性导致系统研究受限的问题，亟需一个统一的平台来整合和标准化多模态衰老数据。
method: 构建了一个基于混合云微服务架构的SenNet数据门户，集成了数据提交、管理、标准化处理流程、空间背景映射及跨物种数据访问功能。
result: 截至2026年4月，该门户已托管来自15个器官、6种检测类型的2041个公开数据集，并提供了丰富的生物标志物目录和标准化实验协议。
conclusion: SenNet门户为衰老研究提供了关键的基础设施和资源，通过促进多模态数据的探索与共享，显著提升了衰老细胞表征和生物标志物发现的能力。
---

## 摘要
细胞衰老是衰老的一个标志，也是各组织功能衰退的驱动因素，但其异质性和背景依赖性限制了系统性研究。公共基金细胞衰老网络（SenNet）计划通过生成多模态、多组织数据集来应对这一挑战，这些数据集描绘了人类整个生命周期及互补小鼠模型中的衰老细胞特征。SenNet 数据门户（https://data.sennetconsortium.org）作为这些资源的公共门户，提供对统一的单细胞、空间、成像、转录组学和蛋白质组学数据的开放访问；此外还提供衰老生物标志物目录以及可用于全面识别和表征小鼠及人类组织中衰老细胞的标准协议。截至 2026 年 4 月，该门户托管了跨越 15 个器官、使用 6 种通用分析类型的 2,041 个公开可用的人类和小鼠数据集。来自 13 个组织图谱中心（TMC）和 12 个技术开发与应用（TDA）组件的专家贡献了组织数据、分析数据、识别衰老生物标志物，并就跨组织抗体统一的面板达成一致。他们还将人类组织数据注册到人类参考图谱（HRA）中，并开发了用于对这些数据进行多尺度和多模态探索的用户界面。该门户由联盟组织与数据协调中心（CODCC）基于可扩展的混合云微服务架构构建，支持数据提交、管理、集成分析、空间背景映射，以及对衰老研究至关重要的跨物种数据的统一访问。本文介绍了用户需求、门户架构、数据处理工作流以及专注于衰老的分析工具；展示了在生物标志物发现、质量基准测试、假设生成、空间分析、高性价比分析和细胞距离分布分析中的应用场景；以及广大研究人员社区的效用和使用情况。讨论了当前的局限性和计划中的扩展，包括扩展的空间组学发布和改进的衰老表型（senotype）表征工具。SenNet 协议、代码和用户界面可在 https://docs.sennetconsortium.org/apis 免费获取。

## Abstract
Cellular senescence is a hallmark of aging and a driver of functional decline across tissues, yet its heterogeneity and context dependence have limited systematic study. The Common Funds Cellular Senescence Network (SenNet) Program addresses this challenge by generating multimodal, multi-tissue datasets that profile senescent cells across the human lifespan and complementary mouse models. The SenNet Data Portal (https://data.sennetconsortium.org) serves as the public gateway to these resources, providing open access to harmonized single-cell, spatial, imaging, transcriptomic, and proteomic data; senescence biomarker catalogs; and standardized protocols that can be used to comprehensively identify and characterize senescent cells in mouse and human tissue. As of April 2026, the portal hosts 2,041 publicly available human and mouse datasets across 15 organs using 6 general assay types. Experts from 13 Tissue Mapping Centers (TMCs) and 12 Technology Development and Application (TDAs) components contribute tissue data, analyze data, identify senescent biomarkers, and agree on panels for cross-tissue antibody harmonization. They also register human tissue data into the Human Reference Atlas (HRA) and develop user interfaces for the multiscale and multimodal exploration of this data. Built on a scalable hybrid cloud microservices architecture by the Consortium Organization and Data Coordinating Center (CODCC), the Portal enables data submission, management, integrated analysis, spatial context mapping, and harmonized access to cross-species data critical for aging research. This paper presents user needs, the Portals architecture, data processing workflows, and senescence-focused analytical tools; usage scenarios illustrating applications in biomarker discovery, quality benchmarking, hypothesis generation, spatial analysis, cost-efficient profiling, and cell distance distribution analysis; and utility and usage by the larger researcher community. Current limitations and planned extensions--including expanded spatial-omics releases and improved tools for senotype characterization--are discussed. SenNet protocols, code, and user interfaces are freely available on https://docs.sennetconsortium.org/apis.