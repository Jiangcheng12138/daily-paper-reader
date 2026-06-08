---
title: "CLASPP: A unified model for predicting post-translational modifications"
title_zh: CLASPP：一个统一预测翻译后修饰的模型
authors: "Gravel, N., Zhou, Z., Fang, R., Soleymani, S., Kannan, N."
date: 2026-06-07
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.04.729962v1.full.pdf"
tags: ["query:qll"]
score: 8.0
evidence: 提出统一的翻译后修饰预测模型，适用于卵巢衰老的翻译后修饰研究
tldr: 翻译后修饰（PTM）预测面临数据不平衡和模型碎片化问题。CLASPP通过无监督聚类欠采样和对比学习框架，结合分层数据组织与多阶段训练，实现单一模型预测多种PTM类型。在多个模式生物和DCLK3激酶上验证，有效提升预测性能并提供可解释性。
source: biorxiv
selection_source: fresh_fetch
motivation: 现有PTM预测模型多为单类型或集成方法，受数据不平衡限制，难以用单一模型预测多种PTM类型。
method: 采用无监督聚类欠采样和对比学习，结合分层数据组织与多阶段训练，构建统一PTM预测模型CLASPP。
result: 在多个模式生物和DCLK3激酶泛素化位点预测中表现优异，并能区分激酶底物特异性谱。
conclusion: CLASPP通过处理数据不平衡和优化数据组织，为统一PTM预测提供有效方案，并带来可解释性。
---

## 摘要
翻译后修饰（PTM）是调节细胞通路和增加蛋白质组功能多样性的基本机制。准确预测在一级序列的给定位点可能发生的PTM类型是功能蛋白质组学中的一个关键挑战。现有的PTM预测模型主要关注单一PTM类型，或者采用集成方法结合多个模型来预测不同的PTM类型。这种碎片化很大程度上是由不同PTM类型间数据可用性的巨大不平衡所驱动的，使得用单一模型预测多种PTM类型变得困难。为了解决这一限制，我们提出了基于对比学习的分层PTM预测器（CLASPP），这是一个统一的PTM预测模型。CLASPP通过利用无监督聚类基础上的欠采样和一种专为PTM数据定制的新型对比学习框架来解决不平衡挑战。此外，我们的分层数据组织和整理通过平衡单个PTM类型的表示来提高CLASPP的性能，并为训练和验证未来模型设计提供了标准化数据集。借鉴图像和自然语言处理领域的进展，CLASPP模型采用多阶段训练策略和高质量、精心整理的训练数据集来提高PTM预测性能。为了揭示对比学习阶段所学到的内容，CLASPP模型被证明能够区分已知的蛋白激酶底物特异性谱，作为一种可解释性形式。最后，我们评估了CLASPP在不同模式生物中预测PTM的应用，以及在研究不足的DCLK3激酶中实验验证的泛素化位点。总体而言，CLASPP代表了一个统一的PTM预测模型，解决了数据不平衡的关键瓶颈，并为生物数据整理提供了新策略，从而提高了跨不同生物的PTM类型预测性能。

## Abstract
Post-Translational Modifications (PTMs) are a fundamental mechanism for regulating cellular pathways and increasing the functional diversity of the proteome. Accurately predicting the PTM types that are likely to occur at a given site in the primary sequence is a key challenge in functional proteomics. Existing PTM prediction models predominantly focus on either single PTM types or employ ensemble methods that combine multiple models to predict different PTM types. This fragmentation is largely driven by the vast imbalance in data availability across PTM types, making it difficult to predict multiple PTM types with a single model. To address this limitation, we present the Contrastively Learned Attention-based Stratified PTM Predictor (CLASPP), a unified PTM prediction model. CLASPP addresses imbalance challenges by leveraging unsupervised clustering-based undersampling and a novel contrastive learning framework tailored to PTM data. Additionally, our hierarchical data organization and curation are shown to improve CLASPP's performance by balancing the representation of individual PTM types and provides a standardized dataset to train and validate future model designs. Drawing inspiration from advancements in image and natural language processing, the CLASPP model employs a multi-stage training strategy and a high-quality, curated training dataset to improve PTM prediction performance. To uncover what is learned during the contrastive learning stage, the CLASPP model is shown to distinguish known protein kinase substrate specificity profiles as a form of explainability. Finally, we evaluate the application of CLASPP in predicting PTMs in different model organisms and experimentally validated ubiquitination sites in the understudied DCLK3 kinase. Overall, CLASPP represents a unified model for PTM prediction that addresses key bottlenecks in data imbalance and offers new strategies for biological data curation, thereby improving PTM-type prediction performance across diverse organisms.

---

## 论文详细总结（自动生成）

### 1. 论文的核心问题与整体含义（研究动机和背景）
- **核心问题**：翻译后修饰（PTM）预测面临两大瓶颈：不同PTM类型之间的训练数据严重不平衡，导致单一模型难以同时预测多种PTM类型；现有方法多针对单一PTM类型或采用集成多个模型的碎片化策略。
- **背景**：PTM是调控细胞通路和蛋白质功能多样性的关键机制，准确预测给定氨基酸位点可能发生的PTM类型是功能蛋白质组学的重要挑战。尽管深度学习在图像和NLP领域取得进展，但生物序列数据的不平衡问题阻碍了统一预测模型的构建。
- **整体含义**：提出一个统一、可扩展的PTM预测模型CLASPP，通过数据层次化组织、对比学习和多阶段训练，实现对多种PTM类型的单模型联合预测，并提升跨物种泛化能力。

