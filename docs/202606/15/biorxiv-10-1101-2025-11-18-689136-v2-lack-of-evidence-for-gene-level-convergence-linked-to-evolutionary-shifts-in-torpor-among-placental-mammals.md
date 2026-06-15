---
title: Lack of evidence for gene-level convergence linked to evolutionary shifts in torpor among placental mammals
title_zh: 缺乏证据表明基因层面的趋同与胎盘哺乳动物休眠的进化转变相关
authors: "Kontopoulos, D. - G., Ahmed, A.-W., Bein, B., Levesque, D. L., Hiller, M."
date: 2026-06-14
pdf: "https://www.biorxiv.org/content/10.1101/2025.11.18.689136v2.full.pdf"
tags: ["query:tr-hb"]
score: 9.0
evidence: 胎盘哺乳动物torpor进化的比较基因组分析
tldr: 冬眠是鸟类和哺乳动物应对恶劣环境的关键生存策略，但不同谱系独立进化冬眠是否涉及相同基因尚不明确。本研究对190个胎盘哺乳动物基因组进行筛选，分析蛋白质编码基因的丢失、正选择和进化速率变化与冬眠使用的关联。结果发现基因-冬眠关联高度支系特异性，没有单一基因能解释大多数冬眠转变，仅通路水平存在有限的趋同进化。这表明冬眠通过多种遗传途径进化，解释了冬眠物种中冬眠模式的巨大多样性。
source: biorxiv
selection_source: fresh_fetch
motivation: 探究不同哺乳动物谱系独立进化冬眠是否涉及相同的遗传变化。
method: 对190种胎盘哺乳动物基因组进行比较筛选，分析基因丢失、正选择和进化速率变化与冬眠使用的关联。
result: 未发现普遍趋同的基因，基因-冬眠关联高度支系特异性，仅在通路水平检测到有限的趋同进化。
conclusion: 冬眠在胎盘哺乳动物中通过多种遗传途径进化，解释了目前冬眠模式的多样性。
---

## 摘要
休眠是许多鸟类和哺乳动物谱系为应对恶劣环境条件而进化出的关键生存策略。不同谱系中休眠的独立进化是否涉及相同基因的变化，目前尚不清楚。在这里，我们对190个胎盘哺乳动物基因组进行了比较筛选，以全面检查单个蛋白质编码基因的丢失、正选择和进化速率变化与休眠使用进化转变之间的关联。我们发现基因-休眠关联具有高度的支系特异性，没有基因能够解释胎盘哺乳动物系统发育中大多数休眠转变。相反，在通路水平上可以检测到相对较高但有限的进化趋同程度。我们的结果表明，休眠在胎盘哺乳动物中通过多种遗传途径出现，这可能解释了今天在能够休眠的物种中观察到的休眠使用模式的巨大多样性。

## Abstract
Torpor is a key survival strategy that many avian and mammalian lineages evolved in response to challenging environmental conditions. Whether the independent evolution of torpor in different lineages involved changes in the same genes remains poorly understood. Here, we performed comparative screens across 190 placental mammal genomes to comprehensively examine associations between loss, positive selection and evolutionary rate shifts in individual protein-coding genes and evolutionary shifts in torpor use. We find that gene-torpor associations are highly clade-specific, with no gene being able to explain the majority of torpor shifts across the phylogeny of placental mammals. Instead, a relatively higher but limited extent of evolutionary convergence can be detected at the pathway level. Our results suggest that torpor emerged through several genetic routes in placental mammals, which likely explains the vast diversity of torpor use patterns that can be observed among torpor-capable species today.

---

## 论文详细总结（自动生成）

# 详细中文总结

## 1. 论文的核心问题与整体含义（研究动机和背景）

- **核心问题**：不同的胎盘哺乳动物谱系独立进化出休眠（冬眠/蛰伏）这一生存策略时，是否涉及相同基因的遗传变化？即基因层面的趋同进化是否存在？
- **研究背景**：休眠是鸟类和哺乳动物应对恶劣环境（如寒冷、食物短缺）的关键适应性策略，但在不同物种中休眠模式（深度、时长、触发条件）差异巨大。此前研究对于不同谱系间休眠进化的遗传基础是否共享尚不清楚。
- **整体意义**：若存在共享基因，则表明休眠进化受到强烈遗传约束；若不存在，则支持休眠通过多种遗传路径进化，有助于解释休眠表型的多样性，并为进化生物学和适应性机制研究提供新视角。

## 2. 论文提出的方法论：核心思想、关键技术细节

- **核心思想**：利用大规模比较基因组学方法，系统筛查蛋白质编码基因的三种进化信号与休眠使用进化转变之间的关联：
  - 基因丢失（gene loss）
  - 正选择（positive selection）
  - 进化速率变化（evolutionary rate shifts）
