---
title: Arousal modulates functional connectivity through structured and hemispherically asymmetric community architecture during wakefulness
title_zh: 觉醒度在清醒状态下通过结构化且半球不对称的社区架构调节功能连接
authors: "Kong, X., Li, S., Gong, G."
date: 2026-04-27
pdf: "https://www.biorxiv.org/content/10.64898/2026.01.06.697875v2.full.pdf"
tags: ["query:slp-ns"]
score: 9.0
evidence: 清醒状态下的觉醒与功能连接
tldr: 本研究利用7T高场强磁共振成像结合瞳孔测量技术，探究了清醒状态下觉醒水平波动对大脑功能连接（FC）的影响。研究发现，觉醒并非均匀影响全脑，而是将FC组织成七个具有特定网络构成的连接群落，并呈现出显著的半球不对称性，特别是左半球表现为信号汇聚的“向心架构”。这种组织模式在自然观影状态下依然稳定，揭示了觉醒调节大脑连接的内在结构化原则。
source: biorxiv
selection_source: fresh_fetch
motivation: 旨在阐明清醒状态下瞬时觉醒水平的波动如何塑造大规模大脑功能连接的动态变化。
method: 结合7T超高场强功能磁共振成像与同步瞳孔测量技术，量化觉醒程度与功能连接随时间变化的协变关系。
result: 觉醒将功能连接组织成七个模块化群落，并表现出以左半球为信号汇聚中心的显著半球不对称性。
conclusion: 觉醒对大脑功能连接的调节遵循结构化且半球不对称的组织原则，且这种模式在不同认知背景下具有高度稳定性。
---

## 摘要
清醒状态下，觉醒度持续波动，但这些瞬时变化如何塑造大规模功能连接（FC）仍不清楚。本研究结合了 7T fMRI 与同步瞳孔测量技术，旨在量化清醒人脑中每一个功能连接的时变 FC 如何随自发觉醒度而共变。觉醒度并非对整个连接组产生均匀影响，而是将 FC 组织成一组由七个连接社区组成的低维集合，每个社区都由特征性的网络组成所定义。这些社区表现出系统性的半球不对称性，特别识别出一种“左半球向心架构”，其中左半球作为觉醒调节信号不对称汇聚的结构汇。重要的是，半球不对称性并非源于连接强度的全局偏移，而是反映了嵌入在社区架构中的结构化空间异质性。这种模块化且不对称的组织在观看自然电影期间高度保留，表明与觉醒相关的 FC 调节反映了在不同清醒认知背景下具有普适性的内在原理。总之，这些发现表明，在清醒状态下，瞬时觉醒波动通过结构化、半球不对称的网络组织来塑造大规模 FC。

## Abstract
Arousal fluctuates continuously during wakefulness, yet how these moment-to-moment variations shape large-scale functional connectivity (FC) remains unclear. Here, we combined 7T fMRI with concurrent pupillometry to quantify, for every functional connection, how time-varying FC covaries with spontaneous arousal in the awake human brain. Rather than exerting a uniform influence across the connectome, arousal organized FC into a low-dimensional set of seven connectivity communities, each defined by characteristic network compositions. These communities exhibited systematic hemispheric asymmetries, specifically identifying a "left-hemisphere centripetal architecture" where the left hemisphere serves as a structural sink for the asymmetric convergence of arousal-modulated signals. Importantly, hemispheric asymmetry did not arise from global shifts in connectivity strength, but instead reflected structured spatial heterogeneity embedded within community architecture. This modular and asymmetric organization was highly preserved during naturalistic movie watching, indicating that arousal-related modulation of FC reflects intrinsic principles that generalize across awake cognitive contexts. Together, these findings demonstrate that moment-to-moment arousal fluctuations shape large-scale FC through structured, hemispherically asymmetric network organization during wakefulness.

---

## 论文详细总结（自动生成）

这是一份关于论文《Arousal modulates functional connectivity through structured and hemispherically asymmetric community architecture during wakefulness》的结构化深度总结：

### 1. 核心问题与整体含义（研究动机和背景）
*   **核心问题**：在清醒状态下，人的觉醒水平（Arousal）会发生瞬时的自发波动。研究旨在探究这种波动如何塑造全脑大规模功能连接（FC）的动态组织模式。
*   **背景**：以往研究多关注不同意识状态（如睡眠、麻醉）间的FC差异，但对清醒状态下细微觉醒波动如何影响连接组（Connectome）缺乏精细刻画。此外，觉醒调节是否具有空间特异性以及是否存在半球不对称性，也是神经科学领域长期悬而未决的问题。

