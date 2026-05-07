---
title: Znf804a is a regulator of circadian behaviors in zebrafish
title_zh: Znf804a 是斑马鱼昼夜节律行为的调节因子
authors: "Bastien, B. L., Li, E. H., Capps, M. E. S., Thyme, S."
date: 2026-05-03
pdf: "https://www.biorxiv.org/content/10.64898/2026.04.29.721668v1.full.pdf"
tags: ["query:slp-ns"]
score: 9.0
evidence: 研究znf804a在睡眠和昼夜节律行为中的作用
tldr: 本研究探讨了精神分裂症风险基因znf804a在斑马鱼中的功能，发现该基因缺失会导致光照缺失环境下的睡眠和昼夜节律行为异常。通过转录组测序，研究揭示了znf804a通过调节核心生物钟调节因子fbxl3a的表达以及影响转录本处理过程，进而干预昼夜节律生物学，为理解精神分裂症相关的睡眠障碍提供了分子机制。
source: biorxiv
selection_source: fresh_fetch
motivation: 旨在探究精神分裂症相关基因znf804a如何影响睡眠和昼夜节律通路，以寻找潜在的治疗靶点。
method: 利用斑马鱼突变体进行多日行为追踪，并结合正常光照与全黑环境下的转录组测序分析基因表达变化。
result: znf804a突变体在无光照条件下表现出节律行为改变，且核心生物钟调节因子fbxl3a的表达随突变拷贝数增加而呈剂量依赖性下降。
conclusion: 研究证实了znf804a是昼夜节律行为的关键调节因子，其通过调控fbxl3a和转录本稳定性来影响生物钟功能。
---

## 摘要
睡眠障碍在精神分裂症患者中十分常见，并可能加剧学习和记忆等认知过程的紊乱。阐明受精神分裂症基因干扰且具有药理学靶向潜力的分子通路，可能为治疗开辟新途径。在本研究中，我们探讨了精神分裂症相关基因 znf804a 与睡眠及昼夜节律通路之间的关系。通过多日行为追踪，我们发现当光照线索被移除时，znf804a 斑马鱼突变体表现出睡眠和昼夜节律行为的变化。通过对在正常光循环和全黑条件下生长的鱼进行大体 RNA 测序，我们发现控制昼夜节律的核心和辅助通路中的基因表达发生了改变。fbxl3a 编码生物钟核心负反馈调节因子的调节蛋白，其表达量随着 znf804a 突变拷贝数的增加而呈剂量依赖性下降。进一步分析还揭示了包括 idh1 在内的特定转录本相对丰度的变化，表明 znf804a 可能影响转录本的处理或稳定性。总之，这些发现将 ZNF804A 的同源基因与睡眠及昼夜节律行为联系起来，并将 fbxl3a 的调节和转录本处理确定为该精神分裂症风险基因影响昼夜节律生物学的候选机制。

## Abstract
Sleep disturbances are common among individuals with schizophrenia and can exacerbate disruptions in cognitive processes like learning and memory. Elucidating pharmacologically targetable molecular pathways perturbed by schizophrenia genes may uncover new treatment avenues. Here, we investigated the relationship of the schizophrenia-associated gene znf804a with sleep and circadian pathways. Using multi-day behavior tracking, we showed that znf804a zebrafish mutants displayed changes in sleep and circadian behaviors when light cues were removed. Through bulk RNA sequencing of fish raised under normal light cycling and dark-only conditions, we identified altered gene expression in the core and auxiliary pathways controlling circadian rhythms. Expression of fbxl3a, which encodes a modulator of the core negative feedback regulator of the clock, decreased in a dose-dependent manner as znf804a mutant copy number increased. Further analysis also revealed shifts in the relative abundance of specific transcripts, including idh1, suggesting znf804a could influence transcript processing or stability. Together, these findings link a ZNF804A ortholog to sleep and circadian behaviors and identify the regulation of fbxl3a and transcript processing as candidate mechanisms through which this schizophrenia risk gene may influence circadian biology.

---

## 论文详细总结（自动生成）

这是一份关于论文《Znf804a 是斑马鱼昼夜节律行为的调节因子》（*Znf804a is a regulator of circadian behaviors in zebrafish*）的结构化深入总结：

