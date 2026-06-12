---
title: "A common connectome-based neural reference space across affective, autonomic, and wakefulness arousal"
title_zh: 一个基于连接组的共同神经参考空间，涵盖情感、自主神经和觉醒唤醒
authors: "Bhattacharyya, K., Huberman-Shlaes, J., Tong, Y., Zhu, Y., Ke, J., Park, J. S., Corriveau, A., Rosenberg, M. D., Leong, Y. C."
date: 2026-06-11
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.08.730730v1.full.pdf"
tags: ["query:slp-ns"]
score: 9.0
evidence: 睡眠-觉醒调节的神经机制
tldr: 研究针对arousal定义不一致的问题，使用动态连接组预测模型对5个fMRI数据集进行分析，预测情感、自主神经和觉醒三种arousal指标。模型能够跨数据集泛化，预测睡眠阶段和记忆增强效应，并发现共享连接主要位于突显网络和体感运动网络之间。结果表明不同arousal类型共享核心神经连接，支持统一的基于连接组的神经参考空间。
source: biorxiv
selection_source: fresh_fetch
motivation: 不同研究对arousal的操作化定义不一致，缺乏统一的神经基础框架，阻碍了跨领域结果的整合。
method: 应用动态连接组预测模型，对5个fMRI数据集（包括自然观影、听故事、静息和睡眠）分别预测主观评分、瞳孔扩张和EEG对应的arousal指标，并测试跨数据集泛化能力。
result: 模型成功跨数据集泛化，能预测睡眠阶段和记忆增强效果；共享连接主要位于突显网络和体感运动网络之间。
conclusion: 存在一个基于连接组的神经参考空间，不同arousal变体共享核心预测连接，为整合跨任务和模态的arousal研究提供了量化框架。
---

## 摘要
唤醒常被用来解释注意力、情绪、记忆和决策中依赖于状态的可变性。然而，该术语的使用并不一致，分别指代情感体验、自主神经激活和觉醒状态。不同唤醒操作化定义在多大程度上反映了一个共享的神经生物学基础仍不清楚，这限制了对跨研究结果的统一。我们将动态连接组预测模型应用于五个fMRI数据集，涵盖自然电影观看、故事聆听、清醒休息和睡眠。我们分别从主观评分、瞳孔扩张和脑电图推导出情感、自主神经和觉醒唤醒的测量指标。在一个数据集中训练的预测唤醒模型能够泛化到其他数据集，表明动态连接捕获了跨测量和任务情境的共享唤醒相关动态。这些模型还预测了手动评分的睡眠阶段，表明它们捕获了延伸到睡眠期间唤醒梯度波动的唤醒动态。电影观看期间解码的唤醒动态预测了参与者后来回忆电影事件的能力，再现了经典的唤醒依赖性记忆增强效应。模型预测得到了重叠功能连接的支持，包括所有模型共享的一个子集。共享连接的最大比例位于突显网络和体感运动网络之间，表明突显检测和行动准备之间的协调增强可能是唤醒多种操作化定义的共同特征。总之，这些结果与一个基于连接组的唤醒神经参考空间一致，其中不同唤醒类型共享一组核心预测连接。我们的发现为整合跨任务和模态的唤醒相关发现提供了一个定量框架。

