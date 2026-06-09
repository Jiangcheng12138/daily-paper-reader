---
title: "CLASPP: A unified model for predicting post-translational modifications"
title_zh: CLASPP：预测翻译后修饰的统一模型
authors: "Gravel, N., Zhou, Z., Fang, R., Soleymani, S., Kannan, N."
date: 2026-06-07
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.04.729962v1.full.pdf"
tags: ["query:qll"]
score: 7.0
evidence: 用于预测翻译后修饰类型的统一模型
tldr: 翻译后修饰（PTM）预测面临数据不平衡和模型碎片化问题。CLASPP模型通过对比学习和分层数据组织，统一预测12种主要PTM类型，性能优于现有工具。其多阶段训练和高质量数据集提升了预测准确性，并能在不同物种间泛化。该工作提供了标准化数据集和开源模型，为PTM预测研究奠定了基础。
source: biorxiv
selection_source: fresh_fetch
motivation: 现有PTM预测模型因数据不平衡多采用单类型或集成方法，缺乏统一模型，限制了跨类型预测性能。
method: 提出CLASPP模型，结合无监督聚类欠采样和对比学习，采用分层数据组织与多阶段训练策略，基于蛋白质语言模型提取序列特征。
result: 在12种主要PTM类型预测上持续超越现有工具，跨物种预测表现稳健，并成功验证了DCLK3激酶的泛素化位点。
conclusion: CLASPP是一种统一的PTM预测模型，有效解决数据不平衡瓶颈，并提供标准化数据集与开源工具，推动功能蛋白质组学研究。
---

## 摘要
翻译后修饰（PTM）是调控细胞通路和增加蛋白质组功能多样性的基本机制。准确预测初级序列中特定位点可能发生的PTM类型是功能蛋白质组学中的一个关键挑战。现有的PTM预测模型主要关注单一PTM类型，或采用集成方法结合多个模型来预测不同的PTM类型。这种碎片化很大程度上是由于不同PTM类型的数据可用性存在巨大不平衡，使得难以用单一模型预测多种PTM类型。为了解决这一局限性，我们提出了基于对比学习注意力的分层PTM预测器（CLASPP），这是一个统一的PTM预测模型。CLASPP通过利用无监督聚类欠采样和针对PTM数据定制的新型对比学习框架来解决不平衡挑战。此外，我们的层次化数据组织和整理通过平衡单个PTM类型的表示来提升CLASPP的性能，并为训练和验证未来模型设计提供了标准化数据集。借鉴图像和自然语言处理领域的进展，CLASPP模型采用多阶段训练策略和高质量、精心整理的训练数据集来提高PTM预测性能。为了揭示对比学习阶段学到的内容，CLASPP模型被证明能够区分已知的蛋白激酶底物特异性谱，作为一种可解释性形式。最后，我们评估了CLASPP在不同模式生物中预测PTM的应用，以及在研究不足的DCLK3激酶中实验验证的泛素化位点。总体而言，CLASPP代表了一个统一的PTM预测模型，解决了数据不平衡的关键瓶颈，并为生物数据整理提供了新策略，从而提高了跨不同生物的PTM类型预测性能。

作者总结：翻译后修饰（PTM）是蛋白质经历的重要变化，影响细胞功能、通讯和疾病的几乎所有方面。由于PTM类型的多样性和现有注释流程的限制，准确预测这些修饰发生的位置和方式具有挑战性。本研究引入了一种统一的深度学习方法，称为CLASPP，利用对比学习仅从初级蛋白质序列同时预测多种PTM类型。通过采用先进的数据平衡和采样方法，CLASPP确保了罕见和常见修饰的可靠预测。该模型利用预训练的蛋白质语言模型来捕获初级蛋白质序列中编码的序列和结构特征。测试结果表明，CLASPP在预测12种主要PTM类型方面持续优于现有工具，其多功能性使得在不同物种中（不仅限于人类蛋白质）都能进行稳健的预测。最终模型、数据整理和训练数据集可免费获取，以供更广泛使用和复现（https://github.com/gravelCompBio/Claspp_forward）。

## Abstract
Post-Translational Modifications (PTMs) are a fundamental mechanism for regulating cellular pathways and increasing the functional diversity of the proteome. Accurately predicting the PTM types that are likely to occur at a given site in the primary sequence is a key challenge in functional proteomics. Existing PTM prediction models predominantly focus on either single PTM types or employ ensemble methods that combine multiple models to predict different PTM types. This fragmentation is largely driven by the vast imbalance in data availability across PTM types, making it difficult to predict multiple PTM types with a single model. To address this limitation, we present the Contrastively Learned Attention-based Stratified PTM Predictor (CLASPP), a unified PTM prediction model. CLASPP addresses imbalance challenges by leveraging unsupervised clustering-based undersampling and a novel contrastive learning framework tailored to PTM data. Additionally, our hierarchical data organization and curation are shown to improve CLASPPs performance by balancing the representation of individual PTM types and provides a standardized dataset to train and validate future model designs. Drawing inspiration from advancements in image and natural language processing, the CLASPP model employs a multi-stage training strategy and a high-quality, curated training dataset to improve PTM prediction performance. To uncover what is learned during the contrastive learning stage, the CLASPP model is shown to distinguish known protein kinase substrate specificity profiles as a form of explainability. Finally, we evaluate the application of CLASPP in predicting PTMs in different model organisms and experimentally validated ubiquitination sites in the understudied DCLK3 kinase. Overall, CLASPP represents a unified model for PTM prediction that addresses key bottlenecks in data imbalance and offers new strategies for biological data curation, thereby improving PTM-type prediction performance across diverse organisms.

Author summaryPost-translational modifications (PTMs) are essential changes that proteins undergo, influencing nearly every aspect of cell function, communication, and disease. Accurately predicting where and how these modifications occur is challenging due to the diversity of PTM types and the limitations of existing annotation pipelines. This study introduces a unified deep learning approach, termed CLASPP, leveraging contrastive learning to predict multiple PTM types simultaneously from primary protein sequence alone. By employing advanced data balancing and sampling methods, CLASPP ensures reliable predictions for rare and common modifications. The model utilizes a pre-trained protein language model to capture sequence and structural features encoded in the primary protein sequence. Test results demonstrate that CLASPP consistently surpasses existing tools in predicting 12 major PTM types, and its versatility enables robust predictions across species, not just in human proteins. The final model, data curation, and training datasets are freely accessible for broader use and reproducibility (https://github.com/gravelCompBio/Claspp_forward).