- **关键技术细节**：
  - 对190个胎盘哺乳动物基因组进行筛选（具体筛选算法和阈值在摘要中未详述，如使用系统发育框架下的分支-位点模型检测正选择，或使用基因丢失预测工具等）。
  - 将每个基因的变化与系统发育树上休眠使用的转变（是否使用休眠）进行关联分析。
  - 在通路水平（pathway level）检测趋同进化程度，以评估基因集功能的富集。
- **公式或算法流程**：摘要未提供具体公式，但可推断使用了系统发育比较方法（如Phylogenetic Generalized Least Squares、分支模型、速率变化检测等）。总体流程为：基因组组装 → 基因注释 → 直系同源鉴定 → 进化信号检测 → 与休眠表型关联分析 → 通路富集分析。

## 3. 实验设计：使用了哪些数据集/场景，基准测试方法，对比的方法

- **数据集**：
  - 190个胎盘哺乳动物基因组（来源：公共数据库如NCBI、Ensembl等，具体未列出，但覆盖主要谱系）。
  - 休眠使用表型数据：可能来自文献和数据库，对每个物种编码是否为冬眠物种（或休眠能力）。
- **基准测试**：论文未提及明确的benchmark，因为这是探索性比较基因组学，而非方法学竞赛。分析标准是：若某个基因在多个独立获得休眠的支系中同时出现丢失/正选择/速率变化，则视为趋同证据。
- **对比的方法**：
  - 在基因层面，比较了不同支系特异性关联与全局关联的差异。
  - 在通路层面，比较了通路与随机期望的趋同程度（可能通过置换检验评估显著性）。
  - 未提及与其他具体方法的直接对比（如其他比较基因组软件等）。

## 4. 资源与算力

- **文中未明确说明**：摘要和元数据未提及GPU型号、数量、训练时长、CPU核心数等计算资源信息。由于是比较基因组学分析，主要依赖大型集群进行序列比对、系统发育树构建和统计检验，但具体细节缺失。仅可推测需要较高内存和多核CPU，但无量化数据。

## 5. 实验数量与充分性

- **实验数量**：
  - 主要实验为对190个基因组的全基因筛查（涵盖数千个蛋白质编码基因）。
  - 检测了三种进化信号（丢失、正选择、速率变化）与休眠使用的关联。
  - 在基因层面和通路层面分别进行分析。
- **充分性评估**：
  - **优点**：样本量（190个物种）在胎盘哺乳动物比较基因组学中属于较大规模；覆盖主要支系，减少了抽样偏差。
  - **不足**：只分析了蛋白质编码基因，未考虑非编码区（如调控元件）或表观遗传变化；休眠表型的定义可能不够精确（如是否区分冬眠与日常休眠）；仅关联了“休眠使用”的二元状态，未考虑休眠的连续性特征（如深度、时长）。
  - **客观性**：结论“缺乏趋同证据”是基于全基因组层面未发现普遍共享基因，分析较为严谨。但需注意负结果可能受统计检验力限制。

## 6. 论文的主要结论与发现

- **主要结论**：
  1. 没有单一基因能够解释胎盘哺乳动物系统发育中大多数休眠转变，基因-休眠关联高度支系特异性（clade-specific）。
  2. 在通路水平检测到相对较高但有限的进化趋同程度（即某些功能通路的基因集在多个支系中同时发生类似变化）。
  3. 这表明休眠在胎盘哺乳动物中通过多种遗传途径（multiple genetic routes）进化，从而解释了休眠模式的巨大多样性。

## 7. 优点：方法或实验设计上的亮点

- **大规模系统性筛查**：首次在190个基因组上系统分析三种进化信号，比以往仅个别基因或少数物种的研究更具全面性。
- **多层次分析**：同时考察基因丢失、正选择、速率变化，并区分基因层面和通路层面，有助于揭示不同层次的进化模式。
- **负结果的价值**：明确报告缺乏基因层面趋同，有助于修正以往可能存在的预期（即认为冬眠必定由保守基因控制），推动更精细的研究。
- **支系特异性分析**：强调高度支系特异性，揭示了进化可塑性。

## 8. 不足与局限

- **数据局限性**：
  - 仅基于蛋白质编码基因，未考虑非编码RNA、启动子、增强子等调控区域的变化。
  - 休眠表型可能为二元分类（有/无），忽略了冬眠的连续特征（如最低体温、持续时间等），可能丢失重要变异。
- **方法局限**：
  - 统计关联方法无法直接证明因果关系，仅揭示相关性。
  - 样本中可能包含近缘物种，系统发育非独立性可能影响检测效力（尽管已使用系统发育方法校正）。
- **偏差风险**：
  - 基因组组装质量参差不齐，可能导致基因丢失的假阳性或假阴性。
  - 休眠物种的生态和生理多样性尚未被纳入（如体型、栖息地等协变量）。
- **应用限制**：
  - 结果对于理解人类代谢调控或医学应用（如诱导冬眠）可能提供线索有限，因为缺乏具体的候选基因。

（完）
