---
title: "SenNet Portal: Build, Optimization and Usage"
title_zh: SenNet 门户：构建、优化与应用
authors: "Borner, K., Blood, P. D., Silverstein, J. C., Ruffalo, M., Satija, R., Gehlenborg, N., Honick, B., Bueckle, A., Jain, Y., Qaurooni, D., Shirey, B., Sibilla, M., Metis, K., Bisciotti, J., Morgan, R. S., Betancur, D., Sablosky, G. R., Turner, M. L., Kim, S.-J., Lee, P. J., Bartz, J., Domanskyi, S., Peters, S. T., Enninful, A., Farzad, N., Fan, R., SenNet Team,, Herr, B. W."
date: 2026-05-04
pdf: "https://www.biorxiv.org/content/10.64898/2026.02.06.704469v2.full.pdf"
tags: ["query:qll"]
score: 8.0
evidence: 跨组织衰老细胞的多模态数据集
tldr: SenNet数据门户是针对细胞衰老研究的综合性公共平台，旨在解决衰老细胞异质性和背景依赖性带来的挑战。该门户整合了来自人类和老鼠15个器官的2000多个多模态数据集，包括单细胞、空间组学和蛋白质组学等。通过提供标准化的实验方案、生物标志物目录和先进的分析工具，SenNet为全球研究人员提供了探索衰老机制、发现生物标志物及进行跨物种比较的关键资源。
source: biorxiv
selection_source: fresh_fetch
motivation: 细胞衰老的异质性和背景依赖性限制了系统性研究，急需一个统一的平台来整合多模态、多组织的衰老细胞数据。
method: 构建了一个基于混合云微服务架构的门户网站，整合了来自多个研究中心的数据提交、标准化处理、空间背景映射及多尺度探索工具。
result: "截至2026年4月，该门户已托管涵盖15个器官、6种主要检测类型的2,041个公开数据集，并提供了标准化的实验协议和生物标志物手册。"
conclusion: SenNet门户为衰老研究提供了关键的基础设施，通过促进数据共享和标准化分析，加速了对衰老细胞在功能衰退中作用的理解。
---

## 摘要
细胞衰老是衰老的一个标志，也是各组织功能衰退的驱动因素，但其异质性和背景依赖性限制了系统性研究。美国国立卫生研究院（NIH）公共基金的细胞衰老网络（SenNet）计划通过生成多模态、多组织数据集来应对这一挑战，这些数据集描绘了人类整个生命周期及互补小鼠模型中的衰老细胞特征。SenNet 数据门户（https://data.sennetconsortium.org）作为这些资源的公共门户，提供对统一的单细胞、空间、成像、转录组学和蛋白质组学数据的开放访问；此外还提供衰老生物标志物目录以及可用于全面识别和表征小鼠及人类组织中衰老细胞的标准协议。截至 2026 年 4 月，该门户托管了涵盖 15 个器官、使用 6 种通用分析类型的 2,041 个公开可用的人类和小鼠数据集。来自 13 个组织图谱中心（TMC）和 12 个技术开发与应用（TDA）组件的专家贡献了组织数据、分析数据、识别衰老生物标志物，并就跨组织抗体统一的面板达成一致。他们还将人类组织数据注册到人类参考图谱（HRA）中，并开发了用于对这些数据进行多尺度和多模态探索的用户界面。该门户由联盟组织与数据协调中心（CODCC）基于可扩展的混合云微服务架构构建，支持数据提交、管理、综合分析、空间背景映射，以及对衰老研究至关重要的跨物种数据的统一访问。本文介绍了用户需求、门户架构、数据处理工作流以及专注于衰老的分析工具；展示了在生物标志物发现、质量基准测试、假设生成、空间分析、高性价比特征分析和细胞距离分布分析中的应用场景；以及广大研究人员群体的效用和使用情况。文中还讨论了当前的局限性和计划中的扩展，包括扩大空间组学数据的发布以及改进衰老表型（senotype）表征工具。SenNet 协议、代码和用户界面可在 https://docs.sennetconsortium.org/apis 免费获取。

## Abstract
Cellular senescence is a hallmark of aging and a driver of functional decline across tissues, yet its heterogeneity and context dependence have limited systematic study. The Common Fund's Cellular Senescence Network (SenNet) Program addresses this challenge by generating multimodal, multi-tissue datasets that profile senescent cells across the human lifespan and complementary mouse models. The SenNet Data Portal (https://data.sennetconsortium.org) serves as the public gateway to these resources, providing open access to harmonized single-cell, spatial, imaging, transcriptomic, and proteomic data; senescence biomarker catalogs; and standardized protocols that can be used to comprehensively identify and characterize senescent cells in mouse and human tissue. As of April 2026, the portal hosts 2,041 publicly available human and mouse datasets across 15 organs using 6 general assay types. Experts from 13 Tissue Mapping Centers (TMCs) and 12 Technology Development and Application (TDAs) components contribute tissue data, analyze data, identify senescent biomarkers, and agree on panels for cross-tissue antibody harmonization. They also register human tissue data into the Human Reference Atlas (HRA) and develop user interfaces for the multiscale and multimodal exploration of this data. Built on a scalable hybrid cloud microservices architecture by the Consortium Organization and Data Coordinating Center (CODCC), the Portal enables data submission, management, integrated analysis, spatial context mapping, and harmonized access to cross-species data critical for aging research. This paper presents user needs, the Portal's architecture, data processing workflows, and senescence-focused analytical tools; usage scenarios illustrating applications in biomarker discovery, quality benchmarking, hypothesis generation, spatial analysis, cost-efficient profiling, and cell distance distribution analysis; and utility and usage by the larger researcher community. Current limitations and planned extensions, including expanded spatial-omics releases and improved tools for senotype characterization, are discussed. SenNet protocols, code, and user interfaces are freely available on https://docs.sennetconsortium.org/apis.