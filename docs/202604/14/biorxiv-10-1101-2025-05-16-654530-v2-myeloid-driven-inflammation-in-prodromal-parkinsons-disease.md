---
title: "Myeloid-Driven Inflammation in Prodromal Parkinson's Disease"
title_zh: 前驱期帕金森病中髓系细胞驱动的炎症
authors: "Yasumizu, Y., Deerhake, M. E., Moon, J., Buitrago-Pocasangre, N., Russo, A., Wang, H., Zhu, B., Seibyl, J. P., Reddy, V., Wang, Q., Neish, K. J., Spillantini, M. G., Posner, D. A., Clatworthy, M., Sumida, T. S., Longbrake, E. E., Cedarbaum, J. M., Zhang, L., Hafler, D. A."
date: 2026-04-14
pdf: "https://www.biorxiv.org/content/10.1101/2025.05.16.654530v2.full.pdf"
tags: ["query:slp-ns"]
score: 9.0
evidence: 快速眼动睡眠行为障碍作为帕金森病前驱症状
tldr: 本研究探讨了前驱期帕金森病（PD）的炎症机制，假设其起源于肠道并演变为神经退行性病变。通过对118名受试者（包括健康对照、前驱期PD、确诊PD及多发性硬化症患者）的脑脊液和血液进行单细胞RNA测序，发现前驱期PD患者脑脊液中免疫细胞显著增多，特别是具有JAK-STAT和TNF信号特征的小胶质细胞样巨噬细胞。研究还揭示了肠道与中枢神经系统之间存在免疫关联，为PD的早期干预提供了新靶点。
source: biorxiv
selection_source: fresh_fetch
motivation: 验证前驱期帕金森病是否为一种由肠道引发并演变为神经退行性过程的炎症性疾病。
method: 对118名受试者的脑脊液和血液样本进行单细胞RNA测序分析，并结合PD小鼠模型进行跨组织转录组对比。
result: 发现前驱期PD患者脑脊液中存在特异性促炎巨噬细胞，且肠道与中枢神经系统之间存在共享的记忆T细胞克隆。
conclusion: 研究揭示了前驱期PD中由髓系细胞介导的TNF炎症过程，并证实了肠道与中枢神经系统之间的免疫联系。
---

## 摘要
我们假设以前驱期帕金森病（PD）为特征的快速眼动睡眠行为障碍和嗅觉减退，是一种始于肠道的炎症性疾病，随后演变为表现为经典PD的神经退行性过程。为了验证这一假设，我们对118名受试者的脑脊液（CSF）和血液进行了单细胞RNA测序分析，并将健康受试者、前驱期PD患者和显性PD患者与中枢神经系统（CNS）自身免疫性疾病多发性硬化症（MS）患者进行了比较。令人惊讶的是，我们发现前驱期PD患者脑脊液中的免疫细胞数量有所增加。单细胞RNA测序显示，在前驱期PD中，脑脊液特异性小胶质细胞样巨噬细胞增多，且具有增强的JAK-STAT和TNF信号特征。脑脊液巨噬细胞表现出与表达α-突触共核蛋白的PD模型小鼠的硬脑膜巨噬细胞和肠肌层巨噬细胞相似的转录谱。最后，在人类的肠道和脑脊液T细胞之间发现了共享的记忆T细胞克隆。这些发现揭示了前驱期PD患者中枢神经系统中由髓系细胞介导的TNF炎症过程，并表明肠道与中枢神经系统之间存在免疫学联系。

## Abstract
We hypothesized that prodromal Parkinson's Disease (PD), characterized by REM Sleep Behavior Disorder and hyposmia, is an inflammatory disorder initiated in the gut that evolves into a neurodegenerative process manifest as classical PD. To test this hypothesis, we performed single-cell RNAseq analysis of cerebrospinal fluid (CSF) and blood from 118 individuals, comparing healthy subjects with prodromal PD and manifest PD to patients with the central nervous system (CNS) autoimmune disease, multiple sclerosis (MS). Surprisingly, we identified increased numbers of immune cells in the CSF of patients with prodromal PD. Single-cell RNA sequencing revealed increases in CSF-specific microglia-like macrophages with enhanced JAK-STAT and TNF signaling signatures in prodromal PD. CSF macrophages exhibited similar transcriptional profiles to dural macrophages and gut muscularis macrophages from -synuclein-expressing PD model mice. Finally, shared memory T cell clones were found in humans between gut and CSF T cells. These findings uncover a myeloid-mediated TNF inflammatory process in the CNS of patients with prodromal PD, with an immunological linkage between the gut and the CNS.

---

## 论文详细总结（自动生成）

这是一份关于论文《Myeloid-Driven Inflammation in Prodromal Parkinson’s Disease》（前驱期帕金森病中髓系细胞驱动的炎症）的结构化深入总结：

