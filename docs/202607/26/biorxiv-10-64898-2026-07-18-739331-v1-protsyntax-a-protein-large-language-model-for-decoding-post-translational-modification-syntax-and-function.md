---
title: "ProtSyntax: a protein large language model for decoding post-translational modification syntax and function"
title_zh: ProtSyntax：一个用于解码翻译后修饰语法和功能的蛋白质大语言模型
authors: "Lin, Y."
date: 2026-07-21
pdf: "https://www.biorxiv.org/content/10.64898/2026.07.18.739331v1.full.pdf"
tags: ["query:qll"]
score: 8.0
evidence: 适用于研究衰老和纤维化中翻译后修饰的PTM预测模型
tldr: "翻译后修饰(PTM)依赖残基化学、序列上下文、三维微环境和修饰状态，但现有模型孤立预测位点，未连接修饰倾向与功能后果。ProtSyntax采用稀疏混合专家架构和几何门控注意力，以自适应多目标学习耦合位点级PTM语法与蛋白级功能。在40个PTM基准上平均MCC和AP分别提升12.7%和10.7%，且能区分真实位点、迁移至稀有PTM、恢复串扰和识别疾病关联。该模型提供了可解释框架，用于解码全蛋白组PTM调控。"
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-18-739331-v1/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1538, \"height\": 1169, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-18-739331-v1/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1558, \"height\": 1204, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-18-739331-v1/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1477, \"height\": 1714, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-18-739331-v1/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1511, \"height\": 1427, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-18-739331-v1/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1509, \"height\": 1749, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-18-739331-v1/fig-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 1511, \"height\": 1663, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-18-739331-v1/fig-007.webp\", \"caption\": \"\", \"page\": 0, \"index\": 7, \"width\": 1505, \"height\": 1173, \"label\": \"Figure\"}]"
tables_json: "[{\"url\": \"assets/tables/biorxiv/biorxiv-10-64898-2026-07-18-739331-v1/table-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1501, \"height\": 1255, \"label\": \"Table\"}, {\"url\": \"assets/tables/biorxiv/biorxiv-10-64898-2026-07-18-739331-v1/table-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1528, \"height\": 1101, \"label\": \"Table\"}]"
motivation: 现有PTM预测模型孤立处理位点，缺乏对激酶特异性、串扰和动力学的联合建模，无法连接修饰倾向与功能后果。
method: ProtSyntax以双向长程建模和几何门控注意力为核心，采用稀疏混合专家架构，在400万样本上通过自适应多目标学习联合优化位点和蛋白级目标。
result: "在40个基准上平均MCC和AP提升12.7%和10.7%，有效区分真实位点与诱饵，迁移至稀有PTM并恢复串扰，关联酶动力学与疾病突变。"
conclusion: ProtSyntax为解码全蛋白组中PTM的调控语法和功能提供了可解释的框架。
---

## 摘要
翻译后修饰（PTMs）通过残基化学性质、序列上下文、三维微环境和修饰状态之间的依赖关系调节蛋白质功能，然而大多数预测器独立地建模位点，并未将修饰倾向性与功能结果联系起来。本文提出ProtSyntax，一个以PTM为中心的蛋白质语言模型，在涵盖40种PTM类别的425万个样本上训练，并针对激酶特异性、PTM串扰和酶动力学进行了监督学习。ProtSyntax在稀疏混合专家架构中集成了双向长程建模与几何门控注意力，并使用自适应多目标学习将残基水平的PTM语法与蛋白质水平的功能耦合。在40个PTM位点基准测试中，相对于最佳基线模型，ProtSyntax的平均MCC和AP分别提高了12.7%和10.7%。它还能区分真实位点与结构不兼容的基序诱饵、迁移到稀有PTM、恢复串扰、将PTM扰动与酶动力学变化联系起来，并识别疾病相关的PTM失调。总之，ProtSyntax为解码整个蛋白质组中的PTM调控提供了一个可解释的框架。

