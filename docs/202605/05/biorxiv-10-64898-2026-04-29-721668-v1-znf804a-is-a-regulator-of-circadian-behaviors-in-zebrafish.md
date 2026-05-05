---
title: Znf804a is a regulator of circadian behaviors in zebrafish
title_zh: Znf804a 是斑马鱼昼夜节律行为的调节因子
authors: "Bastien, B. L., Li, E. H., Capps, M. E. S., Thyme, S."
date: 2026-05-03
pdf: "https://www.biorxiv.org/content/10.64898/2026.04.29.721668v1.full.pdf"
tags: ["query:slp-ns"]
score: 9.0
evidence: 昼夜节律行为和睡眠障碍的调节因子
tldr: 本研究探讨了精神分裂症相关基因znf804a对斑马鱼睡眠和昼夜节律的影响。通过行为追踪和转录组测序，发现znf804a突变体会导致光照缺失下的节律行为异常，并识别出fbxl3a等核心节律调节因子的表达变化，揭示了该基因通过调节转录处理影响昼夜节律的潜在机制，为理解精神分裂症相关的睡眠障碍提供了新视角。
source: biorxiv
selection_source: fresh_fetch
motivation: 旨在探究精神分裂症风险基因znf804a如何通过调控分子通路影响睡眠和昼夜节律。
method: 利用斑马鱼突变体进行多日行为追踪，并结合不同光照条件下的转录组测序分析基因表达差异。
result: 发现znf804a缺失会导致昼夜节律行为改变，并引起fbxl3a等核心时钟调节基因的表达下调及转录本丰度变化。
conclusion: 研究证实了znf804a是昼夜节律行为的关键调节因子，为理解精神分裂症相关的睡眠障碍提供了分子机制参考。
---

## 摘要
睡眠障碍在精神分裂症患者中很常见，并可能加剧学习和记忆等认知过程的紊乱。阐明受精神分裂症基因干扰且具有药物靶向潜力的分子通路，可能为治疗开辟新途径。在本研究中，我们探讨了精神分裂症相关基因 znf804a 与睡眠及昼夜节律通路之间的关系。通过多日的行为追踪，我们发现 znf804a 斑马鱼突变体在移除光照信号后表现出睡眠和昼夜节律行为的改变。通过对在正常光循环和全黑条件下生长的鱼进行大体 RNA 测序（bulk RNA sequencing），我们发现控制昼夜节律的核心及辅助通路中的基因表达发生了改变。fbxl3a 编码生物钟核心负反馈调节因子的调制器，其表达量随着 znf804a 突变拷贝数的增加而呈剂量依赖性下降。进一步分析还揭示了特定转录本（包括 idh1）相对丰度的变化，表明 znf804a 可能影响转录本的加工或稳定性。总之，这些发现将 ZNF804A 的同源基因与睡眠及昼夜节律行为联系起来，并确定了 fbxl3a 的调节和转录本加工是该精神分裂症风险基因影响昼夜节律生物学的候选机制。

## Abstract
Sleep disturbances are common among individuals with schizophrenia and can exacerbate disruptions in cognitive processes like learning and memory. Elucidating pharmacologically targetable molecular pathways perturbed by schizophrenia genes may uncover new treatment avenues. Here, we investigated the relationship of the schizophrenia-associated gene znf804a with sleep and circadian pathways. Using multi-day behavior tracking, we showed that znf804a zebrafish mutants displayed changes in sleep and circadian behaviors when light cues were removed. Through bulk RNA sequencing of fish raised under normal light cycling and dark-only conditions, we identified altered gene expression in the core and auxiliary pathways controlling circadian rhythms. Expression of fbxl3a, which encodes a modulator of the core negative feedback regulator of the clock, decreased in a dose-dependent manner as znf804a mutant copy number increased. Further analysis also revealed shifts in the relative abundance of specific transcripts, including idh1, suggesting znf804a could influence transcript processing or stability. Together, these findings link a ZNF804A ortholog to sleep and circadian behaviors and identify the regulation of fbxl3a and transcript processing as candidate mechanisms through which this schizophrenia risk gene may influence circadian biology.

---

## 论文详细总结（自动生成）

这篇论文研究了精神分裂症（SCZ）高风险基因 *ZNF804A* 在调节昼夜节律和睡眠中的作用。以下是对该论文的深度结构化总结：

### 1. 核心问题与整体含义（研究动机和背景）
*   **核心问题**：探讨精神分裂症风险基因 *ZNF804A* 如何影响睡眠和昼夜节律。
*   **背景**：睡眠障碍是精神分裂症患者的常见症状，会加剧认知功能障碍。虽然 *ZNF804A* 在全基因组关联分析（GWAS）中被确定为顶级风险基因，且与人类睡眠神经生理学有关，但其在模型生物中的具体分子机制和对昼夜节律的调控作用此前尚不明确。

