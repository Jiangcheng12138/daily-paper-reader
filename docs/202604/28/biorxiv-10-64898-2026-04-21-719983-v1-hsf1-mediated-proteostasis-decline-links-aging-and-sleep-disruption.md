---
title: HSF1-mediated Proteostasis Decline Links Aging and Sleep Disruption
authors: "Yamazaki, S., Reddy, A. B."
date: 2026-04-24
pdf: "https://www.biorxiv.org/content/10.64898/2026.04.21.719983v1.full.pdf"
tags: ["query:slp-ns"]
score: 9.0
evidence: 连接衰老与睡眠中断的分子机制
tldr: 本研究通过整合人类和小鼠的转录组与蛋白质组数据，揭示了睡眠中断与衰老之间的分子联系。研究发现，HSF1介导的蛋白质稳态网络在慢性睡眠不足和衰老过程中表现出一致的下调趋势，这与短期睡眠剥夺引起的瞬时激活截然不同。这种衰减在海马体和皮层神经元中尤为严重，表明慢性睡眠压力会削弱细胞的应激保护能力。该研究确立了HSF1介导的蛋白质稳态是连接睡眠稳定性和分子衰老的关键轴，揭示了两者相互影响、加速衰老的系统级机制。
source: biorxiv
selection_source: fresh_fetch
motivation: 旨在阐明睡眠中断与衰老之间关联的分子机制，特别是蛋白质稳态如何介导这一过程。
method: 采用跨物种、跨组织的转录组和蛋白质组整合分析，对比慢性睡眠干扰与自然衰老的分子特征。
result: 识别出HSF1介导的热休克反应是核心信号，其在慢性睡眠不足和衰老中从适应性激活转变为持续性下调。
conclusion: 慢性睡眠中断通过削弱HSF1介导的蛋白质稳态应激反应，加速了分子层面的衰老进程并增加了神经系统的脆弱性。
---

## Abstract
Sleep disruption increases with age and is associated with adverse age-related outcomes, yet the molecular mechanisms linking these phenomena remain unclear. Here, through integrative analysis of human and mouse transcriptomic and proteomic datasets, we identify proteostasis-related pathways whose aging trajectories align with transcriptional responses to chronic sleep disruption across tissues and cell types. In the human prefrontal cortex, gene expression exhibits coherent age-associated directional shifts. Across human peripheral blood following sleep restriction and multiple aging mouse tissues and cell types, proteostasis pathways exhibit concordant downregulation. Among these, heat shock response pathways emerge as the most persistent and cross-modal signatures, with components of the heat shock factor 1 (HSF1)-mediated proteostasis network displaying diminished inducibility with age and chronic sleep insufficiency, in contrast to transient activation following short-term sleep deprivation. This attenuation is particularly pronounced in neurons, where age-associated suppression of HSF1 target programs indicates selective vulnerability of neuronal proteostasis. Spatial and single-cell analyses map this vulnerability to hippocampal circuits during aging and to superficial cortical layers and glutamatergic neurons in Alzheimers disease. These findings support a model in which repeated sleep disruption progressively reduces the inducible capacity of proteostatic stress responses, shifting from adaptive activation to progressive attenuation and accelerating age-related decline in proteome maintenance. Consistent with emerging functional evidence, this identifies HSF1-mediated proteostasis as an integrative axis linking sleep stability and molecular aging, suggesting a self-reinforcing relationship in which sleep disruption and proteostasis decline reciprocally exacerbate one another. These results connect transient molecular responses to sleep perturbations with long-term aging trajectories, revealing a systems-level mechanism through which cumulative sleep disruption may increase vulnerability during aging.

---

## 论文详细总结（自动生成）

这篇论文深入探讨了睡眠中断与衰老之间的分子关联，以下是对该研究的结构化总结：

### 1. 核心问题与整体含义（研究动机和背景）
*   **核心问题**：虽然已知睡眠中断会随年龄增长而加剧，并与多种老年疾病相关，但连接“睡眠不足”与“生物学衰老”的底层分子机制仍不明确。
*   **研究动机**：研究者旨在探究是否存在共同的分子通路，使得长期的睡眠压力能够加速衰老进程，或者衰老如何削弱了生物体应对睡眠压力的能力。
*   **整体含义**：研究确立了 **HSF1（热休克因子1）介导的蛋白质稳态（Proteostasis）** 是连接睡眠稳定性和分子衰老的关键轴心。

