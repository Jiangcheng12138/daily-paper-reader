---
title: Arousal modulates functional connectivity through structured and hemispherically asymmetric community architecture during wakefulness
title_zh: 觉醒在清醒状态下通过结构化且半球不对称的社区架构调节功能连接
authors: "Kong, X., Li, S., Gong, G."
date: 2026-04-27
pdf: "https://www.biorxiv.org/content/10.64898/2026.01.06.697875v2.full.pdf"
tags: ["query:slp-ns"]
score: 9.0
evidence: 觉醒期间觉醒水平对功能连接的调节
tldr: 本研究探讨了清醒状态下唤醒水平波动如何影响大脑功能连接（FC）。通过结合7T高场强fMRI与同步瞳孔测量技术，研究发现唤醒水平并非均匀影响全脑，而是将FC组织成七个具有特定网络构成的连接群落。这些群落表现出显著的半球不对称性，特别是左半球呈现出向心式架构，作为唤醒信号汇聚的结构汇。这种组织模式在自然观影状态下依然稳健，揭示了唤醒调节大脑连接的内在结构化原则。
source: biorxiv
selection_source: fresh_fetch
motivation: 旨在探究清醒状态下瞬时唤醒水平的波动如何塑造大规模大脑功能连接的动态变化。
method: 采用7T高分辨率功能磁共振成像结合同步瞳孔测量技术，量化唤醒水平与功能连接随时间变化的协变关系。
result: 发现唤醒水平将功能连接组织成七个具有半球不对称性的群落，其中左半球在信号汇聚中表现出独特的向心式架构。
conclusion: 唤醒水平通过结构化且半球不对称的网络组织模式调节功能连接，这一机制在不同认知背景下具有高度的一致性。
---

## 摘要
觉醒在清醒状态下持续波动，然而这些瞬时变化如何塑造大规模功能连接（FC）仍不清楚。本研究结合了 7T fMRI 与同步瞳孔测量技术，旨在量化清醒人脑中每一个功能连接的时变 FC 如何随自发觉醒度而共变。研究发现，觉醒并非在整个连接组中施加统一影响，而是将 FC 组织成一组由七个连接社区组成的低维集合，每个社区均由特征性的网络组成所定义。这些社区表现出系统性的半球不对称性，特别识别出一种“左半球向心架构”，其中左半球作为觉醒调节信号不对称汇聚的结构汇。重要的是，半球不对称性并非源于连接强度的全局偏移，而是反映了嵌入在社区架构中的结构化空间异质性。这种模块化且不对称的组织在观看自然电影期间高度保留，表明 FC 的觉醒相关调节反映了在不同清醒认知背景下通用的内在原理。总之，这些发现表明，在清醒状态下，瞬时的觉醒波动通过结构化、半球不对称的网络组织来塑造大规模 FC。

## Abstract
Arousal fluctuates continuously during wakefulness, yet how these moment-to-moment variations shape large-scale functional connectivity (FC) remains unclear. Here, we combined 7T fMRI with concurrent pupillometry to quantify, for every functional connection, how time-varying FC covaries with spontaneous arousal in the awake human brain. Rather than exerting a uniform influence across the connectome, arousal organized FC into a low-dimensional set of seven connectivity communities, each defined by characteristic network compositions. These communities exhibited systematic hemispheric asymmetries, specifically identifying a "left-hemisphere centripetal architecture" where the left hemisphere serves as a structural sink for the asymmetric convergence of arousal-modulated signals. Importantly, hemispheric asymmetry did not arise from global shifts in connectivity strength, but instead reflected structured spatial heterogeneity embedded within community architecture. This modular and asymmetric organization was highly preserved during naturalistic movie watching, indicating that arousal-related modulation of FC reflects intrinsic principles that generalize across awake cognitive contexts. Together, these findings demonstrate that moment-to-moment arousal fluctuations shape large-scale FC through structured, hemispherically asymmetric network organization during wakefulness.

---

## 论文详细总结（自动生成）

这篇论文题为《Arousal modulates functional connectivity through structured and hemispherically asymmetric community architecture during wakefulness》，由北京师范大学龚高浪教授团队完成。以下是对该论文的结构化总结：

### 1. 核心问题与整体含义
*   **研究背景**：觉醒（Arousal）是调节感知、注意力和大规模神经系统协调的核心维度。虽然已知觉醒在清醒状态下会持续波动，但这种瞬时波动如何塑造全脑功能连接（FC）的动态组织仍不清楚。
*   **核心问题**：觉醒对功能连接的影响是全局均匀的，还是具有特定的空间结构？这种调节模式是否存在半球不对称性？
*   **整体含义**：研究揭示了觉醒通过一组低维、结构化且半球不对称的“连接社区”来重塑大脑通讯，为理解脑状态的动态调节提供了新的空间组织原则。