## Abstract
Post-translational modifications (PTMs) regulate protein function through dependencies among residue chemistry, sequence context, three-dimensional microenvironments and modification states, yet most predictors model sites independently and do not connect modification propensity to functional consequences. Here we present ProtSyntax, a PTM-centered protein language model trained on 4.25 million examples spanning 40 PTM classes and supervised for kinase specificity, PTM crosstalk and enzyme kinetics. ProtSyntax integrates bidirectional long-range modeling with geometry-gated attention in a sparse mixture-of-experts architecture and uses adaptive multi-objective learning to couple residue-level PTM syntax to protein-level function. Across 40 PTM-site benchmarks, ProtSyntax improved mean MCC and AP by 12.7% and 10.7%, respectively, relative to the best-performing baselines. It also distinguished authentic sites from structurally incompatible motif decoys, transferred to rare PTMs, recovered crosstalk, linked PTM perturbations to enzyme-kinetic changes and identified disease-associated PTM disruptions. Together, ProtSyntax provides an interpretable framework for decoding PTM regulation across the proteome.

---

## 论文详细总结（自动生成）

# 论文总结：ProtSyntax

## 1. 核心问题与整体含义
- **研究动机**：翻译后修饰（PTM）调控蛋白质功能，但现有预测模型大多将每个位点视为独立分类目标，忽略了残基化学、序列上下文、三维微环境和修饰状态之间的层级依赖关系，也无法将修饰倾向性与蛋白质功能后果联系起来。
- **整体含义**：本文提出将PTM调控视为一种蛋白质语言——残基是字母，基序和三维微环境定义语法，组合修饰状态编码上下文依赖的调控意义。ProtSyntax旨在学习这种“PTM语法”，从而实现从位点预测到修饰功能推断的跨越。

## 2. 方法论
- **核心思想**：构建一个以PTM为中心的大语言模型，通过联合学习PTM位点、激酶特异性、串扰和酶动力学，在统一表示空间中耦合残基级语法和蛋白级功能。
- **关键技术细节**：
  - **稀疏混合专家（MoE）架构**：包含16个专家，Top‑2路由，总参数约4B，每token激活约1B参数。
  - **Bio‑RoPE**：PTM感知的位置编码，将相位分解为结构周期性通道（对应不同二级结构周期）、物理化学通道（引入残基特性偏移）和标准长程旋转通道，使模型编码基序顺序与化学兼容性。
  - **Bi‑Gated DeltaNet**：双向长程语法传播模块。使用两个独立Gated DeltaNet核心分别沿N→C和C→N方向扫描，通过零参数交叉门控融合两个方向状态，强化双向证据一致的残基，抑制局部偶然基序。
  - **Geometric Gated Attention（GGA）**：结构约束注意力模块。将残基框架下的3D探针点距离作为几何惩罚项注入注意力logits，使模型区分序列兼容但结构不容许的微环境。
  - **PACE‑Nash损失**：自适应多目标优化。结合非对称焦点分类、相关性对比学习、不确定性感知的动力学回归、物理化学流形正则化，并通过纳什议价动态协调各任务权重。
- **训练流程**：输入来自冻结的ESM‑C和SaProt嵌入，以及AlphaFold2预测的残基几何特征；经过共享编码器后，多个任务头分别输出PTM分类、激酶特异性、串扰和动力学参数。

## 3. 实验设计
- **数据集**：
  - 通用PTM：348,903正样本、3,902,925化学生成负样本，涵盖40类PTM，55残基窗口。
  - 激酶特异性磷酸化：4类（CDK、AGC、PKC、MAPK），3,803正样本。
  - PTM串扰：262正样本（基于DeepPCT扩展）。
  - 酶动力学：CatPred‑DB（77,020条记录，含Kcat、Km、Ki）。
  - 低资源PTM：留出8种稀有类型（如乳酸化、甲酰化等）。
- **基准场景**：
  - 40类通用PTM位点预测。
  - 4类激酶特异性磷酸化预测。
  - PTM串扰预测。
  - 酶动力学回归（R²和MAE）。
  - 五类语法验证实验：Cloze恢复、结构诱饵区分、低资源迁移（0/10/50样本）、串扰重建、PTM‑功能链接。
  - 疾病案例：突变效应（ClinVar/COSMIC vs gnomAD）、液‑液相分离、阿尔茨海默通路PTM图谱、胶质母细胞瘤耐药干预轴。