### 1. 核心问题与整体含义
该研究探讨了**帕金森病（PD）在临床症状出现前的“前驱期”是否存在免疫炎症机制**。长期以来，PD被视为一种原发性的神经退行性疾病，但研究者假设：PD实际上是一种由肠道引发、随后演变为中枢神经系统（CNS）病理过程的炎症性疾病。研究重点在于揭示快速眼动睡眠行为障碍（RBD，PD的重要前驱症状）患者脑脊液中的免疫改变，以寻找早期干预的生物标志物和治疗靶点。

### 2. 方法论
*   **核心思想**：利用单细胞多组学技术，对比分析前驱期PD、确诊PD、健康对照以及自身免疫性疾病（多发性硬化症，MS）患者的免疫图谱，寻找PD特异性的炎症特征。
*   **关键技术细节**：
    *   **单细胞测序**：对配对的外周血单核细胞（PBMC）和脑脊液（CSF）细胞进行单细胞RNA测序（scRNA-seq）及VDJ测序（TCR/BCR）。
    *   **细胞频率分析**：采用 **scCODA**（一种基于贝叶斯模型的统计工具）来评估不同疾病组间细胞比例的显著差异。
    *   **细胞通讯分析**：使用 **CellPhoneDB** 预测免疫细胞间的配体-受体相互作用。
    *   **遗传学整合**：利用 **scDRS** 将全基因组关联研究（GWAS）的遗传风险评分整合到单细胞数据中，以识别受遗传影响最显著的细胞群体。
    *   **跨组织/物种对比**：将人类数据与PD小鼠模型（MI2BAC）的硬脑膜及肠道巨噬细胞转录组进行整合对比。

### 3. 实验设计
*   **数据集与受试者**：共招募118名受试者，分为五组：RBD（36人）、PD（15人）、PD-RBD（18人）、多发性硬化症（MS，27人）及健康对照（HC，22人）。
*   **Benchmark（基准）**：以年龄匹配的健康受试者为基准，同时以MS作为“T细胞介导的典型CNS自身免疫炎症”对照。
*   **对比维度**：
    *   **组织维度**：血液 vs 脑脊液 vs 肠道。
    *   **疾病维度**：前驱期 vs 确诊期；神经退行性炎症（PD） vs 自身免疫性炎症（MS）。
    *   **物种维度**：人类患者数据 vs $\alpha$-突触共核蛋白转基因小鼠模型。

### 4. 资源与算力
论文中**未明确说明**具体的硬件算力（如GPU型号、数量）或训练时长。分析主要依赖于标准的生物信息学流程（如10x Genomics Chromium平台、Seurat、Scanpy等），这类分析通常在高性能计算集群（HPC）上完成，而非大规模深度学习训练。

### 5. 实验数量与充分性
*   **实验规模**：分析了超过78万个单细胞（PBMC 52万+，CSF 26万+），样本量在单细胞临床研究中属于较大规模。
*   **充分性**：研究不仅观察了细胞数量变化，还深入到了基因通路（Hallmark通路分析）、细胞间通讯、遗传风险关联以及跨物种验证。
*   **客观性**：通过引入MS作为对照组，成功区分了“髓系驱动”与“淋巴系驱动”的两种截然不同的CNS炎症模式，实验设计逻辑严密且具有互补性。

### 6. 主要结论与发现
*   **前驱期炎症显著**：RBD患者脑脊液中的免疫细胞数量显著增加，甚至高于确诊后的PD患者。
*   **特异性巨噬细胞**：鉴定出一种**CSF特异性小胶质细胞样巨噬细胞（CSF Mac）**，在前驱期PD中显著扩增，并表现出强烈的 **TNF$\alpha$** 和 **IL6-JAK-STAT3** 信号特征。
*   **与MS的差异**：在MS中，这种CSF巨噬细胞反而减少，且缺乏TNF信号，证明了PD炎症机制的独特性。
*   **肠-脑轴证据**：在人类肠道组织和脑脊液中发现了**共享的记忆T细胞克隆**；同时，PD小鼠的肠道巨噬细胞也表现出与人类CSF巨噬细胞相似的TNF炎症特征。

### 7. 优点
*   **视角前瞻**：首次在单细胞水平上系统描绘了PD前驱期的CNS免疫景观。
*   **机制突破**：挑战了“PD炎症仅是神经退行性变继发反应”的传统观点，提出了髓系细胞驱动的早期致病模型。
*   **临床关联强**：通过流行病学数据（如抗TNF治疗降低PD风险）与实验数据的结合，为抗TNF疗法进入PD临床试验提供了直接证据。

### 8. 不足与局限
*   **因果关系尚需验证**：虽然发现了肠道与脑部的免疫联系，但仍无法绝对断定炎症是诱发$\alpha$-突触共核蛋白聚集的“第一推动力”。
*   **纵向数据缺失**：该研究为横断面研究，未能追踪同一批RBD患者从炎症发作到最终转化为PD的完整动态过程。
*   **样本异质性**：RBD患者群体本身具有高度异质性，部分患者可能转化为路易体痴呆（DLB）而非PD，这可能对结果产生一定干扰。

（完）
