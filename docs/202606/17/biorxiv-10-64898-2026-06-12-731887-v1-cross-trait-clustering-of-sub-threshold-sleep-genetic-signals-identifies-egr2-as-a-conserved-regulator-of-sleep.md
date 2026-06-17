---
title: Cross-trait clustering of sub-threshold sleep genetic signals identifies EGR2 as a conserved regulator of sleep
title_zh: 跨性状聚类亚阈值睡眠遗传信号识别EGR2为进化保守的睡眠调节因子
authors: "Mace, K. D., Trang, K. B., Zimmerman, A. J., Almeraya del Valle, E., Lottes, E. N., Parker, R. E., Choudhury, J., Chesi, A., Grant, S. F., Kayser, M. S."
date: 2026-06-16
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.12.731887v1.full.pdf"
tags: ["query:slp-ns"]
score: 9.0
evidence: 多性状聚类睡眠遗传信号鉴定EGR2为保守睡眠调节因子
tldr: 特发性嗜睡症遗传信号有限，本研究对亚阈值睡眠遗传变异进行多性状聚类，结合细胞类型特异变异到基因映射筛选候选基因。在果蝇和斑马鱼中验证EGR2（果蝇stripe）敲低延长睡眠，揭示EGR2为保守的睡眠调控因子。方法可推广至其他复杂性状。
source: biorxiv
selection_source: fresh_fetch
motivation: 受限于全基因组显著位点数量，亚阈值遗传信号中可能存在未知的睡眠调控基因。
method: 多性状聚类分析亚阈值遗传变异，结合细胞类型特异映射鉴定候选基因，跨物种功能验证。
result: EGR2在果蝇神经元中敲低增加睡眠时长和巩固度，斑马鱼突变体同样睡眠增多。
conclusion: EGR2是跨物种保守的睡眠调控因子，亚阈值遗传信号可用于发现新基因。
---

## 摘要
特发性嗜睡症是一种高度遗传的睡眠障碍，特征为白天过度嗜睡，但至今只鉴定出少数与嗜睡相关的遗传通路。为了在有限的与嗜睡相关性状的全基因组显著位点之外扩展遗传发现，我们对未达到常规显著性阈值的睡眠相关遗传变异应用了多性状聚类。结合我们的细胞类型特异性变异-基因映射，优先筛选了用于跨物种功能检测的候选效应基因。其中最有力的候选基因之一是EGR2，它作为神经元中ADO-EGR2位点的一个远端效应基因出现。果蝇EGR2同源基因stripe的神经元敲低增加了睡眠时长和睡眠巩固，而斑马鱼egr2同源基因的突变同样增加了睡眠。总之，这些发现表明，可以从低于常规显著性阈值的遗传信号中识别睡眠调控通路，并确立EGR2为跨物种保守的睡眠调节因子。

## Abstract
Idiopathic hypersomnia (IH) is a highly heritable sleep disorder characterized by excessive daytime sleepiness, yet few genetic pathways contributing to hypersomnolence have been identified. To expand genetic discovery beyond the limited number of genome-wide significant loci associated with sleepiness-related traits, we applied multi-trait clustering to sleep-associated genetic variation that did not reach conventional significance thresholds. Integration with our cell-type-specific variant-to-gene mapping prioritized candidate effector genes for cross-species functional screening. Among the strongest candidates was EGR2, which emerged as a distal effector gene at the ADO-EGR2 locus in neurons. Neuronal knockdown of the Drosophila EGR2 ortholog stripe increased sleep duration and sleep consolidation, while mutation of zebrafish egr2 orthologs similarly increased sleep. Together, these findings demonstrate that sleep-regulatory pathways can be identified from genetic signals below conventional significance thresholds and establish EGR2 as a conserved regulator of sleep across species.

---

## 论文详细总结（自动生成）

# 论文详细总结

## 1. 论文的核心问题与整体含义（研究动机和背景）

特发性嗜睡症（IH）是一种高度遗传的睡眠障碍，主要表现为白天过度嗜睡，但其遗传机制至今仍不明确。已有的大型GWAS仅发现了少数与嗜睡相关性状（如日间小睡、嗜睡、睡眠时长）的全基因组显著位点，而IH本身的GWAS（仅414例）未发现任何显著位点。这意味着绝大多数与嗜睡相关的遗传信号可能低于常规显著性阈值（P ≤ 5×10⁻⁸），成为“亚阈值”信号。然而，这些信号可能蕴含生物学意义，而非单纯噪声。

本研究旨在通过跨性状聚类方法，系统性地挖掘亚阈值睡眠遗传变异中的共享模式，结合细胞类型特异性的变异-基因（V2G）映射和跨物种功能验证，鉴定新的睡眠调控基因。该方法有望克服GWAS效力不足的问题，发现保守的睡眠调控通路。