### 2. 方法论
*   **核心思想**：利用斑马鱼作为模型生物，通过基因敲除（突变体）和瞬时敲除（Crispants）技术，结合行为学追踪和高通量转录组测序，建立基因-行为-分子通路之间的联系。
*   **关键技术细节**：
    *   **行为追踪**：使用 96 孔板行为分析系统，配合红外灯和相机，利用 LabVIEW 软件实时记录 4-6 天龄（dpf）幼鱼在不同光照条件下的活动。
    *   **转录组分析（RNA-seq）**：对正常光照（LD）和全黑（DD）环境下的幼鱼头部进行大体 RNA 测序，使用 STAR 比对和 DESeq2 进行差异表达分析。
    *   **转录本水平分析**：采用 Lawson Lab 的斑马鱼转录组注释，分析特定基因的不同异构体（Isoforms）丰度变化，以探究其在 RNA 加工中的作用。
    *   **验证实验**：通过 CRISPR/Cas9 靶向 *znf804a* 的编码区或调节区产生 Crispants，并利用 RT-qPCR 验证关键下游基因（如 *fbxl3a*）的表达。

### 3. 实验设计
*   **实验场景/条件**：
    1.  **正常光循环（14h亮/10h暗）**：观察基础节律。
    2.  **全黑环境（DD）**：移除外部光信号，观察内源性节律漂移。
    3.  **全亮环境（LL）**：观察持续光照下的活动。
    4.  **光照偏移（Light Shift）**：将光照时间提前，测试突变体对环境变化的补偿能力。
*   **对照组（Benchmark）**：野生型（WT）同胞幼鱼。
*   **对比方法**：对比了纯合突变体（-/-）、杂合子（+/-）和野生型（+/+）在不同光照压力下的表现。

### 4. 资源与算力
*   **测序平台**：使用了 Illumina NovaSeq 6000 进行高通量测序。
*   **算力说明**：文中未详细列出具体的 GPU 型号或训练时长（此类生物信息学分析通常依赖 CPU 集群进行比对和统计运算，而非深度学习所需的 GPU 算力）。

### 5. 实验数量与充分性
*   **实验规模**：
    *   行为实验重复了多次，并在五个世代后的独立群体中得到了验证（如 Figure S2）。
    *   RNA-seq 每个条件包含 4 个生物学重复，每个重复由 4 条幼鱼头部混合而成。
    *   GO 富集分析涵盖了多个生物学过程。
*   **充分性评价**：实验设计较为充分，包含了行为学表型、分子机制探索及独立验证（CRISPR 验证），逻辑链条完整。通过不同光照条件的切换，客观地揭示了突变体在失去外部信号时的缺陷。

### 6. 主要结论与发现
*   **行为层面**：*znf804a* 突变体在全黑环境下表现出明显的**昼夜节律漂移**和总体活动量减少；在光照偏移实验中，突变体补偿环境变化的速度较慢。
*   **分子层面**：
    *   识别出 *znf804a* 缺失会导致核心节律基因（如 *per1a*, *cry1bb*, *arntl1a*）和辅助通路基因（*nr1d1*, *rorcb*）失调。
    *   **关键发现**：*fbxl3a*（调节 CRY 蛋白稳定性的关键因子）的表达量随 *znf804a* 突变拷贝数增加呈**剂量依赖性下降**。
    *   **转录加工**：发现 *znf804a* 影响特定基因（如 *idh1*, *caska*, *ctnnd2b*）的转录本丰度转换，支持了其参与 RNA 剪接或稳定性调节的假设。

### 7. 优点
*   **首次关联**：首次在模型生物中证实了 *ZNF804A* 同源基因与昼夜节律行为的直接联系。
*   **多维度分析**：结合了宏观行为表型与微观转录本异构体分析，提供了较深入的机制解释。
*   **剂量效应**：明确展示了基因缺失程度与表型/分子变化之间的线性关系，增强了结论的可信度。

### 8. 不足与局限
*   **生化机制尚不明确**：虽然推测 Znf804a 参与 RNA 加工，但其作为锌指蛋白是直接结合 DNA 还是 RNA，以及其具体的蛋白质结构仍未完全阐明。
*   **细胞异质性**：使用的是大体（Bulk）RNA-seq，可能掩盖了特定脑区或细胞类型（如视交叉上核同源区域）中的微小但关键的表达变化。
*   **物种差异**：斑马鱼幼鱼的睡眠模式与人类成人精神分裂症患者的睡眠结构存在差异，转化医学价值需进一步验证。

（完）
