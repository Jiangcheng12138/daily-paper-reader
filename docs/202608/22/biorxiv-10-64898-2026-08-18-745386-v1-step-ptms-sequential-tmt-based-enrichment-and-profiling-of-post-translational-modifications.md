---
title: "STEP-PTMs: Sequential TMT-based Enrichment and Profiling of Post-Translational Modifications"
title_zh: STEP-PTMs：基于TMT的翻译后修饰顺序富集与分析
authors: "Criscuolo, L., Elmkvist, S. B., Nawrocki, A., Jakobsen, L. A., Jensen, P., Jensen, P. T., Huang, H., Havelund, J. K., Faergeman, N. J., Palmisano, G., Bogetofte, H., Larsen, M. R."
date: 2026-08-19
pdf: "https://www.biorxiv.org/content/10.64898/2026.08.18.745386v1.full.pdf"
tags: ["query:qll"]
score: 8.0
evidence: 翻译后修饰富集工作流可直接支持卵巢衰老与纤维化相关的翻译后修饰研究
tldr: 全面解析同一生物样本中的蛋白质丰度与多种翻译后修饰（PTM）及PTM串扰仍具挑战。本文提出STEP-PTM，一种基于TMT多标定量的模块化工作流，可从单份肽段制备中顺序富集磷酸化、半胱氨酸修饰、唾液酸化N-糖基化、赖氨酸乙酰化及棕榈酰化肽段，同时保留非修饰肽用于蛋白质组分析。应用于脑类器官实现逾万蛋白、近三千代谢物及数万修饰肽定量，展示了跨组织普适性，为系统级调控研究提供集成方案。
source: biorxiv
selection_source: fresh_fetch
motivation: 现有方法难以从同一样本中同时分析多种PTM及蛋白丰度，导致PTM串扰研究受限，亟需集成且减少技术变异的工作流。
method: 构建TMT标记后混合的单一多肽池，顺序执行多种PTM富集模块，保留未修饰肽段用于蛋白质组，并结合PTM特异性数据库搜索提升定量准确性。
result: "在脑类器官中定量10,413种蛋白、2,969种代谢物及19,655个磷酸化肽等，并成功应用于多种小鼠组织，验证了广泛适用性。"
conclusion: STEP-PTM实现了多组学与多PTM的并行定量，为系统解析蛋白质表达和修饰调控提供了可扩展的通用平台。
---

## 摘要
从同一种生物样本中对蛋白质丰度和多种翻译后修饰（PTM）进行全面表征，对于理解细胞调控和PTM串扰至关重要，但在分析上仍具挑战性。在此，我们提出了STEP-PTM（基于标签的翻译后修饰顺序富集），这是一种模块化的TMT多重定量工作流程，能够从单一肽段制备中对蛋白质组、代谢组和多种PTM类别进行整合定量分析。蛋白质经酶解后使用串联质量标签（TMT）进行等量标记，并合并为单一多重肽段池，随后进行顺序PTM富集，从而最大限度地减少技术变异、降低样本需求，并促进跨数据集的直接定量整合。

STEP-PTM支持对磷酸化肽段、含游离和可逆修饰半胱氨酸的肽段、唾液酸化N-连接糖肽、赖氨酸乙酰化肽段和S-棕榈酰化肽段进行灵活的顺序富集，同时保留未修饰肽段用于全局蛋白质组分析。PTM特异性数据库搜索进一步提高了鉴定置信度和定量准确性，且该模块化工作流程可根据生物学问题通过添加或省略富集模块而简便地调整。

将STEP-PTM应用于TMT16-多重脑类器官，我们实现了对同一种生物样本中10,413种蛋白质、2,969种代谢物、19,655条磷酸化肽段、28,876条含可逆修饰半胱氨酸的肽段、9,723条含游离半胱氨酸的肽段、1,716条完整唾液酸化N-连接糖肽和771条赖氨酸乙酰化肽段的定量。我们还进一步展示了该工作流程在多种小鼠组织中的适用性，突显了其在跨多样生物学模型中对蛋白质表达和PTM调控进行整合系统级表征的广泛实用性。

