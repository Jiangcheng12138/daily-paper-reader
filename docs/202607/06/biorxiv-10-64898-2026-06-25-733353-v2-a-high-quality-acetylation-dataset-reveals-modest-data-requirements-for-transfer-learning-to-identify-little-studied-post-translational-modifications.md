---
title: A High-Quality Acetylation Dataset Reveals Modest Data Requirements for Transfer Learning to Identify Little Studied Post-Translational Modifications
title_zh: 一个高质量乙酰化数据集揭示迁移学习识别少研究翻译后修饰的适度数据需求
authors: "Hartmaring, Y., Wang, S., Jones, A. R., Vizcaino, J. A., Schlaffner, C. N., Renard, B. Y."
date: 2026-07-06
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.25.733353v2.full.pdf"
tags: ["query:qll"]
score: 6.0
evidence: 翻译后修饰鉴定数据集和迁移学习方法，可应用于棕榈酰化等PTM研究
tldr: 翻译后修饰鉴定面临数据稀缺挑战。本研究整合9个公开数据集，构建约50万高质量乙酰化谱图，微调AHLF模型。乙酰化和泛素化模型AUC分别达0.87和0.90，仅需约28500个光谱即可接近最优性能，数据多样性可提升泛化性。表明少量高质量数据结合迁移学习可有效应对稀缺修饰识别。
source: biorxiv
selection_source: fresh_fetch
motivation: 针对乙酰化等翻译后修饰数据稀缺导致深度学习分类器难以训练的问题。
method: 整合9个乙酰化富集数据集，获得约50万高质量PSM，微调AHLF模型，并通过降采样评估最小数据需求。
result: 乙酰化和泛素化模型AUC分别为0.87和0.90，仅需28500个乙酰化光谱即可达到近最优性能。
conclusion: 少量高质量数据结合迁移学习可高效识别稀有翻译后修饰，数据多样性有助于提升模型泛化能力。
---

## 摘要
翻译后修饰（PTM）的失调与严重病理相关，包括癌症和阿尔茨海默病。尽管其生物学重要性，但由于巨大的组合搜索空间，鉴定修饰肽仍然具有挑战性。虽然搜索受益于肽修饰状态的先验知识，但大多数PTM的数据稀缺阻碍了像AHLF（肽碎裂的即席学习）这样的准确深度学习分类器的开发。这里，我们克服了乙酰化和泛素化的数据瓶颈。我们整理了一个包含约50万个高质量乙酰化肽谱匹配（PSM）的数据集，来自九个公开的乙酰化富集数据集。我们分别用乙酰化数据集和一个包含200万谱图的强泛素化数据集微调了AHLF，并通过迭代下采样评估了训练的最小数据需求。在SILAC和标签自由子集上单独训练模型也评估了数据多样性的影响。得到的乙酰化和泛素化模型分别达到了0.87和0.90的AUC。超过28,500个乙酰化谱图（约相当于原始模型训练数据的0.3%）后，额外数据仅带来微小的性能提升。最后，我们表明数据多样性有利于泛化性，而在同质数据源上训练的模型倾向于过拟合其各自的数据类型。所有代码和模型权重可在https://gitlab.com/dacs-hpi/ahlf-ptmai获取。

## Abstract
Dysregulation of post-translational modifications (PTMs) is associated with severe pathologies, including cancers and Alzheimer's disease. Despite their biological importance, identifying modified peptides remains challenging due to the immense combinatorial search space. While searches benefit from prior knowledge of a peptide's modification status, the data scarcity for most PTMs hinders the development of accurate deep learning classifiers like AHLF (ad hoc learning of peptide fragmentation). Here, we overcome this data bottleneck for acetylation and ubiquitination. We harmonised a dataset with about 500,000 high quality acetylated peptide-spectrum matches (PSMs) from nine publicly available acetylation-enriched datasets. We fine-tuned AHLF with the acetylation and a 2-million spectra strong ubiquitination dataset separately and assessed the minimum data requirement for training by iteratively downsampling. Training separate models on SILAC and label-free subsets also assessed the impact of data diversity. The resulting acetylation and ubiquitination models achieve an AUC of 0.87 and 0.90 respectively. Beyond 28,500 acetylated spectra, corresponding to roughly 0.3% of the original model's training data, additional data just provides minor performance gains. Finally, we show that data diversity is beneficial for generalizability, while models trained on homogeneous data sources tend to overfit to their respective data type. All code, and model weights are available at https://gitlab.com/dacs-hpi/ahlf-ptmai.