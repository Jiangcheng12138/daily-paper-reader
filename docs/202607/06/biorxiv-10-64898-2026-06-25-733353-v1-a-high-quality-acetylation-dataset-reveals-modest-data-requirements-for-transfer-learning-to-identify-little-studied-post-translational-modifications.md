---
title: A High-Quality Acetylation Dataset Reveals Modest Data Requirements for Transfer Learning to Identify Little Studied Post-Translational Modifications
title_zh: 高质量乙酰化数据集揭示迁移学习识别鲜少研究的翻译后修饰的中等数据需求
authors: "Hartmaring, Y., Wang, S., Jones, A. R., Vizcaino, J. A., Schlaffner, C. N., Renard, B. Y."
date: 2026-06-30
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.25.733353v1.full.pdf"
tags: ["query:qll"]
score: 7.0
evidence: 用于识别翻译后修饰（乙酰化、泛素化）的数据集和迁移学习
tldr: "翻译后修饰识别因搜索空间巨大而困难，数据稀缺制约深度学习。本文整合约50万高质量乙酰化谱图数据集，微调AHLF模型，发现仅需约28500个光谱（原始数据0.3%）即可达到AUC 0.87/0.90，且数据多样性对泛化关键。结果表明迁移学习可有效缓解少研究修饰的数据瓶颈。"
source: biorxiv
selection_source: fresh_fetch
motivation: 解决乙酰化和泛素化等修饰识别中数据稀缺导致深度学习分类器性能不足的问题。
method: 整合九套乙酰化数据形成约50万PSM数据集，微调AHLF并迭代降采样评估最小数据需求。
result: 乙酰化和泛素化模型AUC分别达0.87和0.90，仅需28500个乙酰化光谱即接近最优。
conclusion: 迁移学习仅需少量高质量数据即可有效识别少研究修饰，数据多样性比数量更重要。
---

## 摘要
翻译后修饰（PTM）的失调与包括癌症和阿尔茨海默病在内的严重病理相关。尽管具有生物学重要性，但由于巨大的组合搜索空间，鉴定修饰肽仍然具有挑战性。虽然搜索受益于对肽修饰状态的先验知识，但大多数PTM的数据稀缺阻碍了如AHLF（肽断裂的专门学习）等准确深度学习分类器的发展。在这里，我们克服了乙酰化和泛素化的数据瓶颈。我们整合了一个包含约50万高质量乙酰化肽谱匹配（PSM）的数据集，这些数据来自九个公开的乙酰化富集数据集。我们分别使用乙酰化数据集和一个包含200万谱图的强泛素化数据集对AHLF进行微调，并通过迭代降采样评估训练所需的最小数据量。在SILAC和无标记子集上分别训练模型也评估了数据多样性的影响。得到的乙酰化和泛素化模型的AUC分别为0.87和0.90。超过28,500个乙酰化谱图（相当于原始模型训练数据的约0.3%），额外的数据仅提供微小的性能提升。最后，我们表明数据多样性有利于泛化能力，而在同质数据源上训练的模型倾向于过拟合其各自的数据类型。所有代码和模型权重可在https://gitlab.com/dacs-hpi/ahlf-ptmai获取。

## Abstract
Dysregulation of post-translational modifications (PTMs) is associated with severe pathologies, including cancers and Alzheimer's disease. Despite their biological importance, identifying modified peptides remains challenging due to the immense combinatorial search space. While searches benefit from prior knowledge of a peptide's modification status, the data scarcity for most PTMs hinders the development of accurate deep learning classifiers like AHLF (ad hoc learning of peptide fragmentation). Here, we overcome this data bottleneck for acetylation and ubiquitination. We harmonised a dataset with about 500,000 high quality acetylated peptide-spectrum matches (PSMs) from nine publicly available acetylation-enriched datasets. We fine-tuned AHLF with the acetylation and a 2-million spectra strong ubiquitination dataset separately and assessed the minimum data requirement for training by iteratively downsampling. Training separate models on SILAC and label-free subsets also assessed the impact of data diversity. The resulting acetylation and ubiquitination models achieve an AUC of 0.87 and 0.90 respectively. Beyond 28,500 acetylated spectra, corresponding to roughly 0.3% of the original model's training data, additional data just provides minor performance gains. Finally, we show that data diversity is beneficial for generalizability, while models trained on homogeneous data sources tend to overfit to their respective data type. All code, and model weights are available at https://gitlab.com/dacs-hpi/ahlf-ptmai.