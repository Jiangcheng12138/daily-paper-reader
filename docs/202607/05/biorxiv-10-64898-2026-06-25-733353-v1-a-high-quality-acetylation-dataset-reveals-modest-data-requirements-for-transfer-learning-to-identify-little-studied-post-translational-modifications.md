---
title: A High-Quality Acetylation Dataset Reveals Modest Data Requirements for Transfer Learning to Identify Little Studied Post-Translational Modifications
title_zh: 一个高质量乙酰化数据集揭示迁移学习识别少研究翻译后修饰的适度数据需求
authors: "Hartmaring, Y., Wang, S., Jones, A. R., Vizcaino, J. A., Schlaffner, C. N., Renard, B. Y."
date: 2026-06-30
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.25.733353v1.full.pdf"
tags: ["query:qll"]
score: 6.0
evidence: 翻译后修饰数据集和迁移学习方法
tldr: "翻译后修饰鉴定面临数据稀缺难题。本研究整合九组公开数据构建约50万高质量乙酰化谱数据集，微调深度学习模型AHLF。实验表明，仅需28,500个谱图即可达到接近最优性能（AUC 0.87），数据多样性提升泛化性，而单一数据源易致过拟合。该工作为少数修饰的深度学习鉴定提供了低成本数据需求的有效指导。"
source: biorxiv
selection_source: fresh_fetch
motivation: 大多数翻译后修饰数据稀缺，阻碍深度学习分类器开发，需探究最小数据需求及数据多样性的影响。
method: 整合九组公开乙酰化富集数据得到约50万PSMs，微调AHLF并迭代下采样评估数据量，同时训练SILAC和label-free子集对比。
result: "乙酰化和泛素化模型AUC分别达0.87和0.90；超过28,500个乙酰化谱后性能增益微小，多样性数据比同质数据泛化性更优。"
conclusion: 高质量小数据集即可训练有效鉴定模型，代码与权重公开，为稀缺修饰研究提供可复现的指导。
---

## 摘要
翻译后修饰（PTM）的失调与严重的病理状况相关，包括癌症和阿尔茨海默病。尽管它们具有生物学重要性，但由于巨大的组合搜索空间，识别修饰肽仍然具有挑战性。虽然搜索受益于对肽修饰状态的先验知识，但大多数PTM的数据稀缺阻碍了像AHLF（肽碎裂的即时学习）这样准确的深度学习分类器的发展。在这里，我们克服了乙酰化和泛素化的数据瓶颈。我们从九个公开可用的乙酰化富集数据集中协调了一个包含约50万高质量乙酰化肽谱匹配（PSM）的数据集。我们分别使用乙酰化数据集和一个包含200万光谱的强泛素化数据集对AHLF进行了微调，并通过迭代降采样评估了训练的最小数据需求。在SILAC和无标记子集上分别训练模型也评估了数据多样性的影响。得到的乙酰化和泛素化模型分别达到了0.87和0.90的AUC。超过28,500个乙酰化光谱（大约相当于原始模型训练数据的0.3%）后，额外的数据仅带来微小的性能提升。最后，我们表明数据多样性有利于泛化性，而在同质数据源上训练的模型倾向于过拟合其各自的数据类型。所有代码和模型权重可在https://gitlab.com/dacs-hpi/ahlf-ptmai获取。

## Abstract
Dysregulation of post-translational modifications (PTMs) is associated with severe pathologies, including cancers and Alzheimers disease. Despite their biological importance, identifying modified peptides remains challenging due to the immense combinatorial search space. While searches benefit from prior knowledge of a peptides modification status, the data scarcity for most PTMs hinders the development of accurate deep learning classifiers like AHLF (ad hoc learning of peptide fragmentation). Here, we overcome this data bottle-neck for acetylation and ubiquitination. We harmonised a dataset with about 500,000 high quality acetylated peptide-spectrum matches (PSMs) from nine publicly available acetylation-enriched datasets. We fine-tuned AHLF with the acetylation and a 2-million spectra strong ubiquitination dataset separately and assessed the minimum data requirement for training by iteratively downsampling. Training separate models on SILAC and label-free subsets also assessed the impact of data diversity. The resulting acetylation and ubiquitination models achieve an AUC of 0.87 and 0.90 respectively. Beyond 28,500 acetylated spectra, corresponding to roughly 0.3% of the original models training data, additional data just provides minor performance gains. Finally, we show that data diversity is beneficial for generalizability, while models trained on homogeneous data sources tend to overfit to their respective data type. All code, and model weights are available at https://gitlab.com/dacs-hpi/ahlf-ptmai.