## Abstract
Comprehensive characterization of protein abundance and multiple post-translational modifications (PTMs) from the same biological samples is essential for understanding cellular regulation and PTM crosstalk but remains analytically challenging. Here, we present STEP-PTM (Sequential Tag-based Enrichment of Post-Translational Modifications), a modular TMT-multiplexed workflow that enables integrated quantitative analysis of the proteome, metabolome and multiple PTM classes from a single peptide preparation. Proteins are digested, isobarically labeled using tandem mass tags (TMT), and combined into a single multiplexed peptide pool prior to sequential PTM enrichment, thereby minimizing technical variability, reducing sample requirements and facilitating direct quantitative integration across datasets.

STEP-PTM supports flexible sequential enrichment of phosphopeptides, peptides containing free and reversibly modified cysteines, sialylated N-linked glycopeptides, lysine-acetylated peptides and S-palmitoylated peptides, while preserving non-modified peptides for global proteome analysis. PTM-specific database searches further improve identification confidence and quantitative accuracy, and the modular workflow can readily be adapted by incorporating or omitting enrichment modules according to the biological question.

Application of STEP-PTM to TMT16-plex cerebral brain organoids enabled the quantification of 10,413 proteins, 2,969 metabolites, 19,655 phosphopeptides, 28,876 peptides containing reversibly modified cysteines, 9,723 peptides containing free cysteines, 1,716 intact sialylated N-linked glycopeptides and 771 lysine-acetylated peptides from the same biological samples. We further demonstrate the applicability of the workflow to multiple mouse tissues, highlighting its broad utility for integrated systems-level characterization of protein expression and PTM regulation across diverse biological models.

---

## 论文详细总结（自动生成）

# STEP-PTMs 论文总结

## 1. 核心问题与整体含义（研究动机和背景）

- **背景**：全面表征同一生物样本中的蛋白质丰度与多种翻译后修饰（PTM）对于理解细胞调控和 PTM 串扰至关重要，但在分析上仍具有很大挑战。
- **核心问题**：现有方法难以从同一样本中同时富集和分析多种 PTM 以及全局蛋白质组，通常需要分开处理，导致技术变异大、样本消耗多，并且不利于跨 PTM 数据的定量整合。
- **整体含义**：该论文提出了一种名为 **STEP-PTM**（Sequential Tag-based Enrichment of Post-Translational Modifications）的模块化 TMT 多重定量工作流，能够从单一肽段制备中同时定量蛋白质组、代谢组和多种 PTM 类别，为系统级蛋白质调控和 PTM 串扰研究提供了集成化解决方案。

## 2. 方法论：核心思想与关键技术细节

- **核心思想**：采用 TMT（串联质量标签）等量标记后，将所有肽段合并为一个多重肽段池，再依次执行多种 PTM 富集，从而最小化技术变异、减少样本需求，并支持跨数据集的直接定量整合。
- **主要流程**（文字描述）：
  1. 蛋白质酶解为肽段；
  2. 使用 TMT 进行等量标记，并将标记后的肽段合并为单一多重肽段池；
  3. 对肽段池顺序执行多种 PTM 富集模块；
  4. 保留未修饰肽段用于全局蛋白质组分析；
  5. 对各类 PTM 富集产物进行质谱检测，并使用 PTM 特异性数据库搜索以提高鉴定置信度和定量准确性。
- **支持的 PTM 富集模块**：
  - 磷酸化肽段；
  - 含游离半胱氨酸的肽段；
  - 含可逆修饰半胱氨酸的肽段；
  - 唾液酸化 N-连接糖肽；
  - 赖氨酸乙酰化肽段；
  - S-棕榈酰化肽段。
- **模块化特点**：可根据具体生物学问题灵活添加或省略相应富集模块，便于适应不同研究场景。

