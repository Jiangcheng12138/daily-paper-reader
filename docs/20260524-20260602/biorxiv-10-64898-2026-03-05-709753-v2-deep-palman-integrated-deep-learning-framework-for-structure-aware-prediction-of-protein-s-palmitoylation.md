---
title: Deep-Palm：an integrated deep learning framework for structure-aware prediction of protein S-Palmitoylation
title_zh: Deep-Palm：一种用于蛋白质S-棕榈酰化结构感知预测的集成深度学习框架
authors: "Deng, M., Huang, J., Wang, W., Fu, S., Wang, H., Li, L., Kang, Y.-J., Xu, B."
date: 2026-05-28
pdf: "https://www.biorxiv.org/content/10.64898/2026.03.05.709753v2.full.pdf"
tags: ["query:qll"]
score: 8.0
evidence: 预测S-棕榈酰化位点，直接相关于研究其在衰老中的作用
tldr: 蛋白质S-棕榈酰化是一种可逆脂质修饰，调控蛋白定位与信号传导，其异常与癌症及耐药相关，实验鉴定费力。本文提出Deep-Palm深度学习框架，整合氨基酸序列、理化性质、ESM嵌入和空间结构四分支信息。测试集AUC达0.950，优于pCysMod、MusiteDeep、GPS-Palm等方法，在不同序列上下文和GO功能组中表现稳定。独立质谱数据验证其能敏感识别新棕榈酰化位点，为大规模候选位点优先排序提供了准确且生物信息丰富的工具。
source: biorxiv
selection_source: fresh_fetch
motivation: 实验鉴定S-棕榈酰化位点劳动密集，亟需计算工具辅助大规模候选位点筛选。
method: Deep-Palm集成四个分支：氨基酸序列、理化性质、ESM嵌入和空间结构，进行多层面特征融合。
result: 测试集AUC为0.950，超越现有预测器，并在多样场景中保持稳定性能。
conclusion: Deep-Palm为S-棕榈酰化位点预测提供了准确且生物学可解释的框架，有助于发现新修饰位点。
---

## 摘要
蛋白质S-棕榈酰化是一种可逆的脂质修饰，调控蛋白质的定位、运输和信号传导。其失调与癌症和治疗耐药性相关，因此准确的位点注释对于理解疾病相关的调控机制至关重要。然而，实验鉴定S-棕榈酰化位点仍然费力，突显了对能够支持大规模候选位点优先排序的计算工具的需求。S-棕榈酰化位点识别需要整合围绕半胱氨酸残基的多层次信息，包括序列上下文、局部蛋白质性质和结构特征。我们提出了Deep-Palm，一个整合四个互补分支的深度学习框架：氨基酸序列、理化性质、ESM嵌入和空间结构。在测试集上，Deep-Palm达到了0.950的AUC，并优于对比预测器，包括pCysMod、MusiteDeep和GPS-Palm。Deep-Palm在不同半胱氨酸序列上下文和基因本体功能组中也表现出稳定的性能。特征层面分析揭示了棕榈酰化与非棕榈酰化肽段窗口之间不同的空间结构和蛋白质性质模式。独立的质谱数据集进一步证明了Deep-Palm灵敏识别先前未注释的S-棕榈酰化位点的能力。总之，Deep-Palm为S-棕榈酰化位点预测提供了一个准确且具有生物学信息的框架，有助于发现新的候选S-棕榈酰化位点。

## Abstract
Protein S-palmitoylation is a reversible lipid modification that regulates protein localization, trafficking, and signaling. Its dysregulation has been implicated in cancer and therapeutic resistance, making accurate site annotation important for understanding disease-related regulatory mechanisms. However, experimental identification of S-palmitoylation sites remains labor-intensive, highlighting the need for computational tools that can support large-scale candidate-site prioritization. S-palmitoylation-site recognition requires the integration of multiple levels of information surrounding candidate cysteine residues, including sequence context, local protein properties and structural features. Here, we present Deep-Palm, a deep learning framework that integrates four complementary branches: amino acid sequence, physicochemical properties, ESM embedding and spatial structure. On the testing set, Deep-Palm achieved an AUC of 0.950 and outperformed the compared predictors, including pCysMod, MusiteDeep and GPS-Palm. Deep-Palm also showed stable performance across diverse cysteine sequence contexts and Gene Ontology functional groups. Feature-level analyses revealed distinct spatial structural and protein property patterns between palmitoylated and non-palmitoylated peptide windows. Independent mass spectrometry datasets further demonstrated the ability of Deep-Palm to sensitively identify previously unannotated S-palmitoylation sites. Together, Deep-Palm provides an accurate and biologically informative framework for S-palmitoylation-site prediction, facilitating the discovery of novel candidate S-palmitoylation sites.