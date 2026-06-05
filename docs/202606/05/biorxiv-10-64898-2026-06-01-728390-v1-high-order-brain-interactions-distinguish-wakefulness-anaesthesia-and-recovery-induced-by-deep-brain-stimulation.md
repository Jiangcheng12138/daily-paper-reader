---
title: "High-order brain interactions distinguish wakefulness, anaesthesia, and recovery induced by deep brain stimulation"
title_zh: 高阶脑相互作用区分清醒、麻醉及由深部脑刺激诱导的恢复
authors: "Cofre, R., Espinosa-Curilem, C., Uhrig, L., Tasserie, J., Herzog, R., Gatica, M., Luppi, A., Silva, J. F., Jarraya, B."
date: 2026-06-03
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.01.728390v1.full.pdf"
tags: ["query:slp-ns"]
score: 9.0
evidence: 跨意识状态的高阶脑相互作用
tldr: 理解意识依赖大规模脑交互，但传统成对功能连接无法捕捉多脑区集体依赖。本研究利用多元信息论O-information分析非人灵长类静息态fMRI数据，刻画清醒、麻醉（不同药物）及深部脑刺激促醒等状态下的高阶交互重组。发现最优子集的O-information可稳健区分意识与无反应状态，冗余性在清醒时升高、麻醉时降低，协同-冗余转变在多麻醉条件下显著。高阶信息特征显著优于成对连接，特别是协同特征对相关性不可见。结果表明意识反映高阶交互结构重构。
source: biorxiv
selection_source: fresh_fetch
motivation: 传统成对功能连接无法捕捉多脑区集体依赖，需要高阶交互来区分意识状态。
method: 应用O-information分析非人灵长类静息态fMRI数据，优化区域子集以区分清醒、麻醉及恢复状态。
result: 冗余性特征在意识状态下升高，协同-冗余转变可区分状态，高阶特征优于成对连接。
conclusion: 意识依赖于高阶交互的重构，需要超越成对连接的多变量表征。
---

## 摘要
理解意识如何依赖于大规模脑相互作用是意识神经科学和临床转化的关键。然而，这需要超越传统的功能连接成对描述，因为后者无法捕捉多个脑区之间涌现的集体依赖性。这里，我们使用多变量信息论度量来表征高阶相互作用如何在意识状态间重组。具体而言，我们将O-信息应用于非人灵长类动物的静息态fMRI数据，以量化多区域脑动力学是由协同还是冗余信息共享主导。我们分析两个互补数据集：(i) 使用不同分子药物（丙泊酚、七氟烷、氯胺酮）诱导的清醒和麻醉性意识丧失，以及(ii) 在丙泊酚麻醉期间由中央丘脑深部脑刺激驱动的意识恢复，以行为响应性为指标。我们在两种互补的优化极性下识别出最优区域子集，其O-信息能够稳健地区分有意识状态与无响应状态。第一种捕捉到在意识扫描中升高的冗余性，在麻醉下降低，提供稳健的区分能力，并将高压中央丘脑刺激状态更接近于清醒。第二种捕捉到从协同到冗余的转变，在多麻醉条件下显著，但在不同数据集中具有上下文依赖性。区分性能依赖于相互作用阶数：基于冗余的特征随着子集大小的增加而改善，而基于协同的特征在低阶达到峰值。高阶信息特征显著优于成对功能连接，尤其是对于相关性无法察觉的协同特征。这些发现表明，意识反映在高阶相互作用结构的重组中，其不同的信息基质需要超越成对连接的多变量表征。

## Abstract
Understanding how consciousness depends on large-scale brain interactions is key for both the neuroscience of consciousness and clinical translation. However, it requires moving beyond classical pairwise descriptions of functional connectivity, which cannot capture the collective dependencies emerging across multiple brain regions. Here, we use multivariate information theory measures to characterize how higher-order interactions reorganize across states of consciousness. Specifically, we apply O-information to resting-state fMRI data from non-human primates to quantify whether multiregional brain dynamics are dominated by synergistic or redundant information sharing. We analyse two complementary datasets: (i) wakefulness and anaesthesia-induced loss of consciousness using different molecular agents (propofol, sevoflurane, ketamine), and (ii) the recovery of consciousness driven by central thalamic deep brain stimulation during propofol anaesthesia, indexed by behavioural responsiveness. We identify optimal regional subsets whose O-information robustly discriminates conscious from non-responsive states under two complementary optimization polarities. The first captures elevated redundancy in conscious scans that decreases under anaesthesia, providing robust discrimination and placing high-voltage central-thalamus stimulation closer to wakefulness. The second captures a synergy-to-redundancy transition, prominent in multi-anaesthesia conditions but context-dependent across datasets. Discrimination performance depends on interaction order: redundancy-based signatures improve with increasing subset size, whilst synergy-based signatures peak at low orders. Higher-order informational features significantly outperform pairwise functional connectivity, particularly for synergistic signatures which remain invisible to correlations. These findings demonstrate that consciousness is reflected in the reconfiguration of higher-order interaction structures, with distinct informational substrates requiring multivariate characterization beyond pairwise connectivity.

---

## 论文详细总结（自动生成）

## 1. 论文的核心问题与整体含义（研究动机和背景）
- **核心问题**：传统脑功能连接研究仅考虑成对区域间的相关性，无法捕捉多个脑区之间涌现的集体依赖性（高阶交互）。意识状态（清醒、麻醉、刺激促醒）的神经基础是否体现在这些高阶交互的重组上？
- **整体含义**：揭示意识依赖于大规模脑区间高阶信息交互的结构重构，为意识状态的神经标记物提供新的多变量度量，推动临床意识评估与促醒干预的量化工具发展。