## 2. 论文提出的方法论：核心思想、关键技术细节

### 核心思想
- **多性状聚类**：利用贝叶斯非负矩阵分解（bNMF）对亚阈值GWAS变异进行聚类，识别具有相似跨表型关联模式的变异群体，从而提取出可能代表共同生物学通路的信号。
- **细胞类型特异性V2G映射**：将聚类得到的变异与人类神经细胞的染色质开放区域和三维染色质相互作用数据结合，定位到候选效应基因。
- **跨物种功能验证**：在果蝇（RNAi）和斑马鱼（CRISPR）中进行反向遗传筛选，验证候选基因对睡眠行为的影响。

### 关键技术细节
1. **变异选择与LD剪枝**：
   - 从三个大型UK Biobank GWAS（日间小睡、日间嗜睡、睡眠时长）中提取P ≤ 5×10⁻⁶的变异，共初始筛选数千个位点。
   - 进行LD剪枝（r² < 0.05，EUR参考群体），最终保留4,254个独立变异。

2. **特征矩阵构建**：
   - 对每个变异，提取在18个睡眠表型（9个自报告、8个加速度计、1个OSA）中的关联z-score，并缩放去偏。
   - 将z-score矩阵扩展为双列非负矩阵（正、负值分别表示）。

3. **bNMF聚类**：
   - 使用BayesNMF.L2EU算法，设置K=20初始，运行1,000次，计算负对数证据。
   - 比较K=3~7，K=5在统计上最优，但K=4在生物学上更优（K=5的嗜睡信号分散，而K=4的Cluster 2更能集中捕获已知睡眠倾向位点，如CADM2，且V2G基因重迭度80.6%）。最终选择K=4。
   - 变异分配到Cluster：以95%分位数权重阈值确定。

4. **V2G映射**：
   - 使用iPSC衍生神经元、神经祖细胞（NPC）、星形胶质细胞的ATAC-seq和Capture-C/Hi-C数据定义顺式调控元件（cRE）。
   - 若变异位于cRE内，且该cRE通过染色质环连接到目标基因的启动子开放染色质区域（OCR），则将该基因列为候选。
   - 最终从Cluster 2的213个变异中定位到93个基因（53个蛋白编码基因）。

5. **果蝇RNAi筛选**：
   - 使用pan-neuronal（elav-GAL4）和pan-glial（repo-GAL4）驱动果蝇直系同源基因的RNAi。
   - 通过DAM系统测量睡眠时长、睡眠结构、活动指数等，并使用PCA和k-means聚类识别表型簇。

6. **斑马鱼验证**：
   - 针对egr2a和egr2b设计CRISPR gRNA，靶向保守功能域，制备双突变体（crispant）。
   - 自动化视频追踪测量白天/夜间睡眠和活动。

## 3. 实验设计：数据集、Benchmark与对比方法

### 数据集
- **GWAS数据**：
  - 日间小睡（N=452,633）
  - 日间嗜睡（N=452,071）
  - 睡眠时长（N=446,118）
  - 以上均来自UK Biobank。
- **额外表型**：18个睡眠相关表型（自报告、加速度计、OSA）。
- **染色质数据**：iPSC衍生神经元、NPC、星形胶质细胞的ATAC-seq和Capture-C/Hi-C（来自已发表数据集）。

### Benchmark
- **内部对照**：已知的6个“睡眠倾向”位点（包括之前验证的CADM2）均被Cluster 2的95%权重阈值捕获，证实聚类方法的有效性。
- **K=4 vs K=5比较**：虽然K=5统计最优，但K=4在生物学上更优：K=5分散了嗜睡信号，而K=4的Cluster 2基因集覆盖了K=5中80.6%的基因，并额外扩展了68个候选基因。

### 对比方法
论文未直接与其他聚类方法（如LDSC、pleiotropy analysis等）进行对比，而是侧重于自身方法链的验证和跨物种实验。主要对比是不同K值选择对结果的影响。

## 4. 资源与算力

论文**未明确说明**所使用的计算资源（如GPU型号、数量、训练时长等）。仅提及bNMF算法运行了1,000次（K=3~7各），但未提供具体的计算硬件或时间信息。此外，V2G映射和果蝇/斑马鱼行为分析也未涉及算力描述。

## 5. 实验数量与充分性

