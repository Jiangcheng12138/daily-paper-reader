---
title: Arousal modulates functional connectivity through structured and hemispherically asymmetric community architecture during wakefulness
title_zh: 觉醒度在清醒状态下通过结构化且半球不对称的社区架构调节功能连接
authors: "Kong, X., Li, S., Gong, G."
date: 2026-04-27
pdf: "https://www.biorxiv.org/content/10.64898/2026.01.06.697875v2.full.pdf"
tags: ["query:slp-ns"]
score: 9.0
evidence: 觉醒期间觉醒水平调节功能连接
tldr: 本研究探讨了清醒状态下瞬时觉醒水平如何调节大脑功能连接（FC）。通过结合7T超高场强fMRI与同步瞳孔测量技术，研究发现觉醒并非均匀影响全脑，而是将FC组织成七个具有特定网络构成的模块化社区。这些社区表现出显著的半球不对称性，特别是左半球作为觉醒调节信号的汇聚中心。这种组织模式在自然观影状态下依然稳健，揭示了觉醒调节大脑连接的内在结构化原则。
source: biorxiv
selection_source: fresh_fetch
motivation: 旨在阐明清醒状态下瞬时觉醒波动如何塑造大规模大脑功能连接的动态变化。
method: 采用7T高分辨率功能磁共振成像（fMRI）结合同步瞳孔测量技术，量化觉醒水平与功能连接随时间变化的协变关系。
result: 发现觉醒将功能连接组织成七个模块化社区，并呈现出以左半球为信号汇聚中心的系统性半球不对称架构。
conclusion: 觉醒通过结构化且半球不对称的网络组织模式调节功能连接，这一内在原则在不同认知背景下具有普适性。
---

## 摘要
觉醒度在清醒状态下持续波动，但这些瞬时变化如何塑造大规模功能连接（FC）仍不清楚。在本研究中，我们结合了 7T fMRI 与同步瞳孔测量技术，以量化清醒人脑中每一个功能连接的时变 FC 如何随自发觉醒度而共变。觉醒度并非对整个连接组产生统一影响，而是将 FC 组织成一组由七个连接社区组成的低维集合，每个社区都由特征性的网络组成所定义。这些社区表现出系统性的半球不对称性，特别是识别出一种“左半球向心架构”，其中左半球作为觉醒调节信号不对称汇聚的结构汇。重要的是，半球不对称性并非源于连接强度的全局偏移，而是反映了嵌入在社区架构中的结构化空间异质性。这种模块化且不对称的组织在观看自然主义电影期间高度保留，表明与觉醒相关的 FC 调节反映了在不同清醒认知背景下通用的内在原理。总之，这些研究结果表明，在清醒状态下，瞬时的觉醒波动通过结构化、半球不对称的网络组织来塑造大规模 FC。

## Abstract
Arousal fluctuates continuously during wakefulness, yet how these moment-to-moment variations shape large-scale functional connectivity (FC) remains unclear. Here, we combined 7T fMRI with concurrent pupillometry to quantify, for every functional connection, how time-varying FC covaries with spontaneous arousal in the awake human brain. Rather than exerting a uniform influence across the connectome, arousal organized FC into a low-dimensional set of seven connectivity communities, each defined by characteristic network compositions. These communities exhibited systematic hemispheric asymmetries, specifically identifying a "left-hemisphere centripetal architecture" where the left hemisphere serves as a structural sink for the asymmetric convergence of arousal-modulated signals. Importantly, hemispheric asymmetry did not arise from global shifts in connectivity strength, but instead reflected structured spatial heterogeneity embedded within community architecture. This modular and asymmetric organization was highly preserved during naturalistic movie watching, indicating that arousal-related modulation of FC reflects intrinsic principles that generalize across awake cognitive contexts. Together, these findings demonstrate that moment-to-moment arousal fluctuations shape large-scale FC through structured, hemispherically asymmetric network organization during wakefulness.

---

## 论文详细总结（自动生成）

这是一份关于论文《Arousal modulates functional connectivity through structured and hemispherically asymmetric community architecture during wakefulness》的结构化深入总结：

### 1. 核心问题与整体含义（研究动机和背景）
*   **核心问题**：在清醒状态下，大脑的觉醒水平（Arousal）会发生细微且持续的瞬时波动。过去的研究多关注不同意识状态（如睡眠 vs. 清醒）间的剧烈变化，但对于**清醒状态下这种时刻变化的觉醒波动如何塑造大规模全脑功能连接（FC）的动态组织**，以及这种调节是否存在**半球不对称性**，目前尚不清楚。
*   **整体含义**：研究旨在揭示觉醒对大脑连接组的调节并非全局统一的“背景噪音”，而是一种具有高度空间结构化、低维模块化且半球不对称的内在组织原则。