### 2. 方法论：核心思想与技术细节
*   **核心思想**：通过同步采集超高场强fMRI数据和瞳孔直径（作为觉醒度的生理指标），量化每一个功能连接（Edge）随觉醒水平波动的共变程度。
*   **关键流程**：
    1.  **时变功能连接（tvFC）计算**：使用滑动窗口法（窗口30s，步长5s）计算400个脑区两两之间的动态相关性。
    2.  **觉醒指标提取**：对瞳孔直径进行预处理（去噪、插值、平滑），并降采样至与fMRI相同的时间分辨率。
    3.  **觉醒-tvFC耦合量化**：计算每个连接的tvFC序列与瞳孔直径序列之间的皮尔逊相关系数，生成“觉醒-tvFC耦合矩阵”。
    4.  **社区检测（Community Detection）**：对耦合矩阵进行无监督聚类（K-means），将具有相似觉醒敏感性的连接归类为不同的“连接社区”。
    5.  **不对称性分析**：定义了**整合指数（Integration）**和**隔离指数（Segregation）**，用于量化觉醒调节在左右半球内及半球间的分布差异。

### 3. 实验设计与对比
*   **数据集**：使用了著名的 **HCP (Human Connectome Project) 7T 数据集**，包含139名健康受试者。
*   **实验场景**：
    *   **静息态（Resting State）**：作为基准场景，探究内在的组织原则。
    *   **自然观影（Movie Watching）**：作为验证场景，测试发现的组织模式在复杂认知任务下是否具有跨情境的稳定性。
*   **对比与验证**：
    *   使用**空间排列零模型（Spatial Permutation Null Model）**来验证半球不对称性的显著性。
    *   通过**折半信度（Split-half）**和**受试者水平重采样**验证社区结构的鲁棒性。
    *   对比了不同功能网络（如DMN、FPN、视觉网络等）在觉醒调节中的参与度差异。

### 4. 资源与算力
*   **算力说明**：论文中**未明确说明**具体的GPU型号、数量或训练时长。
*   **技术栈**：提到使用了 Python 生态系统（NumPy, SciPy, scikit-learn）进行算法实现，并使用 Matplotlib, Seaborn, Surfplot 进行可视化。由于涉及7T高分辨率数据的处理和大规模矩阵运算，推测需要高性能计算集群支持。

### 5. 实验数量与充分性
*   **实验规模**：分析了485个静息态扫描序列和513个观影扫描序列，样本量在7T研究中属于较大规模。
*   **充分性评价**：
    *   **非常充分**：研究不仅在静息态下发现了模式，还在观影状态下进行了跨情境验证。
    *   **多维度验证**：包含了社区稳定性测试、节点水平的熵分析、空间异质性分析以及针对头动和全局信号等混淆因素的敏感性分析。
    *   **客观性**：使用了无监督聚类和严格的零模型检验，确保了结论的客观性。

### 6. 主要结论与发现
*   **低维社区架构**：觉醒对连接组的影响并非全局均匀的，而是组织成**7个不同的连接社区**，每个社区有特定的网络组成。
*   **左半球向心架构**：发现了一种显著的半球不对称性，即“左半球向心架构”。左半球作为觉醒调节信号的汇聚中心，优先整合了来自同侧和对侧的输入。
*   **空间异质性驱动**：半球不对称性并非源于平均连接强度的整体偏移，而是源于社区内部**空间分布的异质性（梯度）**。
*   **跨情境稳定性**：这种模块化且不对称的组织模式在静息态和观影态之间高度一致，反映了大脑内在的生理组织原则。

### 7. 优点与亮点
*   **高分辨率视角**：利用7T fMRI的优势，在“边（Edge）”水平上精细刻画了觉醒的调节作用，而非传统的区域水平。
*   **创新的分析框架**：将觉醒波动与动态FC耦合，并引入社区检测和不对称性指数，为理解脑态切换提供了新工具。
*   **揭示了深层原则**：明确了觉醒调节与大脑内在层次结构（如单峰-跨峰梯度）之间的关联。

### 8. 不足与局限
*   **缺乏皮层下深度分析**：虽然推测这些模式受蓝斑（LC）或丘脑等皮层下结构驱动，但受限于分析框架（对称皮层分区），未直接纳入皮层下核团的实证分析。
*   **瞳孔指标的间接性**：瞳孔直径虽是觉醒的良好指标，但仍属于外周生理信号，未来需结合EEG等电生理手段进行多模态验证。
*   **场强泛化性**：研究完全基于7T数据，在更普及的3T磁共振设备上是否能稳定观测到这些精细社区结构尚待验证。
*   **因果关系不明**：目前的研究属于相关性分析，无法确定觉醒波动是FC改变的原因还是结果。

（完）