### 实验组数
- **bNMF聚类**：对K=3~7重复1,000次以评估稳定性。
- **V2G映射**：涵盖三种神经细胞类型，从213个变异鉴定93个候选基因。
- **果蝇RNAi筛选**：
  - 初始筛选：使用pan-neuronal和pan-glial驱动，每个基因至少2个独立RNAi系。
  - 详细表型分析：包括sleep architecture（长睡眠bout比例、pWake/pDoze）、睡眠稳态、昼夜节律、空间筛选（8种GAL4驱动）。
  - 针对stripe/EGR2：3个独立RNAi系验证。
- **斑马鱼实验**：两个生物学重复（不同clutch），共65个crispant和96个阴性对照。

### 充分性与客观性
- **充分**：多层次的验证（聚类→V2G→功能筛选→详细表型→空间定位→脊椎动物验证），覆盖了从人类遗传学到行为学的完整链路。
- **客观**：内部阳性对照（CADM2）；多重独立RNAi系排除脱靶；果蝇实验中通过PCA和k-means聚类无偏识别表型簇；斑马鱼中排除了形态异常个体，并检测了潜在运动/癫痫效应。
- **公平**：对比K=4和K=5的结果，并解释了选择依据；基因组注释未依赖最近基因原则，而是采用染色质构象数据，避免偏差。

## 6. 论文的主要结论与发现

- **多性状聚类可有效提取亚阈值遗传信号**：从~4,254个亚阈值变异中鉴定出Cluster 2，其关联模式（白天嗜睡、日间小睡、自我报告长睡眠、加速度计白天不活动）与嗜睡倾向一致，并恢复了已知睡眠位点（CADM2）。
- **EGR2/stripe是跨物种保守的睡眠调节因子**：
  - 果蝇中，神经元stripe RNAi敲低显著增加睡眠时长、睡眠巩固度（长bout增加、sleep-to-wake转换概率降低），且不影响运动活动、昼夜节律和睡眠稳态。
  - 斑马鱼中，egr2ab双突变增加白天睡眠约1.5小时，增加睡眠bout数量和长度。
- **嗅觉神经元是stripe调控睡眠的关键细胞位置**：利用orco-GAL4和peb-GAL4在嗅觉神经元中敲低stripe，可复现全神经元的嗜睡表型，而其他多数神经亚群未产生明显表型。
- **ADO-E GR2位点中EGR2为效应基因**：变异rs10995311位于ADO外显子区内，但通过染色质环与EGR2启动子互作；预测的ADO错义变异（Pro39Ala）被多个工具评为良性；果蝇中敲低ADO同源基因CG7550未改变睡眠，而stripe敲低表型显著。

## 7. 优点

- **方法创新**：首次将bNMF应用于亚阈值睡眠GWAS信号，从“噪声”中提取生物学信号，为研究其他高度多基因的复杂性状提供了范式。
- **全面整合**：将人类遗传学、表观基因组学、细胞类型特异性染色质构象、跨物种功能验证有机结合，形成了从变异到行为机制的完整通路。
- **内部参照验证**：成功捕获已知的嗜睡效应基因CADM2，增强了方法可信度和结论可靠性。
- **实验设计严谨**：使用多个独立RNAi系、PCA无偏聚类、空间特异性筛选、斑马鱼双基因敲除、形态学及行为异常排除等，减少假阳性和混淆因素。
- **跨物种保守性证据强**：果蝇和斑马鱼均一致显示EGR2敲低/突变导致睡眠增多，暗示其在进化中保守的睡眠调控功能。

## 8. 不足与局限

- **亚阈值信号噪声问题**：尽管聚类方法可富集信号，但亚阈值变异本身含有大量虚假关联，仍然可能存在假阳性。
- **表型特异性有限**：Cluster 2反映的是“嗜睡倾向”而非特发性嗜睡症的特异性，因为大规模GWAS数据主要来自一般人群，而非临床IH患者。
- **V2G映射的分辨率限制**：染色质相互作用数据来自体外分化细胞（iPSC神经元、NPC、星形胶质细胞），可能未完全反映体内真实调控环境；部分互作在NPC和星形胶质细胞中仅接近阈值，不排除技术误差。
- **RNAi潜在脱靶**：虽然使用了多个独立RNAi系，但整体筛选中的部分阳性结果仍可能源于脱靶效应（stripe为最强候选，且经多重验证）。
- **斑马鱼模型存在个体异常**：部分egr2ab crispants出现尾部弯曲、抽动等表型（类似癫痫），虽已排除这些个体，但提示EGR2可能参与神经系统发育或运动控制，可能间接贡献于睡眠表型。
- **算力与资源未报告**：缺乏计算细节，不利于可重复性评估。
- **应用限制**：该方法依赖于大型GWAS和高质量细胞类型染色质数据，对于缺乏此类资源的疾病/性状可能难以直接复制。

（完）