### 2. 论文提出的方法论
*   **核心思想**：通过跨物种（人类和小鼠）、跨组织（脑部与外周）、跨模态（转录组与蛋白质组）的整合分析，寻找在慢性睡眠中断和自然衰老中表现一致的分子特征。
*   **关键技术细节**：
    *   **多组学整合**：对比人类前额叶皮层、外周血以及小鼠多种组织在衰老和睡眠干预下的基因表达差异。
    *   **时效性对比**：区分“短期睡眠剥夺”（急性应激）与“长期睡眠限制”（慢性压力）对蛋白质稳态网络的不同影响。
    *   **空间与单细胞分析**：利用单细胞测序和空间转录组技术，精确定位受影响的特定细胞群（如海马体回路、皮层谷氨酸能神经元）。

### 3. 实验设计
*   **数据集/场景**：
    *   **人类数据**：前额叶皮层（PFC）衰老转录组、外周血睡眠限制实验数据。
    *   **小鼠数据**：涵盖多种组织和细胞类型的衰老图谱。
    *   **疾病模型**：阿尔茨海默病（AD）相关的单细胞数据。
*   **对比基准（Benchmark）**：
    *   对比了**急性睡眠剥夺**（通常引起应激反应激活）与**慢性睡眠不足/自然衰老**（表现为反应能力衰减）。
    *   对比了不同脑区和细胞类型对蛋白质稳态失效的敏感性。

### 4. 资源与算力
*   **算力说明**：论文中未明确提及具体的 GPU 型号、数量或训练时长。此类生物信息学研究通常侧重于统计分析、差异表达分析和多组学整合算法，对大规模深度学习算力的需求相对较低，更多依赖于高性能计算集群（HPC）进行序列比对和数据处理。

### 5. 实验数量与充分性
*   **实验规模**：研究整合了多套公开的大规模人类和小鼠数据集，涵盖了从整体组织到单细胞层面的多个维度。
*   **充分性评价**：实验设计非常充分。通过跨物种（人与鼠）的一致性验证，增强了结论的普适性；通过区分急性与慢性效应，揭示了机制的动态演变；引入 AD 疾病模型进一步验证了该机制在病理状态下的临床相关性。

### 6. 论文的主要结论与发现
*   **HSF1 反应的转变**：短期睡眠剥夺会触发 HSF1 介导的保护性热休克反应（暂时性激活），但慢性睡眠中断和衰老会导致该通路从“适应性激活”转变为“持续性下调”。
*   **蛋白质稳态崩溃**：慢性睡眠不足会削弱细胞维持蛋白质组稳定的能力，这种现象在海马体和皮层神经元中尤为显著。
*   **恶性循环**：研究提出了一个模型，即睡眠中断与蛋白质稳态衰减相互加剧——睡眠不足加速分子衰老，而衰老进一步破坏睡眠稳定性。
*   **神经元脆弱性**：识别出谷氨酸能神经元是蛋白质稳态失效的高危群体，这解释了为何睡眠问题常与认知退化相关。

### 7. 优点（亮点）
*   **系统级视角**：不局限于单一组织，而是揭示了全身性（外周到中枢）的分子协同变化。
*   **动态机制解析**：成功解释了为什么偶尔熬夜（急性）和长期失眠（慢性）对身体的影响在分子层面上存在本质区别。
*   **高分辨率定位**：利用空间转录组技术将抽象的分子通路落实到了具体的脑回路和细胞亚群上。

### 8. 不足与局限
*   **因果律验证**：虽然数据分析显示了强相关性，但对于“HSF1 下调直接导致衰老加速”的直接功能性干预实验（如在老年模型中增强 HSF1 是否能逆转睡眠缺失损害）在本文中体现较少。
*   **数据异质性**：整合多套来自不同实验室的数据集可能存在批次效应或实验条件的细微偏差。
*   **应用限制**：目前发现主要集中在分子标志物层面，如何将其转化为临床干预手段（如靶向 HSF1 的药物）仍有较长距离。

（完）