- **对比方法**：
  - 通用PTM：PTMGPT2、PTM‑Mamba、MTPrompt‑PTM、AstraPTM2。
  - 激酶特异性：DCPPS。
  - 串扰：DeepPCT、ProXTalk。
  - 动力学：CatPred。
  - 消融：去除各模块（Bio‑RoPE、Bi‑Gated DeltaNet、GGA、PACE‑Nash）的变体。

## 4. 资源与算力
- 训练使用**24张NVIDIA H100 GPU**集群（Methods 4.4节）。
- 推理可在H100、A100、5090、4090等GPU上运行。
- 模型参数量约4B，激活参数约1B。
- **未明确说明训练时长**，仅提到优化器为AdamW，峰值学习率4e⁻⁴，5,000预热步，batch size 256或512。

## 5. 实验数量与充分性
- **大量实验**：包括40类PTM的全量基准、4类激酶任务、串扰任务、动力学回归、5类语法验证实验、3类消融（模块级）、鲁棒性（pLDDT分层、不同结构生成器）、低资源迁移、疾病案例等。
- **充分性评估**：实验设计较为全面，覆盖了性能、泛化、可解释性和应用场景。
- **公平性**：所有基线使用匹配的数据划分和评价协议（如CD‑HIT 50%序列去冗余、随机种子划分8:1:1），但需注意某些基线（如PTMGPT2）可能未在所有任务上重新训练，而是引用原论文结果（文中未详细说明，但声称采用匹配协议）。
- **客观性**：评价指标选择MCC、AP、AUC、R²、MAE等标准指标，无过度拟合报告。

## 6. 主要结论与发现
- 在40类PTM基准上，ProtSyntax的平均MCC和AP分别比最佳基线提升**12.66%**和**10.67%**。
- 在激酶特异性、串扰、动力学任务上也一致优于对比方法（MCC+9.24%、AP+9.71%等）。
- 能成功进行**PTM语法学习**：Cloze恢复准确率0.842、结构诱饵配对排名准确率0.887、低资源零样本AUPRC 0.432（10样本即升至0.611）。
- 恢复91%实验验证的串扰关系；在酶动力学中，ΔPTM分数与Δlog Kcat的Spearman ρ达0.628。
- 疾病变异识别AUROC 0.885；在FUS相分离模拟中捕捉到非线性阈值效应。
- 阿尔茨海默通路PTM图谱覆盖383个蛋白、86,219个高分位点，重现已知修饰。

## 7. 优点
- **生物学驱动的架构设计**：四个模块（Bio‑RoPE、Bi‑Gated DeltaNet、GGA、PACE‑Nash）均对应PTM语法的不同层级，具有明确可解释性。
- **多任务统一学习**：将PTM分类、串扰、动力学回归联合训练，迫使表示空间同时编码语法和功能，提升迁移能力。
- **广泛的验证体系**：不仅报告标准基准，还设计了多种“语法测试”（cloze、结构诱饵、低资源迁移等），证实模型学到了真正的调控规则而非简单模式匹配。
- **开源可复现**：代码、数据集、模型权重均在Hugging Face和GitHub公开，并提供Web界面ProtSyntax Lab。
- **计算效率**：采用MoE激活稀疏性，推理速度最快（文中提及）。

## 8. 不足与局限
- **数据偏差**：训练集依赖现有实验注释，对稀有、瞬时、条件特异性PTM覆盖不足，可能引入偏向常见PTM的归纳偏差。
- **结构依赖**：依赖AlphaFold2等预测的静态构象，无法完全表示构象集合、酶‑底物遭遇态或高度动态环境（如固有无序区），降低结构模糊区域的可靠性。
- **功能连接有限**：当前仅通过酶动力学监督和计算机模拟连接语法与功能，未直接建模PTM占用率、时间信号动态、蛋白质形式多样性或细胞类型特异性调控。
- **评估局限性**：部分消融实验仅在磷酸化数据集上进行，结论推广需谨慎；疾病案例数量有限，仅为概念验证。
- **未比较同类基底模型**：与PTMGPT2等专用模型相比，ProtSyntax是专门从零训练的PTM模型，而非在通用蛋白质语言模型上微调，因此对比可能不直接体现结构级优势。

（完）