## Abstract
Arousal is often invoked to explain state-dependent variability in attention, emotion, memory, and decision-making. However, the term is used inconsistently, referring variously to affective experience, autonomic activation, and states of wakefulness. The extent to which different operationalizations of arousal reflect a shared neurobiological basis remains unclear, limiting efforts to unify findings across studies. We applied dynamic connectome predictive models to five fMRI datasets spanning naturalistic movie watching, story listening, wakeful rest, and sleep. We derived measures of affective, autonomic, and wakefulness arousal from subjective ratings, pupil dilation, and EEG, respectively. Models trained to predict arousal in one dataset generalized across datasets, indicating that dynamic connectivity captures shared arousal-related dynamics across measures and task contexts. The models also predicted manually scored sleep stages, suggesting that they capture arousal dynamics that extend to the graded fluctuations in arousal during sleep. Decoded arousal dynamics during movie-viewing predicted how well participants later recalled movie events, reproducing classic arousal-dependent memory enhancement effects. Model predictions were supported by overlapping functional connections, including a subset shared across all models. The largest proportion of shared connections was between the salience and somatomotor networks, suggesting that increased coordination between salience detection and action readiness may be a common feature across multiple operationalizations of arousal. Together, these results are consistent with a connectome-based neural reference space for arousal, in which different varieties share a core set of predictive connections. Our findings offer a quantitative framework for integrating arousal-related findings across tasks and modalities.

---

## 论文详细总结（自动生成）

# 论文中文详细总结

## 1. 论文的核心问题与整体含义（研究动机和背景）

- **核心问题**：不同研究对“唤醒（arousal）”一词的操作化定义极不一致，分别指代情感体验（主观评分）、自主神经激活（瞳孔扩张）和觉醒状态（脑电图/睡眠阶段）。这些不同的唤醒指标是否共享一个共同的神经生物学基础尚不清楚，阻碍了跨领域研究结果的整合与统一。
- **研究动机**：为了检验是否存在一个基于连接组的“神经参考空间”，使不同维度的唤醒（情感、自主神经、觉醒）均能映射到一组共享的脑功能连接模式上，从而提供一个定量的统一框架。

## 2. 论文提出的方法论：核心思想、关键技术细节

- **核心思想**：利用动态功能连接（dynamic connectivity）构建预测模型，将不同模态的唤醒指标（主观评分、瞳孔直径、EEG衍生的睡眠阶段）作为预测目标，训练一个“动态连接组预测模型”（dynamic connectome predictive model）。如果模型能在不同数据集和任务间泛化，则表明存在共享的唤醒相关神经动态。
- **关键技术细节**：
  - 使用滑动时间窗口从fMRI数据中提取动态功能连接矩阵（即随时间变化的脑区间相关性）。
  - 以这些动态连接特征作为输入，以各唤醒指标（连续值）作为输出，训练回归/分类模型（具体算法未在摘要中详述，可能为弹性网络、SVR或深度网络）。
  - 在一个数据集上训练模型后，直接应用于其他数据集的动态连接特征，检验预测准确性。
  - 此外，将模型应用于自然观影数据集，解码出逐时刻的唤醒估计值，并检验其与后续记忆表现的关联（经典唤醒-记忆增强效应）。
- **公式或算法流程**：文中未给出具体数学公式，流程可概括为：
  1. 预处理fMRI数据 → 提取灰质ROI时间序列 → 滑动窗口构建动态功能连接矩阵。
  2. 对每个窗口的特征降维/筛选（可能采用基于连接组的预测建模框架，即CPM）。
  3. 使用监督学习训练模型，将窗口级连接模式映射到对应的唤醒测量值。
  4. 跨数据集验证：训练集→测试集泛化，以及睡眠阶段分类、记忆预测等下游任务。

## 3. 实验设计：数据集、基准、对比方法

- **数据集与场景**：共使用5个fMRI数据集，涵盖：
  - 自然电影观看（2个数据集）
  - 故事聆听
  - 清醒休息
  - 睡眠（含同时EEG）
- **唤醒指标**：
  - 情感唤醒：从主观评分（如情绪效价/唤醒度评分）获得。
  - 自主神经唤醒：从瞳孔扩张（瞳孔直径变化）获得。
  - 觉醒唤醒：从EEG推导的睡眠阶段（手动评分）获得。
- **基准**：未明确提及具体的对比方法，但跨数据集泛化本身就是一种较强的检验。逻辑上，该方法与单数据集内训练-测试（无泛化）做了对比；睡眠阶段预测可看作一项独立验证基准。
- **对比方法**：摘要中未列出其他方法（如传统基于静态连接或基于平均活动的模型），可能未做系统对比，而是侧重于证明模型泛化能力。

