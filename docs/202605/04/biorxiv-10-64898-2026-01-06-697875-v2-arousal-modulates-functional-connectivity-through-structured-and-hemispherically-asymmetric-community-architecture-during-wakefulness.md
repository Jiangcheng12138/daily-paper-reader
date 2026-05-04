---
title: Arousal modulates functional connectivity through structured and hemispherically asymmetric community architecture during wakefulness
title_zh: 觉醒在清醒状态下通过结构化且半球不对称的社区架构调节功能连接
authors: "Kong, X., Li, S., Gong, G."
date: 2026-04-27
pdf: "https://www.biorxiv.org/content/10.64898/2026.01.06.697875v2.full.pdf"
tags: ["query:slp-ns"]
score: 9.0
evidence: 清醒期间的觉醒和功能连接
tldr: 本研究利用7T超高场强fMRI结合瞳孔测量技术，探究了清醒状态下觉醒水平波动对大脑功能连接（FC）的影响。研究发现觉醒水平并非均匀影响全脑，而是通过七个具有特定网络组成的连接社区来组织FC，并揭示了左半球向心架构的半球不对称性。这种模块化且不对称的组织在不同认知背景下具有高度稳定性，为理解觉醒如何塑造大规模脑网络提供了新视角。
source: biorxiv
selection_source: fresh_fetch
motivation: 旨在阐明清醒状态下瞬时觉醒水平的波动如何塑造大规模大脑功能连接的动态变化。
method: 结合7T高分辨率功能磁共振成像与同步瞳孔测量技术，量化功能连接随自发觉醒波动的协变关系。
result: 发现觉醒将功能连接组织成七个具有半球不对称性的社区，特别是识别出左半球作为觉醒调制信号汇聚点的“向心架构”。
conclusion: 觉醒水平通过结构化且半球不对称的模块化组织来调节大规模功能连接，且这种组织原则在不同认知任务中具有普适性。
---

## 摘要
觉醒在清醒状态下持续波动，然而这些瞬时变化如何塑造大规模功能连接（FC）仍不清楚。本研究结合了 7T fMRI 与同步瞳孔测量技术，旨在量化清醒人脑中每一个功能连接的时变 FC 如何随自发觉醒度而共变。研究发现，觉醒并非在整个连接组中施加统一影响，而是将 FC 组织成一组由七个连接社区组成的低维集合，每个社区均由特征性的网络组成所定义。这些社区表现出系统性的半球不对称性，特别识别出一种“左半球向心架构”，其中左半球作为觉醒调节信号不对称汇聚的结构汇。重要的是，半球不对称性并非源于连接强度的全局偏移，而是反映了嵌入在社区架构中的结构化空间异质性。这种模块化且不对称的组织在观看自然电影期间高度保留，表明 FC 的觉醒相关调节反映了在不同清醒认知背景下通用的内在原理。总之，这些发现表明，在清醒状态下，瞬时的觉醒波动通过结构化、半球不对称的网络组织来塑造大规模 FC。

## Abstract
Arousal fluctuates continuously during wakefulness, yet how these moment-to-moment variations shape large-scale functional connectivity (FC) remains unclear. Here, we combined 7T fMRI with concurrent pupillometry to quantify, for every functional connection, how time-varying FC covaries with spontaneous arousal in the awake human brain. Rather than exerting a uniform influence across the connectome, arousal organized FC into a low-dimensional set of seven connectivity communities, each defined by characteristic network compositions. These communities exhibited systematic hemispheric asymmetries, specifically identifying a "left-hemisphere centripetal architecture" where the left hemisphere serves as a structural sink for the asymmetric convergence of arousal-modulated signals. Importantly, hemispheric asymmetry did not arise from global shifts in connectivity strength, but instead reflected structured spatial heterogeneity embedded within community architecture. This modular and asymmetric organization was highly preserved during naturalistic movie watching, indicating that arousal-related modulation of FC reflects intrinsic principles that generalize across awake cognitive contexts. Together, these findings demonstrate that moment-to-moment arousal fluctuations shape large-scale FC through structured, hemispherically asymmetric network organization during wakefulness.

---

## 论文详细总结（自动生成）

这是一份关于论文《Arousal modulates functional connectivity through structured and hemispherically asymmetric community architecture during wakefulness》的结构化深入总结：

### 1. 论文的核心问题与整体含义（研究动机和背景）
*   **核心问题**：在清醒状态下，人的觉醒水平（Arousal）会发生瞬时的自发波动。论文旨在探究这些细微的觉醒波动如何塑造大脑大规模功能连接（FC）的动态组织。
*   **研究背景**：过去的研究多关注离散状态（如清醒与睡眠、麻醉的对比），或仅关注局部脑区的信号振幅。目前尚不清楚觉醒对全脑功能连接的影响是全局均匀的，还是具有特定的空间结构和半球不对称性。

