---
title: Comparative single-cell transcriptomic roadmap of mammalian fetal ovarian development
title_zh: 哺乳动物胎儿卵巢发育的比较单细胞转录组图谱
authors: "Fang, Y., Han, S., Zhang, J., Xie, S., Wei, Y., Tang, Y., Duan, J. E."
date: 2026-05-05
pdf: "https://www.biorxiv.org/content/10.64898/2026.05.01.721341v1.full.pdf"
tags: ["query:qll"]
score: 9.0
evidence: 哺乳动物胎儿卵巢发育和颗粒细胞的转录组图谱
tldr: "本研究通过整合牛、人类和小鼠三个物种的107,930个单细胞转录组数据，构建了哺乳动物早期卵巢发育的跨物种图谱。研究识别了11种共有细胞类型，并发现牛特有的类固醇生成细胞群。通过发育轨迹和机器学习分析，揭示了生殖细胞的保守性与颗粒细胞的物种差异性，为理解哺乳动物卵巢发育的保守与进化机制提供了重要框架。"
source: biorxiv
selection_source: fresh_fetch
motivation: 旨在阐明哺乳动物早期卵巢发育的细胞组成和发育动力学在不同物种间的异同。
method: 整合并分析了牛、人类和小鼠在性别决定及早期卵巢分化阶段的逾10万个单细胞转录组数据。
result: 鉴定了11种共有细胞类型及牛特有的细胞群，并发现生殖细胞在转录水平上高度保守，而颗粒细胞表现出显著的物种差异。
conclusion: 该研究为哺乳动物早期卵巢发育提供了比较转录组学框架，揭示了生殖细胞和体细胞谱系发育的保守与特异性机制。
---

## 摘要
早期卵巢发育奠定了女性生殖的细胞基础，但其在不同哺乳动物物种中的细胞组成和发育动态仍缺乏深入表征。在本研究中，我们构建了牛（E38-E112）、人类（PCW6-16）和小鼠（E11.5-E18.5）早期雌性性腺发育的跨物种单细胞转录组图谱，整合了跨越性别决定和早期卵巢分化等可比发育窗口的 107,930 个细胞。我们在三个物种中鉴定了 11 种共有的性腺细胞类型，包括生殖细胞和颗粒细胞，并发现了一个此前未描述的具有类固醇合成特征的牛特异性细胞群，这表明卵巢体细胞谱系发育存在物种差异。表观遗传调节因子在生殖细胞和颗粒细胞中表现出动态激活。发育轨迹分析揭示了与生殖细胞和颗粒细胞发育相关的共有及物种特异性基因，包括生殖细胞中保守的动态表达基因（如 TFAP2C 和 ZCWPW1）以及颗粒细胞中的 FOS 和 JUNB。利用机器学习支持向量机（SVM）模型进行的跨物种细胞类型分类显示，免疫细胞和生殖细胞等细胞类型在转录水平上具有保守性，而颗粒细胞则表现出显著的跨物种差异，这与细胞外基质相关基因的表达有关。总之，我们的研究为理解哺乳动物早期卵巢发育的保守和差异机制提供了一个比较框架。

## Abstract
Early ovarian development establishes the cellular basis of female reproduction, yet its cellular composition and developmental dynamics remain poorly characterized across mammalian species. Here, we generated a cross-species single-cell transcriptomic atlas of early female gonadal development in cattle (E38-E112), human (PCW6-16), and mouse (E11.5-E18.5), integrating 107,930 cells across comparable developmental windows, spanning sex determination and early ovarian differentiation. We identified 11 shared gonadal cell types across three species, including germ cells and granulosa cells, and uncovered a previously undescribed bovine-specific cell population with steroidogenic features, suggesting species differences in ovarian somatic lineage development. Epigenetic regulators exhibited dynamic activation in germ cells and granulosa cells. Developmental trajectory analysis revealed shared and species-specific genes associated with germ cell and granulosa cell development, including conserved dynamically expressed genes such as TFAP2C and ZCWPW1 in germ cells and FOS and JUNB in granulosa cells. Cross-species cell type classification using a machine learning support vector machine (SVM) model revealed transcriptionally conserved cell types, such as immune cells and germ cells, while granulosa cells showed substantial cross-species divergence, associated with extracellular matrix-related gene expression. Together, our study provides a comparative framework for understanding conserved and divergent mechanisms of early ovarian development across mammals.

---

## 论文详细总结（自动生成）

这是一份关于论文《Comparative single-cell transcriptomic roadmap of mammalian fetal ovarian development》（哺乳动物胎儿卵巢发育的比较单细胞转录组图谱）的结构化深入总结：

### 1. 核心问题与整体含义（研究动机和背景）
*   **核心问题**：哺乳动物早期卵巢发育（性别决定及早期分化阶段）在不同物种间的细胞组成、分子调控机制以及发育动力学存在哪些保守性与差异性？
*   **研究背景**：早期性腺发育奠定了雌性生殖的基础。虽然人类、小鼠和家畜（如牛）的单物种研究已有进展，但由于发育时间轴不一致、技术批次效应以及缺乏统一的分析框架，跨物种的系统性比较一直难以实现。
*   **研究意义**：通过构建跨物种图谱，不仅能揭示生殖细胞发育的通用规律，还能识别导致物种间生殖策略差异的特异性因素，对人类生殖健康、畜牧业生产及发育生物学具有重要价值。