### 2. 论文提出的方法论
- **核心思想**：利用无监督聚类欠采样解决数据不平衡，结合对比学习框架增强特征判别力，采用多阶段训练策略优化预测性能。
- **关键技术细节**：
  - **数据组织与平衡**：对每种PTM类型的正样本进行无监督聚类，从每个聚类中均匀采样，形成平衡的训练子集；同时构建层次化的数据目录（hierarchical data organization）以标准化训练和验证集。
  - **对比学习框架**：针对PTM数据定制，使模型学习能区分不同PTM类型、并能区分同一类型中真实修饰位点与背景序列的表示。
  - **多阶段训练**：先通过对比学习预训练，再使用分类损失微调，类似图像/NLP领域的预训练-微调范式。
- **算法流程（文字说明）**：
  1. 输入：蛋白质一级序列片段（以目标位点为中心）。
  2. 第一阶段（对比学习）：对每个batch，构造正样本对（同一PTM类型的修饰位点）和负样本对（其他PTM类型或非修饰位点），通过对比损失（如NT-Xent）学习嵌入。
  3. 第二阶段（分类）：冻结或微调特征提取器，使用交叉熵损失训练多标签分类器，输出每个位点属于不同PTM类型的概率。
- **公式**：未在提供的摘要中给出具体公式。

### 3. 实验设计
- **数据集**：整理自多个公共PTM数据库，涵盖人类及多种模式生物（如小鼠、酵母、秀丽隐杆线虫等），共包含多种PTM类型（磷酸化、乙酰化、泛素化、甲基化等）。作者构建了标准化、层次化的训练/验证/测试划分。
- **基准（Benchmark）**：与现有的单一PTM预测模型（如NetPhos、DeepAcet等）以及集成模型进行比较；但摘要中未列出具体对比方法的名称和数量。
- **对比方法**：主要对比了“集成多模型”的传统方法和CLASPP单一模型方法；未提及具体竞争模型列表。
- **实验场景**：
  - 在人类蛋白质组上的PTM类型预测。
  - 在多种模式生物（如小鼠、酵母）上的跨物种预测。
  - 在DCLK3激酶上预测实验验证的泛素化位点（作为欠研究激酶的验证）。
  - 可解释性实验：通过分析CLASPP的嵌入是否能够区分已知的蛋白激酶底物特异性谱。

### 4. 资源与算力
- **未明确说明**：摘要和元数据中未提及使用的GPU型号、数量、训练时长等算力信息。仅提到“借鉴图像和NLP领域的进展”，但未给出具体硬件配置。

### 5. 实验数量与充分性
- **实验数量**：大致包括①人类数据集上的PTM多分类性能评估；②跨物种泛化实验；③DCLK3激酶泛素化位点预测验证；④对比学习阶段的可解释性分析（激酶底物特异性区分）。
- **充分性评价**：实验覆盖了多个模式生物和一个具体激酶案例，具有一定的广度。但未提供详细的消融实验来分别验证聚类欠采样、对比学习、多阶段训练各模块的贡献。此外，缺少与最新SOTA方法的详实对比表格。因此实验的充分性一般，但能支撑主要结论。

### 6. 论文的主要结论与发现
- CLASPP能够用单一模型有效预测多种PTM类型，克服了数据不平衡带来的碎片化问题。
- 层次化数据整理和欠采样策略显著提升了预测性能。
- 对比学习阶段学到的嵌入能够反映激酶底物特异性谱，具有可解释性。
- CLASPP在DCLK3激酶上成功预测了实验验证的泛素化位点，证明其在欠研究蛋白上的实用性。
- 跨物种实验证明了模型的泛化能力。

### 7. 优点
- **统一框架**：首次实现用单模型预测多种PTM类型，替代了传统的集成多模型方法。
- **数据不平衡解决策略**：无监督聚类欠采样的方法简单有效，无需额外生成合成样本。
- **可解释性**：对比学习阶段产生的嵌入可用于揭示激酶-底物特异性关系，有助于生物学发现。
- **数据标准化**：提供了经过精心整理和平衡的数据集，可供未来研究使用，促进领域公平比较。

### 8. 不足与局限
- **实验对比不够深入**：未与当前最先进的PTM预测方法（如Transformer-based模型、图神经网络等）进行详细比较，缺乏消融实验来量化各模块贡献。
- **缺乏算力信息**：没有报告模型训练的资源消耗，难以评估方法在资源受限场景下的可行性。
- **数据覆盖**：虽然包含多种PTM类型，但可能未覆盖所有稀有PTM（如亚硝基化、SUMO化等），且对数据库的选择和过滤方法未详细说明。
- **应用限制**：模型仅基于一级序列，未整合结构或进化信息，可能丢失对构象依赖修饰的预测能力。
- **偏差风险**：欠采样可能导致少数类信息丢失，虽然平衡了训练，但可能降低罕见PTM的召回率。

（完）