### 2. 论文提出的方法论
*   **核心思想**：通过结合超高场强（7T）功能磁共振成像（fMRI）与同步瞳孔测量技术，量化每一个功能连接（Edge）随觉醒水平波动的协变程度。
*   **关键技术细节**：
    *   **觉醒指标**：使用瞳孔直径作为觉醒水平的连续生理指标。
    *   **时变功能连接（tvFC）**：采用滑动窗口法（窗口长30秒，步长5秒）计算全脑400个感兴趣区域（ROI）之间的动态相关性。
    *   **耦合量化（Arousal–tvFC coupling）**：计算每个连接的tvFC时间序列与瞳孔直径序列之间的皮尔逊相关性，生成“觉醒-tvFC耦合矩阵”。
    *   **社区检测**：对耦合矩阵进行无监督聚类（K-means），将具有相似觉醒敏感性的连接归类为不同的“连接社区”。
    *   **不对称性分析**：利用对称的皮层分区，计算整合指数（Integration）和隔离指数（Segregation），评估觉醒调节在左右半球之间的差异。

### 3. 实验设计
*   **数据集**：使用人类连接组计划（HCP）7T 数据集，包含139名健康受试者。
*   **实验场景**：
    *   **静息态（Resting-state）**：作为基准，分析内在的组织原则。
    *   **自然电影观看（Movie-watching）**：作为跨任务验证，测试发现的组织模式在复杂认知背景下的稳定性。
*   **对比与验证**：
    *   使用**空间置换零模型（Spatial Permutation Null Model）**来验证半球不对称性的显著性。
    *   通过**分半信度（Split-half）**和**重采样（Resampling）**验证社区结构的鲁棒性。
    *   对比了不同模态（单峰 vs 跨峰网络）的参与特征。

### 4. 资源与算力
*   **算力说明**：论文中**未明确说明**具体的 GPU 型号、数量或训练时长。由于该研究主要涉及 fMRI 图像预处理、统计建模和无监督聚类，而非深度学习大模型的训练，其算力需求主要集中在处理 HCP 7T 高分辨率大数据集的存储和并行计算上。

### 5. 实验数量与充分性
*   **实验规模**：分析了485个静息态扫描运行（Runs）和513个电影观看运行。
*   **充分性评估**：
    *   **样本量**：N=139 在高场强 fMRI 研究中属于较大样本。
    *   **多维度验证**：进行了消融实验性质的控制分析（如控制头动、全局信号），并对滑动窗口参数、时间延迟等进行了敏感性分析。
    *   **客观性**：通过跨任务（静息 vs 电影）的一致性分析，证明了结论并非特定场景的偶然发现，实验设计严谨且客观。

### 6. 论文的主要结论与发现
*   **七大社区架构**：觉醒对连接组的影响并非均匀分布，而是组织成7个低维连接社区，每个社区有独特的网络组成（如单峰网络参与度较低，跨峰网络参与度较高）。
*   **左半球向心架构**：发现了一种显著的半球不对称性，左半球表现为觉醒调节信号的“结构汇（Structural Sink）”，即左半球倾向于整合来自双侧的觉醒调节输入。
*   **空间异质性驱动**：半球不对称性并非源于全局连接强度的偏移，而是源于社区内部空间分布的异质性（梯度）。
*   **跨背景稳定性**：这种模块化和不对称的组织模式在观看电影时依然存在，说明它是大脑处理觉醒信号的内在固有原则。

### 7. 优点（亮点）
*   **高分辨率视角**：利用 7T fMRI 的高信噪比，捕捉到了 3T 扫描可能忽略的细微社区结构。
*   **从“边”出发**：不同于传统的基于“点（脑区）”的分析，本文从“连接（边）”的角度揭示了觉醒如何重塑脑网络拓扑。
*   **揭示不对称机制**：首次系统性地将觉醒波动与大规模 FC 的半球侧化联系起来，并提出了“向心架构”的概念。

### 8. 不足与局限
*   **间接指标**：瞳孔直径虽然是公认的觉醒指标，但仍属于外周生理信号，不能完全等同于中枢神经系统的觉醒状态。
*   **缺乏皮层下直接证据**：虽然推测这些模式受蓝斑（LC）等核团驱动，但受限于分析框架，未直接对皮层下核团进行整合建模。
*   **分区方案依赖**：结论基于特定的对称皮层分区方案，虽然做了鲁棒性检验，但不同分区方案可能对微小边界的定义存在偏差。
*   **因果关系不明**：作为相关性研究，尚无法确定是觉醒波动导致了 FC 改变，还是 FC 的动态切换引起了觉醒水平的变化。

（完）