### 2. 论文提出的方法论
*   **核心思想**：通过整合新生成的牛（Bovine）数据与已发表的人类和小鼠数据，利用同源基因映射和机器学习模型，在统一的转录组空间内量化物种间的细胞相似性。
*   **关键技术细节**：
    *   **数据整合**：基于Ensembl的1:1同源基因（共16,073个）进行跨物种整合。
    *   **拟时序分析（Pseudotime）**：使用 `Monocle3` 重建生殖细胞和颗粒细胞的发育轨迹。
    *   **转录调控网络**：利用 `pySCENIC` 推断转录因子（TF）及其靶基因的调控活性（Regulons）。
    *   **细胞通讯**：使用 `CellChat` 分析配体-受体对，表征生殖细胞与体细胞间的相互作用。
    *   **SVM分类模型**：训练线性支持向量机（SVM）模型，以人类数据为基准预测鼠和牛的细胞类型，通过预测概率量化细胞类型的转录保守性。

### 3. 实验设计
*   **数据集/场景**：
    *   **牛（Bovine）**：新生成的scRNA-seq数据，涵盖E38至E112共6个阶段。
    *   **人类（Human）**：PCW6至PCW16共6个阶段。
    *   **小鼠（Mouse）**：E11.5至E18.5共5个阶段。
*   **分析基准（Benchmark）**：以人类已知的性腺细胞类型标记基因和发育阶段作为主要参考基准。
*   **对比维度**：
    *   11种共有细胞类型的分布与比例。
    *   生殖细胞从多能性到减数分裂的基因表达动态。
    *   颗粒细胞分化过程中的物种特异性通路。

### 4. 资源与算力
*   **测序平台**：使用了10x Genomics（MobiCube/MobiNova系统）进行单细胞文库构建，Illumina NovaSeq进行测序。
*   **算力说明**：文中**未明确说明**具体的GPU型号、数量或训练时长。分析主要依赖于R（Seurat, Monocle3）和Python（pySCENIC）环境下的生物信息学标准流程。

### 5. 实验数量与充分性
*   **实验规模**：整合了总计**107,930个**高质量单细胞，涵盖了三个物种的关键发育窗口。
*   **充分性评价**：
    *   **样本覆盖**：涵盖了性别决定、有丝分裂扩张、减数分裂起始等关键生物学事件，时间点设置合理。
    *   **分析深度**：除了常规的聚类分析，还深入到了表观遗传调节因子动态、转录因子调控网络以及机器学习分类预测，实验维度非常丰富。
    *   **客观性**：通过下采样（Downsampling）和自助法（Bootstrapping）训练SVM模型，确保了跨物种比较的统计稳健性。

### 6. 主要结论与发现
*   **细胞类型鉴定**：识别出11种跨物种共有的细胞类型，并发现了一个**牛特有的类固醇生成细胞群**（表达 *CYP17A1* 和 *HSD3B1*），这在人、鼠胎儿卵巢中未见类似群体。
*   **生殖细胞保守性**：生殖细胞的发育轨迹在三个物种中高度保守，共同经历多能性基因（*POU5F1*, *NANOG*）下调和减数分裂基因（*SYCP1*, *ZCWPW1*）上调。
*   **颗粒细胞差异性**：颗粒细胞在物种间表现出显著的转录分歧。SVM预测显示其保守性最低，差异主要集中在**细胞外基质（ECM）**相关基因（如牛的 *LAMA2*, *MMP14*）。
*   **调控因子**：识别出 *FOS* 和 *JUNB* 是颗粒细胞发育中保守的调控因子，而 *PBX1* 在牛的生殖细胞和颗粒细胞中均表现出特异的高活性。

### 7. 优点（亮点）
*   **跨物种视角**：首次将牛这一重要家畜纳入人、鼠的比较框架，填补了大型哺乳动物早期卵巢发育单细胞图谱的空白。
*   **量化比较**：引入SVM机器学习模型，将定性的细胞类型观察转化为定量的“保守性得分”，增强了结论的说服力。
*   **多维度解析**：结合了转录组、表观调控推断和细胞通讯，提供了全方位的发育路线图。

### 8. 不足与局限
*   **基因覆盖限制**：分析仅限于1:1同源基因，忽略了物种特异性基因、非编码RNA或基因家族扩增对发育的贡献。
*   **发育阶段对齐**：虽然选择了可比的时间窗口，但不同物种的发育速率和采样间隔仍存在细微差异，可能导致某些瞬时细胞状态的遗漏。
*   **验证手段单一**：研究主要基于生物信息学推断，缺乏原位杂交（ISH）或免疫荧光（IF）等空间层面的实验验证，尤其是对牛特有细胞群的空间定位。
*   **功能验证缺失**：识别出的物种特异性调控因子（如牛的 *PBX1*）尚未通过功能缺失或过表达实验进行生物学功能验证。

（完）