### 2. 方法论
*   **核心思想**：通过量化“觉醒-时变功能连接（tvFC）耦合”，在边缘（Edge）水平上绘制觉醒对全脑连接的影响图谱。
*   **关键技术流程**：
    1.  **觉醒量化**：利用同步瞳孔测量技术，提取瞳孔直径序列作为觉醒波动的代理指标。
    2.  **时变连接计算**：采用滑动窗口法（窗口30s，步长5s）计算400个对称ROI之间的动态相关性。
    3.  **耦合估计**：计算每个连接（Edge）的tvFC时间序列与瞳孔直径序列之间的Pearson相关性，生成“觉醒-tvFC耦合矩阵”。
    4.  **社区检测**：对耦合特征进行无监督K-means聚类，识别受觉醒调节的相似连接模式。
    5.  **不对称性度量**：定义“整合指数（Integration）”和“隔离指数（Segregation）”，量化觉醒调节在左右半球间的分布差异。

### 3. 实验设计
*   **数据集**：使用人类连接组计划（HCP）7T 高场强数据集。
*   **场景/范式**：
    *   **静息态（Resting-state）**：139名受试者，485个有效扫描运行（Runs）。
    *   **自然观影（Movie-watching）**：513个有效扫描运行，用于验证结论的跨情境稳定性。
*   **对比与验证**：
    *   使用**空间置换零模型（Spatial permutation null model）**作为统计基准。
    *   对比了不同连接类型（单模态 vs 跨模态）的参与熵。
    *   跨范式对比：使用匈牙利算法对齐静息态与观影态的社区结构。

### 4. 资源与算力
*   **算力说明**：论文中未明确说明具体的GPU/CPU型号、数量或具体的训练/计算时长。
*   **数据规模**：涉及约1000个高分辨率（7T）fMRI扫描序列的大规模预处理和统计建模，计算量主要集中在滑动窗口计算和大规模聚类分析上。

### 5. 实验数量与充分性
*   **实验规模**：样本量较大（N=139），涵盖了近千次扫描任务，数据质量高（7T）。
*   **充分性验证**：
    *   进行了**分半信度验证**和**受试者水平重采样**。
    *   执行了**敏感性分析**，排除了头动、全局信号等非神经噪声的干扰。
    *   进行了**跨认知背景（静息 vs 观影）**的验证。
*   **评价**：实验设计严谨，统计检验充分，通过多维度的鲁棒性测试确保了结果的客观性。

### 6. 主要结论与发现
*   **七大社区结构**：觉醒对连接组的影响并非弥散性的，而是组织成7个具有特定网络构成的低维社区。
*   **左半球向心架构**：发现了一种独特的“左半球向心架构（Left-hemisphere centripetal architecture）”，即左半球作为觉醒信号不对称汇聚的结构“汇（Sink）”。
*   **空间异质性驱动**：半球不对称性并非源于全局连接强度的偏移，而是源于社区内部高度结构化的空间异质性（梯度）。
*   **内在稳定性**：这种模块化和不对称的组织模式在静息和观影状态下高度一致，反映了大脑处理觉醒波动的内在原则。

### 7. 优点
*   **高分辨率视角**：利用7T fMRI的优势，在边缘水平（Edge-level）而非区域水平观察觉醒影响，提供了更精细的图谱。
*   **多模态结合**：将外周生理指标（瞳孔）与中枢神经活动（fMRI）紧密结合，捕捉瞬时动态。
*   **理论贡献**：挑战了觉醒是“全局均匀增益调节”的传统观点，提出了结构化调节的新模型。

### 8. 不足与局限
*   **下皮层缺失**：由于采用皮层分区，未直接分析驱动觉醒的关键下皮层核团（如蓝斑、丘脑）与皮层社区的直接互动。
*   **代理指标局限**：瞳孔直径虽是常用指标，但仍是觉醒的间接反映，未来需结合EEG等更高时间分辨率的手段。
*   **场强普适性**：结论基于7T数据，在临床常用的3T设备上是否能稳定观测到这些微细社区结构仍需验证。
*   **因果性方向**：作为相关性研究，尚无法完全确定觉醒波动与FC重构之间的因果方向。

（完）