### 2. 方法论：核心思想与关键技术
*   **核心思想**：通过同步采集高分辨率功能磁共振成像（fMRI）和瞳孔测量数据，量化每一个功能连接（Edge）随觉醒水平波动的共变程度。
*   **关键技术细节**：
    *   **觉醒度量化**：使用瞳孔直径作为觉醒的生理指标，经过预处理（去伪影、插值、平滑）后降采样至 1Hz。
    *   **时变功能连接（tvFC）**：采用滑动窗口法（窗口 30s，步长 5s）计算 400个对称皮层区域之间的 Pearson 相关系数。
    *   **觉醒-tvFC 耦合**：计算每个连接的 tvFC 时间序列与瞳孔直径序列之间的相关性，生成“耦合矩阵”。
    *   **社区检测**：对耦合矩阵进行无监督聚类（K-means），将全脑连接划分为具有相似觉醒敏感性的“连接社区”。
    *   **不对称性分析**：定义了**整合指数（Integration）**和**隔离指数（Segregation）**，用于量化觉醒调节在左右半球内及半球间的分布差异。

### 3. 实验设计与对比
*   **数据集**：使用了 **HCP (Human Connectome Project) 7T 数据集**，包含 139 名健康受试者的静息态（Resting-state）和自然主义观影（Movie-watching）数据。
*   **场景对比**：
    *   **静息态 vs. 观影态**：验证觉醒调节模式在不同认知背景下的稳定性。
    *   **真实数据 vs. 空间置换零模型（Null Model）**：通过 10,000 次空间置换检验半球不对称性的显著性。
*   **基准（Benchmark）**：以全脑平均水平和经典的 Yeo 七网络（DMN, FPN 等）作为空间分布的参照。

### 4. 资源与算力
*   **算力说明**：论文中**未明确说明**具体的 GPU 型号、数量或训练时长。
*   **实现工具**：提到使用了 Python (NumPy, SciPy, scikit-learn) 进行算法实现，并使用 Matplotlib, Seaborn 和 Surfplot 进行可视化。

### 5. 实验数量与充分性
*   **实验规模**：分析了 485 个静息态扫描序列和 513 个观影态扫描序列，样本量较大且数据质量极高（7T 超高场强）。
*   **充分性验证**：
    *   进行了**折半信度检验（Split-half）**和**受试者水平的重采样（Resampling）**。
    *   控制了头动、全局信号等非神经混杂因素。
    *   跨任务（静息 vs. 观影）的一致性分析证明了结果的普适性。
*   **评价**：实验设计非常严谨，通过多维度的鲁棒性分析确保了结论的客观性和公平性。

### 6. 主要结论与发现
*   **七大社区架构**：觉醒对 FC 的调节表现为 7 个稳定的低维社区，而非全脑均匀分布。
*   **左半球向心架构**：发现了一种显著的半球不对称性，左半球表现为觉醒调节信号的“汇聚中心”（左半球内的连接增强，且右半球向左半球的输入也受到显著调节）。
*   **空间异质性驱动**：半球不对称性并非源于平均连接强度的全局改变，而是源于社区内部复杂的空间梯度（异质性）。
*   **跨情境稳定性**：这种模块化和不对称的组织原则在静息和观影状态下高度一致，反映了大脑的内在属性。

### 7. 优点与亮点
*   **高分辨率数据**：利用 7T fMRI 的高信噪比，捕捉到了以往 3T 研究可能忽略的细微连接动态。
*   **创新的耦合视角**：不只是看区域激活，而是看“连接-觉醒”的动态耦合，提供了连接组学的新维度。
*   **严谨的对称性框架**：使用了专门设计的对称皮层分区，确保了半球比较的数学严密性。

### 8. 不足与局限
*   **缺乏皮层下分析**：由于使用了对称皮层分区，未直接分析驱动觉醒的关键结构（如蓝斑、丘脑等皮层下核团），相关机制仍属推测。
*   **瞳孔指标的局限**：瞳孔虽然是良好的觉醒代理指标，但仍属于外周生理信号，未来需结合 EEG 等多模态数据。
*   **设备依赖性**：结论基于 7T 数据，在更普及的 3T 临床设备上是否能稳定复现尚待验证。
*   **因果关系不明**：目前的研究属于相关性分析，无法确定是觉醒波动导致了 FC 改变，还是大脑状态切换引起了瞳孔变化。

（完）