## 3. 实验设计：数据集、场景与对比方法

- **主要应用场景**：将 STEP-PTM 应用于 **TMT16-plex 脑类器官**样本，实现了多组学和多 PTM 的同时定量。
- **定量覆盖结果**（来自同一生物样本）：
  - 10,413 种蛋白质；
  - 2,969 种代谢物；
  - 19,655 条磷酸化肽段；
  - 28,876 条含可逆修饰半胱氨酸的肽段；
  - 9,723 条含游离半胱氨酸的肽段；
  - 1,716 条完整唾液酸化 N-连接糖肽；
  - 771 条赖氨酸乙酰化肽段。
- **普适性验证**：在多种小鼠组织中进一步展示了该工作流程的适用性。
- **Benchmark 与对比方法**：论文摘要中 **未提及** 与现有 PTM 富集工作流的系统比较，也没有明确的基准数据集。因此目前仅能评估其自身的能力展示，无法从摘要判断相对优势。
- **没有提到消融实验**：未说明是否对不同富集模块的组合、顺序或效率进行了对照实验。

## 4. 资源与算力

- **未明确说明**：提供的摘要和元数据中 **没有提及** GPU 型号、数量、训练时长或大规模计算资源信息。
- 由于该工作流属于质谱为主的生化湿实验流程，可能不涉及大规模深度学习训练，但文本未给出任何算力相关描述。

## 5. 实验数量与充分性

- **实验数量**：
  - 一项主要应用实验：TMT16-plex 脑类器官；
  - 一项适用性展示：多种小鼠组织；
  - 未描述消融实验、重复次数、不同条件对比等。
- **充分性评估**：
  - 从摘要层面看，实验证明了工作流的可行性和跨组织适用性，但 **缺乏与已有方法的直接对比**；
  - **未报告重复实验数量和统计显著性**，也没有关于定量变异性的详细分析；
  - 因此，实验设计的 **完整性、客观性和公平性需要阅读全文进一步评估**。

## 6. 主要结论与发现

- STEP-PTM 能够从单一生物样本中同时定量蛋白质组、代谢组和多种 PTM，显著提高组学信息整合能力。
- 该工作流减少了技术变异、降低了样本需求量，并支持跨数据集的定量整合。
- 在脑类器官中实现了大规模多 PTM 定量，并在小鼠组织中验证了其跨组织普适性。
- 作者认为该方法为系统解析蛋白质表达与 PTM 调控提供了一个 **可扩展的通用平台**。

## 7. 优点

- **高度集成**：同一份肽段制备可获得蛋白质组、代谢组和多种 PTM 信息，避免重复样本处理。
- **减少技术变异**：TMT 标记后合并为单一肽段池，便于不同富集模块间的定量比较和 PTM 串扰分析。
- **模块化设计**：可灵活调整富集模块，适应不同生物学问题，具有良好的扩展性。
- **不浪费未修饰肽段**：保留用于全局蛋白质组分析，提高样本利用率。
- **PTM 特异性数据库搜索**：有效提升鉴定的置信度和定量准确性。

## 8. 不足与局限

- **信息来源受限**：目前仅有摘要层面信息，缺乏详细实验参数、重复次数、统计检验和误差分析。
- **缺乏基准对比**：未与现有 PTM 富集流程（如独立富集或商业化试剂盒）进行直接比较，难以定量评估其相对优势和劣势。
- **未涉及生物学验证**：摘要中仅展示定量覆盖面，未展示 PTM 串扰或关键修饰位点的功能验证。
- **未说明检测灵敏度与动态范围**：对低丰度 PTM、稀有修饰或极端动态范围样本的适用性尚不清楚。
- **未披露资源消耗**：总实验时间、成本、所需样本量下限等实际应用信息缺失。
- **普适性证据有限**：仅提及“多种小鼠组织”和脑类器官，未给出具体组织类型、样本量及物种差异分析。

（完）
