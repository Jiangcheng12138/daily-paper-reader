---
title: Spatial Organellomics Maps Cell State Diversity and Metabolic Adaptation in Tissues
title_zh: 空间细胞器组学描绘组织中的细胞状态多样性与代谢适应
authors: "Adhikari, R., Hillsley, A., Johnson, A. D., Gao, S. M., Espinosa-Medina, I., Funke, J., Feliciano, D."
date: 2026-04-09
pdf: "https://www.biorxiv.org/content/10.1101/2024.12.06.627285v2.full.pdf"
tags: ["query:qll"]
score: 6.0
evidence: 绘制组织中的细胞状态多样性和代谢适应图谱
tldr: 该研究开发了空间细胞器组学（sOrganellomics）成像工作流，利用机器学习分析多细胞器特征来定义和映射细胞状态。研究发现肝脏中的肝细胞并非传统的同质分带分布，而是以复杂的交织群落形式存在，并揭示了营养压力下线粒体结构与生物能量的异质性重塑，为理解组织代谢适应和疾病进展提供了新工具。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2024-12-06-627285-v2/fig-001.webp\", \"caption\": \"Fig. 5. Organelle remodeling during fasting links structural state transitions to functional adaptation in vivo. (A) PCA visualization of hepatocyte categories from control and fasted livers,\", \"page\": 26, \"index\": 1, \"width\": 993, \"height\": 1000}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2024-12-06-627285-v2/fig-002.webp\", \"caption\": \"Fig. 3. sOrganellomics reveals sub-zonal diversity and putative metabolic specialization of hepatocyte states. (A) Schematic of the classical model of liver zonation with three zones along\", \"page\": 22, \"index\": 2, \"width\": 995, \"height\": 1260}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2024-12-06-627285-v2/fig-003.webp\", \"caption\": \"Fig. 6. Organelle signatures enable predictive modeling of hepatocyte states and disease progression. (A) Schematic of the multilayer perceptron (MLP) architecture used to predict\", \"page\": 28, \"index\": 3, \"width\": 985, \"height\": 1166}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2024-12-06-627285-v2/fig-004.webp\", \"caption\": \"Fig. 1. sOrganellomics quantifies multi-organelle architecture to define cell states across metabolic organs. (A) Schematic illustrating how multiple layers of cellular regulation shape\", \"page\": 19, \"index\": 4, \"width\": 1004, \"height\": 648}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2024-12-06-627285-v2/fig-005.webp\", \"caption\": \"Fig. 4. Nutritional perturbations remodel sub-zonal hepatocyte heterogeneity across the PV– CV axis. (A–C) Representative confocal images of liver acini from control-fed (A), overnight-\", \"page\": 24, \"index\": 5, \"width\": 974, \"height\": 1300}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2024-12-06-627285-v2/fig-006.webp\", \"caption\": \"Fig. 2. Single-cell mapping of organelle architecture reveals hepatocyte heterogeneity beyond\", \"page\": 20, \"index\": 6, \"width\": 974, \"height\": 1177}]"
motivation: 传统的转录组分析难以捕捉细胞器结构所蕴含的功能代谢信息，限制了对细胞状态多样性的深入理解。
method: 开发了集成自动分割与机器学习的sOrganellomics成像技术，通过多细胞器形态特征对细胞状态进行空间制图。
result: 揭示了肝细胞以交织群落而非单纯分带形式组织，并发现禁食会诱发线粒体膜电位改变及生物能量异质性。
conclusion: 细胞器架构可作为衡量组织内功能细胞状态多样性和代谢适应性的可扩展读数。
---

## 摘要
细胞状态多样性驱动着组织的适应性、修复和疾病韧性，但全面捕捉这种细胞复杂性仍是一项挑战。目前大多数方法依赖于转录谱分析，往往忽略了蕴含在细胞器结构中的功能性见解，而细胞器结构是细胞代谢和应激的关键指标。在此，我们介绍了空间细胞器组学（sOrganellomics），这是一种整合了自动分割与机器学习的成像工作流，旨在基于多细胞器特征对细胞状态进行分类和空间映射。在代谢特化器官中，这些特征能够区分器官特异性的细胞身份。在肝脏中，sOrganellomics 揭示了一种此前未被认识的肝细胞组织形式：不同的肝细胞状态形成了交错混杂的群落，而非经典的同质化梯度分区，且这种模式会被营养压力所破坏。活体成像进一步将禁食相关的结构重塑与体内线粒体膜电位改变及生物能量异质性联系起来。该方法描绘了代谢转变和早期疾病进展，确立了细胞器架构作为组织中功能性细胞状态多样性的可扩展读数。

## Abstract
Cell state diversity drives tissue adaptability, repair, and disease resilience, but fully capturing this cellular complexity remains a challenge. Most current approaches rely on transcriptional profiling and often overlook functional insights embedded in organelle structure, key indicators of cellular metabolism and stress. Here, we introduce spatial Organellomics (sOrganellomics), an imaging workflow integrating automated segmentation with machine learning to classify and spatially map cell states based on multi-organelle features. Across metabolically specialized organs, these features distinguish organ-specific cellular identities. In the liver, sOrganellomics reveals a previously unrecognized hepatocyte organization: different hepatocyte states form intermixed communities rather than classical homogeneous graded zones, a pattern disrupted by nutritional stress. Intravital imaging further links fasting-associated architectural remodeling to altered mitochondrial membrane potential and bioenergetic heterogeneity in vivo. This approach maps metabolic transitions and early disease progression, establishing organelle architecture as a scalable readout of functional cell state diversity in tissues.