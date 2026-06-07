---
title: "CLASPP: A unified model for predicting post-translational modifications"
title_zh: "CLASPP: 用于预测翻译后修饰的统一模型"
authors: "Gravel, N., Zhou, Z., Fang, R., Soleymani, S., Kannan, N."
date: 2026-06-07
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.04.729962v1.full.pdf"
tags: ["query:qll"]
score: 6.0
evidence: 统一的翻译后修饰预测模型，可应用于卵巢衰老研究
tldr: 翻译后修饰(PTM)预测中数据严重不平衡，现有模型多为单类型或集成方法。CLASPP通过对比学习、聚类欠采样和分层数据组织构建统一预测模型，在多种模式生物和DCLK3激酶泛素化位点上验证了性能提升，并展现了可解释性。该工作解决了数据不平衡瓶颈，提供了新的数据策展策略。
source: biorxiv
selection_source: fresh_fetch
motivation: 现有PTM预测模型因数据不平衡难以用单一模型预测多种PTM类型，需要统一框架解决碎片化问题。
method: 采用对比学习、无监督聚类欠采样和多阶段训练策略，结合分层数据组织以平衡PTM类型表示。
result: 在多种模式生物和DCLK3激酶泛素化位点上实验验证，预测性能优于现有方法且具可解释性。
conclusion: CLASPP作为统一模型解决了PTM预测中的数据不平衡，提供了新策展策略并跨生物提升预测性能。
---

## 摘要
翻译后修饰（PTMs）是调控细胞通路和增加蛋白质组功能多样性的基本机制。准确预测一级序列中特定位点可能发生的PTM类型是功能蛋白质组学中的一个关键挑战。现有的PTM预测模型主要关注单一PTM类型，或者采用集成方法结合多个模型来预测不同的PTM类型。这种碎片化主要是由PTM类型之间数据可用性的巨大不平衡导致的，使得用单一模型预测多种PTM类型变得困难。为了解决这一局限，我们提出了对比学习注意力引导的分层PTM预测器（CLASPP），这是一个统一的PTM预测模型。CLASPP通过利用基于无监督聚类的欠采样和一种针对PTM数据定制的新型对比学习框架来应对不平衡挑战。此外，我们展示了分层数据组织和整理通过平衡单个PTM类型的表示来提升CLASPP的性能，并为训练和验证未来模型设计提供了标准化数据集。受图像和自然语言处理领域进展的启发，CLASPP模型采用多阶段训练策略和高质量、精心整理的训练数据集来提高PTM预测性能。为了揭示对比学习阶段学到的内容，CLASPP模型被证明能够区分已知的蛋白激酶底物特异性谱，作为一种可解释性形式。最后，我们评估了CLASPP在不同模式生物中预测PTM的应用，以及在研究不足的DCLK3激酶中经实验验证的泛素化位点。总体而言，CLASPP代表了一种统一的PTM预测模型，解决了数据不平衡的关键瓶颈，并为生物数据整理提供了新策略，从而提高了跨不同生物的PTM类型预测性能。

## Abstract
Post-Translational Modifications (PTMs) are a fundamental mechanism for regulating cellular pathways and increasing the functional diversity of the proteome. Accurately predicting the PTM types that are likely to occur at a given site in the primary sequence is a key challenge in functional proteomics. Existing PTM prediction models predominantly focus on either single PTM types or employ ensemble methods that combine multiple models to predict different PTM types. This fragmentation is largely driven by the vast imbalance in data availability across PTM types, making it difficult to predict multiple PTM types with a single model. To address this limitation, we present the Contrastively Learned Attention-based Stratified PTM Predictor (CLASPP), a unified PTM prediction model. CLASPP addresses imbalance challenges by leveraging unsupervised clustering-based undersampling and a novel contrastive learning framework tailored to PTM data. Additionally, our hierarchical data organization and curation are shown to improve CLASPP's performance by balancing the representation of individual PTM types and provides a standardized dataset to train and validate future model designs. Drawing inspiration from advancements in image and natural language processing, the CLASPP model employs a multi-stage training strategy and a high-quality, curated training dataset to improve PTM prediction performance. To uncover what is learned during the contrastive learning stage, the CLASPP model is shown to distinguish known protein kinase substrate specificity profiles as a form of explainability. Finally, we evaluate the application of CLASPP in predicting PTMs in different model organisms and experimentally validated ubiquitination sites in the understudied DCLK3 kinase. Overall, CLASPP represents a unified model for PTM prediction that addresses key bottlenecks in data imbalance and offers new strategies for biological data curation, thereby improving PTM-type prediction performance across diverse organisms.