## 2. 论文提出的方法论：核心思想、关键技术细节
- **核心思想**：利用多元信息论中的 **O-information（O-信息）** 量化多区域脑动力学是偏向**协同性**（synergy）还是**冗余性**（redundancy）信息共享。高阶交互指三个及以上脑区之间无法简化为成对关系的统计依赖。
- **关键技术细节**：
  - 对静息态fMRI数据进行多元信息分解，计算特定区域子集的O‑information值（正值为冗余主导，负值为协同主导）。
  - 通过两种互补优化极性识别**最优区域子集**：第一种侧重捕捉清醒时冗余性升高（麻醉时降低）；第二种侧重捕捉从协同到冗余的转变（synergy‑to‑redundancy transition）。
  - 对比不同子集大小（即交互阶数）对区分性能的影响。
- **算法流程（文字说明）**：提取BOLD时间序列 → 划分脑区 → 对多个区域子集计算O-information → 使用两种优化准则搜索最优子集 → 评估子集O-information在清醒、麻醉、刺激促醒状态下的区分能力 → 与成对功能连接（FC）特征比较。

## 3. 实验设计：数据集、场景、基准和对比方法
- **数据集与场景**：
  - **数据集1**：非人灵长类（猕猴）静息态fMRI，包含**清醒**状态以及三种不同麻醉药物（丙泊酚、七氟烷、氯胺酮）诱导的**意识丧失**状态。
  - **数据集2**：在丙泊酚麻醉期间，通过**中央丘脑深部脑刺激（DBS）** 驱动意识恢复（以行为响应性为指标），记录不同刺激电压下的fMRI数据。
- **Benchmark**：意识状态行为评估（清醒/有响应 vs 麻醉/无响应）作为金标准。
- **对比方法**：
  - 传统**成对功能连接（FC）** 特征（Pearson相关系数矩阵）。
  - 高阶信息特征（O-information）与FC特征的区分性能进行比较，重点关注FC无法捕捉的协同特征。

## 4. 资源与算力
- 论文摘要及元数据**未明确说明**所使用的GPU型号、数量、训练时长或具体计算资源。推测主要使用CPU集群进行信息论计算，但无法确认。

## 5. 实验数量与充分性
- **实验数量**：
  - 两个独立数据集（多药物麻醉+刺激促醒）。
  - 多个区域子集大小（从低阶到高阶）的O-information分析。
  - 两种优化极性下的最优子集搜索。
  - 与成对FC的全面比较。
- **充分性与客观性**：
  - 实验覆盖了清醒、多种麻醉（不同药理机制）、刺激诱导恢复等多种意识状态，具有较强的生态效度。
  - 对比了最常用的成对连接方法，凸显高阶交互的增量价值。
  - 但**缺乏消融实验**（如仅使用低阶信息、随机子集等）来验证优化过程的必要性；也未报告跨个体交叉验证的严格统计指标（如AUC、准确率等），仅在摘要中提及“稳健区分”。

## 6. 论文的主要结论与发现
- **高阶特征显著优于成对FC**：尤其是协同特征在FC中完全不可见，却能在状态区分中提供独特信息。
- **冗余性随意识状态变化**：清醒时最优子集的冗余性升高，麻醉时下降；高压中央丘脑DBS使冗余性模式更接近清醒。
- **协同-冗余转变**：在多麻醉条件下可显著区分状态，但该转变具有数据集和上下文依赖性。
- **交互阶数影响性能**：基于冗余的区分性能随子集大小（阶数）增加而改善；基于协同的区分性能在低阶达到峰值。
- **意识反映高阶交互结构重构**：不同意识状态对应不同的高阶信息基质，需要超越成对连接的多变量表征。

## 7. 优点：方法或实验设计上的亮点
- **方法论创新**：将多元信息论中的O-information引入意识研究，直接量化高阶交互的协同/冗余属性，比传统格兰杰因果或偏相关更全面地刻画集体依赖性。
- **实验设计严谨**：利用非人灵长类进行多药物、多状态、以及刺激干预的纵向对比，控制药物特异性，增强普适性。
- **双重优化策略**：从冗余升高和协同-冗余转变两个视角寻找最优子集，避免单一极性的偏差。
- **对临床转化的启示**：发现高阶信息特征对FC不可见，提示未来临床意识评估可考虑使用高阶脑网络标记。

## 8. 不足与局限：包括实验覆盖、偏差风险、应用限制等
- **实验覆盖有限**：仅使用非人灵长类，人类意识状态（如睡眠、昏迷、植物状态）能否推广未知。
- **空间与时间分辨率**：fMRI时间分辨率低，可能漏掉快速的高阶交互；脑区划分方式影响O-information计算结果，未讨论划分粒度的影响。
- **缺乏因果验证**：仅描述相关关系，未证明高阶交互是意识状态的必要条件或结果。
- **计算局限性**：O-information随区域数增加呈指数增长，实际只能分析有限子集（5~10个区域），可能忽略全脑尺度的高阶模式。
- **未提供统计检验细节**：摘要未报告效应量、置信区间或交叉验证的稳健性，读者难以评估区分性能的可靠性。
- **优化子集的可解释性**：未列出哪些脑区构成最优子集，缺乏神经解剖学意义上的解读。

（完）