### 1. 论文的核心问题与整体含义（研究动机和背景）
*   **核心问题**：探讨精神分裂症（Schizophrenia, SZ）的关键风险基因 *ZNF804A* 如何影响睡眠和昼夜节律行为，并寻找其背后的分子调控机制。
*   **研究背景**：睡眠障碍是精神分裂症患者的常见症状，且会加剧认知功能障碍。虽然 *ZNF804A* 是首个通过全基因组关联分析（GWAS）确定的 SZ 风险基因，但其在调节生物钟和睡眠方面的具体生物学功能尚不清楚。

### 2. 论文提出的方法论
*   **核心思想**：利用斑马鱼作为脊椎动物模型，通过基因敲除观察其在不同光照环境下的行为变化，并结合转录组学分析定位受影响的分子通路。
*   **关键技术细节**：
    *   **基因编辑**：使用 CRISPR/Cas9 技术产生 *znf804a* 基因突变体。
    *   **行为追踪**：利用自动化行为监测系统，在受精后 4-7 天（dpf）的幼鱼中记录活动量和睡眠参数。
    *   **环境干预**：设置正常光循环（LD, 14h光照/10h黑暗）和恒定黑暗（DD）两种环境，以区分光驱动行为与内源性昼夜节律。
    *   **转录组分析**：对不同基因型和环境下的幼鱼进行 Bulk RNA-seq，使用 DESeq2 进行差异表达分析，并利用特定算法评估转录本异构体（Isoform）的相对丰度。

### 3. 实验设计
*   **实验场景**：实验室受控环境下的斑马鱼幼鱼行为实验。
*   **Benchmark/对照**：以野生型（WT）斑马鱼为基准，对比杂合子（Het）和纯合突变体（Mut）的表现。
*   **对比方法**：
    *   **行为对比**：LD 环境（外部线索存在）vs DD 环境（依赖内源生物钟）。
    *   **分子对比**：不同基因型间的基因表达差异，以及不同光照条件对基因表达的影响。

### 4. 资源与算力
*   **算力说明**：论文中未明确提及具体的 GPU 型号或大规模计算集群。
*   **资源消耗**：主要涉及标准的生物信息学处理流程（如序列比对、差异表达统计），这类任务通常在常规的高性能计算（HPC）服务器上完成，不涉及深度学习模型的大规模训练。

### 5. 实验数量与充分性
*   **实验规模**：
    *   **行为学**：进行了多批次独立重复实验，每组样本量（N值）通常在数十条鱼，确保了统计学意义。
    *   **转录组**：涵盖了 3 种基因型（WT, Het, Mut）和 2 种环境（LD, DD）的组合，样本覆盖全面。
*   **充分性评价**：实验设计较为充分。通过 DD 环境下的行为观察，有力地证明了 *znf804a* 对内源节律的调节作用，而非仅仅是对光线的反应。

### 6. 论文的主要结论与发现
*   **行为层面**：在恒定黑暗（DD）环境下，*znf804a* 突变体表现出明显的睡眠减少和活动节律改变，证明该基因是昼夜节律行为的关键调节因子。
*   **分子层面**：
    *   **核心靶点**：发现 *fbxl3a*（编码一种调节生物钟核心负反馈蛋白降解的蛋白）的表达量随 *znf804a* 突变拷贝数的增加而呈剂量依赖性下降。
    *   **处理机制**：*znf804a* 缺失影响了特定转录本（如 *idh1*）的相对丰度，暗示其可能参与转录本的稳定性或剪接处理。
*   **整体结论**：*znf804a* 通过调控核心生物钟组件（如 *fbxl3a*）和转录本处理过程，进而干预生物体的昼夜节律。

### 7. 优点
*   **模型选择恰当**：斑马鱼幼鱼透明且具有保守的睡眠结构，适合高通量行为筛选。
*   **环境控制严谨**：通过 DD 实验排除了光照补偿效应，精准定位了内源性节律缺陷。
*   **剂量效应分析**：展示了从杂合子到纯合子的表型梯度，增强了结论的可信度。

### 8. 不足与局限
*   **因果验证尚缺**：虽然发现了 *fbxl3a* 表达下降，但未进行“回补实验”（即在突变体中过表达 *fbxl3a*）来确认其是否能修复行为缺陷。
*   **物种外推性**：斑马鱼与人类在神经系统复杂程度上存在差异，*ZNF804A* 在人类大脑中的具体作用机制仍需在哺乳动物模型或类器官中进一步验证。
*   **发育阶段局限**：研究仅限于幼鱼期，未探讨该基因缺失对成年斑马鱼长期睡眠模式及认知功能的影响。

（完）
