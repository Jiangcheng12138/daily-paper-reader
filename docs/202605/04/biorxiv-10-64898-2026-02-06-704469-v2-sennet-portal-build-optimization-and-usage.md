---
title: "SenNet Portal: Build, Optimization and Usage"
title_zh: SenNet 门户：构建、优化与使用
authors: "Borner, K., Blood, P. D., Silverstein, J. C., Ruffalo, M., Satija, R., Gehlenborg, N., Honick, B., Bueckle, A., Jain, Y., Qaurooni, D., Shirey, B., Sibilla, M., Metis, K., Bisciotti, J., Morgan, R. S., Betancur, D., Sablosky, G. R., Turner, M. L., Kim, S.-J., Lee, P. J., Bartz, J., Domanskyi, S., Peters, S. T., Enninful, A., Farzad, N., Fan, R., SenNet Team,, Herr, B. W."
date: 2026-05-04
pdf: "https://www.biorxiv.org/content/10.64898/2026.02.06.704469v2.full.pdf"
tags: ["query:qll"]
score: 7.0
evidence: 细胞衰老数据集和衰老生物标志物目录
tldr: 细胞衰老是衰老的核心特征，但其异质性使研究面临挑战。SenNet计划通过建立数据门户，整合了人类和小鼠的多模态、多组织数据集，包括单细胞、空间组学和蛋白质组学等。该门户基于混合云架构，提供标准化协议、生物标志物目录及分析工具。目前已涵盖15个器官的2000多个数据集，为衰老细胞的识别、表征及生物标志物发现提供了重要的开放资源和技术支持。
source: biorxiv
selection_source: fresh_fetch
motivation: 针对细胞衰老的异质性和背景依赖性，亟需一个统一的平台来系统性地整合、管理和分析跨组织、跨物种的多模态衰老数据。
method: 构建了基于混合云微服务架构的SenNet数据门户，集成了单细胞、空间组学、影像学等多种数据，并制定了标准化的实验协议与分析工作流。
result: 该门户已公开托管跨15个器官的2041个数据集，并提供了生物标志物目录、空间背景映射及多种衰老相关的分析工具。
conclusion: SenNet门户为全球研究者提供了全面且标准化的衰老研究资源，极大地促进了衰老细胞的精准识别、功能表征及生物标志物的开发。
---

## 摘要
细胞衰老是衰老的一个标志，也是各组织功能衰退的驱动因素，但其异质性和背景依赖性限制了系统性研究。美国国立卫生研究院（NIH）公共基金的细胞衰老网络（SenNet）计划通过生成多模态、多组织数据集来应对这一挑战，这些数据集描绘了人类整个生命周期及互补小鼠模型中的衰老细胞特征。SenNet 数据门户（https://data.sennetconsortium.org）作为这些资源的公共入口，提供了对统一的单细胞、空间、成像、转录组学和蛋白质组学数据的开放访问，以及衰老生物标志物目录和用于全面识别和表征小鼠及人类组织中衰老细胞的标准协议。截至 2026 年 4 月，该门户托管了涵盖 15 个器官、使用 6 种通用分析类型的 2,041 个公开的人类和小鼠数据集。来自 13 个组织图谱中心（TMC）和 12 个技术开发与应用（TDA）组件的专家贡献了组织数据、分析数据、识别衰老生物标志物，并就跨组织抗体统一的面板达成一致。他们还将人类组织数据注册到人类参考图谱（HRA）中，并开发了用于多尺度和多模态探索这些数据的用户界面。该门户由联盟组织和数据协调中心（CODCC）基于可扩展的混合云微服务架构构建，支持数据提交、管理、集成分析、空间背景映射，以及对衰老研究至关重要的跨物种数据的统一访问。本文介绍了用户需求、门户架构、数据处理工作流以及专注于衰老的分析工具；展示了在生物标志物发现、质量基准测试、假设生成、空间分析、高效成本分析和细胞距离分布分析中的应用场景；并阐述了广大研究人员社区的效用和使用情况。文中还讨论了当前的局限性和计划中的扩展，包括扩大空间组学发布和改进衰老表型（senotype）表征工具。SenNet 协议、代码和用户界面可在 https://docs.sennetconsortium.org/apis 免费获取。

## Abstract
Cellular senescence is a hallmark of aging and a driver of functional decline across tissues, yet its heterogeneity and context dependence have limited systematic study. The Common Fund's Cellular Senescence Network (SenNet) Program addresses this challenge by generating multimodal, multi-tissue datasets that profile senescent cells across the human lifespan and complementary mouse models. The SenNet Data Portal (https://data.sennetconsortium.org) serves as the public gateway to these resources, providing open access to harmonized single-cell, spatial, imaging, transcriptomic, and proteomic data; senescence biomarker catalogs; and standardized protocols that can be used to comprehensively identify and characterize senescent cells in mouse and human tissue. As of April 2026, the portal hosts 2,041 publicly available human and mouse datasets across 15 organs using 6 general assay types. Experts from 13 Tissue Mapping Centers (TMCs) and 12 Technology Development and Application (TDAs) components contribute tissue data, analyze data, identify senescent biomarkers, and agree on panels for cross-tissue antibody harmonization. They also register human tissue data into the Human Reference Atlas (HRA) and develop user interfaces for the multiscale and multimodal exploration of this data. Built on a scalable hybrid cloud microservices architecture by the Consortium Organization and Data Coordinating Center (CODCC), the Portal enables data submission, management, integrated analysis, spatial context mapping, and harmonized access to cross-species data critical for aging research. This paper presents user needs, the Portal's architecture, data processing workflows, and senescence-focused analytical tools; usage scenarios illustrating applications in biomarker discovery, quality benchmarking, hypothesis generation, spatial analysis, cost-efficient profiling, and cell distance distribution analysis; and utility and usage by the larger researcher community. Current limitations and planned extensions, including expanded spatial-omics releases and improved tools for senotype characterization, are discussed. SenNet protocols, code, and user interfaces are freely available on https://docs.sennetconsortium.org/apis.