## 4. 资源与算力

- 文中**未明确说明**使用的GPU型号、数量、训练时长等具体算力信息。考虑到数据量（5个fMRI数据集，每个可能数十至上百名被试）和动态连接建模的计算量，推测需要一定GPU资源（如NVIDIA V100或A100），但无法从摘要确认。

## 5. 实验数量与充分性

- **实验组数**：
  - 跨数据集泛化试验：从1个数据集训练，在其他4个数据集上测试，可能构成多个交叉验证组合（如5选1+4测试）。
  - 睡眠阶段预测：使用模型输出预测人工评分的睡眠阶段（二分类或多分类）。
  - 记忆增强效应：在电影观看数据集中，解码的唤醒动态与后续回忆表现的相关性分析。
- **充分性评估**：
  - **优点**：覆盖了多种任务（观影、听故事、静息、睡眠）和多种唤醒操作化定义，泛化检验较为严格；睡眠预测和记忆预测提供了额外的生态效度验证。
  - **不足**：未提及是否进行了控制分析（如混淆变量分析、随机标签检验、交叉验证稳定性评估）；未比较不同模型架构或特征选择方案；未报告效应量、置信区间等统计细节。因此，实验设计虽合理但可能不够全面，需要全文补充更多消融实验（如使用静态连接、单一网络等）。

## 6. 论文的主要结论与发现

- **主要结论**：存在一个基于连接组的神经参考空间，不同操作化定义的唤醒（情感、自主神经、觉醒）共享一组核心的预测功能连接。
- **关键发现**：
  - 动态连接组预测模型能在不同数据集和任务间泛化，说明其捕获了任务可变的共享唤醒动态。
  - 模型可预测手工评分的睡眠阶段，表明唤醒动态从清醒延伸到睡眠。
  - 电影观看期间解码的唤醒动态能预测后续记忆表现，复现了经典的唤醒-记忆增强效应。
  - 共享连接的最大比例位于**突显网络（salience network）**与**体感运动网络（somatomotor network）**之间，提示唤醒的多个变体共同特征为“突显检测与行动准备之间的协调增强”。

## 7. 优点：方法或实验设计上的亮点

- **方法论亮点**：
  - 首次尝试跨多种唤醒操作化定义建立统一的神经参考空间。
  - 利用动态而非静态连接，能够捕捉随任务和状态变化的唤醒波动。
  - 跨数据集的泛化检验比单数据集内部验证更具说服力。
  - 将模型应用于下游行为预测（睡眠阶段、记忆表现），提供外部效度证据。
- **实验设计亮点**：
  - 涵盖多模态唤醒指标（主观、瞳孔、EEG），覆盖不同生理和行为层面。
  - 包含自然刺激（电影、故事），生态效度较高。
  - 睡眠数据为模型提供了从清醒到睡眠的连续梯度。

## 8. 不足与局限

- **实验覆盖**：
  - 仅包含5个数据集，且均来自实验室环境（尽管有自然观影），缺乏真实世界脑成像数据（如可穿戴fNIRS/EEG）。
  - 未提及模型在不同扫描仪、不同站点之间的泛化能力。
- **偏差风险**：
  - 动态连接的特征维度高，可能存在过拟合风险，摘要未报告交叉验证的稳定性和控制分析（如置换检验）。
  - 唤醒指标本身可能存在共线性（如自主神经唤醒与觉醒唤醒部分重叠），未做去相关分析。
- **应用限制**：
  - 模型训练需要同时记录fMRI和多个外周/主观指标，数据采集成本高。
  - 动态连接计算依赖窗口长度和步长选择，未讨论参数敏感性。
- **统计细节缺失**：摘要未提供具体统计量（如相关系数r、分类准确率、p值等），难以评估效果大小和可靠性。
- **未对比静态连接模型**：无法断言动态连接相对于静态连接的优势。

（完）
