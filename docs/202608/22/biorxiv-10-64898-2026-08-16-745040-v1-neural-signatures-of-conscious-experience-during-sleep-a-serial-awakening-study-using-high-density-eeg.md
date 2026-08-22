---
title: "Neural Signatures of Conscious Experience During Sleep: A Serial Awakening Study Using High-Density EEG"
title_zh: 睡眠中意识体验的神经特征：基于高密度脑电图的序列唤醒研究
authors: "Selte, A., Haworth, S. E., Vannasse, T. J., Alauddin, T., Gjini, K., Philibert-Rosas, S., Brace, C., Sevak, B., Riedner, B., Kalkach-Aparicio, M., Tononi, G., Boly, M., Struck, A. F."
date: 2026-08-20
pdf: "https://www.biorxiv.org/content/10.64898/2026.08.16.745040v1.full.pdf"
tags: ["query:slp-ns"]
score: 9.0
evidence: 非快速眼动睡眠觉醒，高密度脑电，意识神经特征
tldr: 意识体验的神经机制尚不明确，睡眠为研究意识有无提供了理想窗口。本研究利用高密度脑电对140名受试者进行连续唤醒，分析了699次非快速眼动睡眠阶段的有无梦境体验。结果发现梦境体验与后部脑区α、δ功率降低及γ相关指标升高、网络组织改变有关。跨被试机器学习分类器均优于随机水平，最佳集成模型ROC-AUC达0.80。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-08-16-745040-v1/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 495, \"height\": 162, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-08-16-745040-v1/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1525, \"height\": 1887, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-08-16-745040-v1/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 3134, \"height\": 1941, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-08-16-745040-v1/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 232, \"height\": 188, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-08-16-745040-v1/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 232, \"height\": 188, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-08-16-745040-v1/fig-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 815, \"height\": 560, \"label\": \"Figure\"}]"
tables_json: "[{\"url\": \"assets/tables/biorxiv/biorxiv-10-64898-2026-08-16-745040-v1/table-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1714, \"height\": 1605, \"label\": \"Table\"}]"
motivation: 在睡眠中比较有/无主观体验时的脑活动，可避开行为反应干扰，识别意识的神经相关信号。
method: 对140人进行整夜256导高密度脑电记录，采用连续唤醒范式，提取睡醒前60秒的频谱、连接和图论特征，并用机器学习分类梦境有无。
result: 梦境体验伴随后部α、δ功率下降和γ相关指标上升，网络组织改变；最佳集成模型ROC-AUC和平均精确度均为0.80。
conclusion: 后部脑电频谱平衡和大尺度网络组织是NREM睡眠意识状态的可复现神经特征，为意识研究提供客观指标。
---

## 摘要
识别意识的神经特征仍然是神经科学的核心挑战。睡眠为比较有无主观体验时的大脑活动提供了一个易处理的模型，同时最大程度地减少了行为反应性混杂因素。我们使用 140 名参与者的过夜 256 电极高密度脑电图和序列唤醒范式，分析了 699 次非快速眼动（NREM）睡眠 2 期和 3 期唤醒（351 次有梦境体验，348 次无体验）。唤醒前 60 秒的特征包括区域频谱功率、滞后相干连接性、图论指标和伽马-阿尔法功率比。梦境体验与后部频谱平衡的变化相关，特别是 alpha 和 delta 功率降低、伽马相关指标增加，以及大规模网络组织的改变。在参与者级别的交叉验证机器学习分析中，所有分类器的表现均优于随机水平，最佳集成模型的 ROC-AUC 达到 0.80，平均精度为 0.80。这些发现确定了 NREM 睡眠期间意识状态的可复现的后部电生理和网络级特征。

## Abstract
Identifying neural signatures of consciousness remains a central challenge in neuroscience. Sleep offers a tractable model for comparing brain activity in the presence or absence of subjective experience while minimizing behavioral responsiveness confounds. Using overnight 256 electrode high-density EEG in 140 participants and a serial-awakening paradigm, we analyzed 699 non-rapid eye movement (NREM) sleep stage 2 and 3 awakenings (351 dreaming experience, 348 no experience). Features from the 60s preceding awakening included regional spectral power, lagged-coherence connectivity, graph-theoretic metrics and gamma-to-alpha power ratios. Dreaming experiences were associated with shifts in posterior spectral balance, particularly reduced alpha and delta power and increased gamma-related measures, together with altered large scale network organization. In participant-level cross-validated machine-learning analyses, all classifiers performed above chance, with the best ensemble model reaching an ROC-AUC of 0.80 and average precision of 0.80. These findings identify reproducible posterior electrophysiological and network-level signatures of conscious states during NREM sleep.

---

## 论文详细总结（自动生成）

## 1. 论文的核心问题与整体含义（研究动机和背景）

- **核心问题**：意识体验的神经相关物（Neural Correlates of Consciousness, NCC）是什么？主观体验的有无如何在脑活动中体现？
- **研究背景**：意识研究长期面临行为反应混杂的难题。睡眠提供了一个独特窗口——受试者处于无行为反应状态，却可以在有/无主观体验之间自然切换，使研究者能够分离意识体验的神经特征与行为反应性。
- **研究动机**：
  - 既往研究表明梦境体验与后部皮层低频活动（尤其是delta波）降低有关，但多数研究样本量小（多在数十人以内），结论未获大规模验证。
  - 传统的单一频谱分析方法可能不足以捕捉意识的复杂性，需要结合功能连接、网络组织、跨频耦合等多维度信息。
  - 机器学习可用于在高维特征空间中系统搜索区分意识与非意识状态的最优特征组合，但在此类数据上尚无大规模应用。
- **整体含义**：本研究旨在通过大规模高密度脑电图（HD-EEG）数据和序列唤醒范式，识别可复现的、客观的睡眠意识状态电生理标记，为意识的科学研究和临床意识评估提供客观工具。

## 2. 论文提出的方法论

### 2.1 核心思想
将觉醒前60秒的脑电信号转化为多维特征空间，涵盖频谱功率、功能连接、网络拓扑和跨频平衡四大类特征，通过统计筛选和机器学习分类，区分"有意识体验"（CE）和"无意识体验"（NCE）两种状态。

### 2.2 关键技术细节

**（1）频谱分析**
- 使用 **Welch法**（2秒窗口，50%重叠）估计功率谱密度（PSD）。
- 提取五个频带的带限功率：delta（0.5–4Hz）、theta（4–8Hz）、alpha（8–12Hz）、beta（12–30Hz）、gamma（30–40Hz）。
- 按解剖学定义将电极分为后部（posterior）、额部（frontal）和对照（control）三大区域：
  - **后部区域**：以顶枕区为主（如P7、P5、PO3等）
  - **额部区域**：前额叶及前部电极（如F7、AF3、Fp1等）
  - **对照区域**：中央区电极（如C3、C4、Cz等）

**（2）功能连接**
- 使用**滞后相干性（Lagged Coherence）**构建连接矩阵：
  - 公式：$LagCoh(xy)(f) = |Im(C_{xy}(f))|² / (P_{xx}(f)·P_{yy}(f))$
  - 基于互谱密度的虚部归一化，可最大程度地减少零延迟耦合和容积传导伪迹。
- 滑动窗口法（2秒、50%重叠），每个频带生成一个平均连接矩阵。

**（3）图论网络指标**
从加权连接矩阵中计算三个全局指标：
- **模块度（Modularity Q）**：衡量网络社区结构/功能分离程度
- **全局效率（Global Efficiency）**：基于最短路径长度的倒数，衡量网络整合程度
- **Rich-club系数**：衡量高度节点（hub）之间的优先连接程度

**（4）工程化跨频特征**
- 构造**gamma/alpha功率比**（后部和额部分别计算），反映皮层激活水平与跨频平衡。

**（5）特征筛选流程**
- 初始约60个候选特征 → Mann-Whitney U检验 → Benjamini-Hochberg FDR校正 → 仅保留效应量|Rank-Biserial r| > 0.4的特征 → 互信息分析（处理非线性关系）→ LASSO正则化（降低冗余和多重共线性）。

**（6）机器学习分类**
- 使用多种分类器：逻辑回归、支持向量机（SVM）、前馈神经网络、K近邻（KNN）、感知器、随机森林、概率集成模型。
- 采用**参与者级5折交叉验证**（同一参与者的所有唤醒归属同一折），防止数据泄漏。

## 3. 实验设计

### 3.1 数据集
- **参与者**：140名健康成人（男性82名，女性58名），年龄25–66岁（平均44.24岁）。
- **数据采集**：整夜256导高密度脑电图（HD-EEG）记录，采用**序列唤醒范式**（serial awakening paradigm）。
- **唤醒方法**：通过自动听觉刺激唤醒，询问参与者是否做梦。
- **纳入标准**：仅分析NREM睡眠2期和3期的唤醒；排除NREM 1期、NREM 4期和REM睡眠唤醒。
- **数据规模**：共699次有效唤醒（351次有意识体验CE，348次无意识体验NCE），平均每人4.99次唤醒。
- **标签定义**：CE = 能清晰报告梦境内容；NCE = 未做梦且无法回忆梦境内容。

### 3.2 Benchmark
- 分类任务：CE vs NCE
- 主要评估指标：ROC-AUC（主指标）、平均精度（AP）
- 基线：随机水平（AUC = 0.5）

### 3.3 对比方法
- 六种监督学习算法对比：逻辑回归、SVM、KNN、感知器、随机森林、概率集成模型。
- 不同特征域的效果通过统计显著性检验和效应量进行比较（频谱、连接、图论、工程化特征）。

## 4. 资源与算力

- **论文未明确说明**使用的GPU型号、数量或具体训练时长。
- 从方法推断：该研究使用的特征数量较少（经筛选后约10个特征），模型复杂度不高（逻辑回归、SVM、随机森林等），预计对算力需求较低，可在标准CPU工作站上完成训练。
- 数据规模（699个样本、256导联、60秒脑电）无需分布式计算或大规模并行处理。

## 5. 实验数量与充分性

### 5.1 实验数量
- **统计筛选**：约60个候选特征，通过Mann-Whitney U检验和FDR校正，最终保留12个显著特征。
- **分类实验**：6种模型 × 5折交叉验证 = 30组评估。
- **无单独消融实验**：论文未报告单独的特征域消融（如仅频谱、仅连接、仅图论特征）的对比实验。

### 5.2 充分性与客观性评估
- **优点**：
  - 参与者级交叉验证有效防止了被试泄漏，评估更保守可信。
  - ROC-AUC和PR-AUC双重指标，结论一致性高。
  - 统计筛选标准严格（FDR校正 + 效应量阈值双门槛）。
- **不足**：
  - 样本仅来自单一机构和单一记录系统，缺乏外部验证。
  - 未报告模型校准和特定操作点的敏感度/特异度。
  - 未进行NREM2与NREM3的分层（stage-specific）分析。
  - 未对特征域做系统消融，无法判断各特征域的独立贡献。
  - 缺失分类器的置信区间和显著性检验。

## 6. 论文的主要结论与发现

- **后部频谱特征是意识体验最强的判别指标**：
  - CE期后部α功率显著降低（r = -0.82，大效应量）
  - 后部δ功率降低（r = -0.78）
  - 后部γ功率降低（r = -0.68，即频率平衡整体向低频移动）
  - 后部gamma/alpha比升高（r = 0.75），额部gamma/alpha比升高（r = 0.63）
- **网络组织与意识体验相关**：
  - CE期delta频带网络模块度（Q）更低（r = -0.78），表明网络分离度降低
  - alpha频带全局效率更高（r = 0.58），表明网络整合增强
  - gamma频带rich-club系数更高（r = 0.49），表明hub节点间连接增强
- **机器学习分类有效**：所有分类器均优于随机水平。
  - 最佳表现：概率集成模型（ROC-AUC = 0.80，AP = 0.80）
  - 中间表现：随机森林（AUC 0.76）、逻辑回归（0.75）、SVM（0.74）
  - 较弱表现：KNN（0.71）、感知器（0.69）
- **线性/核方法表现竞争力强**，说明判别信息存在于所选特征空间中，而非依赖高度灵活的模型。
- **意识体验与网络整合增强、功能分离降低相关**，支持大规模信息整合对意识具有重要作用的观点。

## 7. 优点

- **大规模样本**：140名参与者、699次唤醒，远超此前同类研究（多在20–50人规模）。
- **多模态特征融合**：同时涵盖频谱功率、功能连接、图论指标和工程化跨频特征，克服了单一特征域的局限。
- **严格的防泄漏设计**：参与者级分组交叉验证，有效避免同一受试者的多次唤醒被同时分入训练和测试集。
- **稳健的统计方法**：FDR校正 + 效应量阈值 + 非参数检验（Mann-Whitney U），降低了假阳性风险。
- **滞后相干性选择**：抑制了容积传导和零延迟耦合的干扰，提高了连接估计的可靠性。
- **对意识理论的多重支持**：结果与全局工作空间理论（后部皮质激活）、整合信息理论（网络整合提升）一致，有理论关联性。
- **实践转化潜力**：提出的特征和模型有望在小通道数场景下应用，为临床意识评估提供无创客观工具。

## 8. 不足与局限

- **标签依赖主观报告**：意识体验依赖受试者醒来后的口头报告，可能低估实际体验（记忆遗忘），无法区分"意识体验的缺失"与"回忆失败"。
- **NREM阶段限制**：仅分析了NREM 2期和3期，结果不可推广到REM睡眠、麻醉状态或严重脑损伤患者。
- **头皮脑电的间接性**：头皮HD-EEG提供的是神经活动的间接相关性测量，空间分辨率有限。
- **连接估计的敏感性**：尽管采用滞后相干性，但头皮记录仍受容积传导、参考电极选择和信噪比波动影响。
- **唤醒前60秒的混淆因素**：唤醒前后的觉醒水平波动（睡眠惯性）可能影响频谱特征，CE/NCE差异可能部分反映"临近唤醒时的觉醒程度"而非"纯粹的意识状态"。
- **网络阈值问题未充分讨论**：图论指标对阈值选择和预处理参数敏感，论文未报告阈值稳定性分析。
- **泛化性未验证**：未在独立数据集或不同记录系统上进行外部验证。
- **因果性无法推断**：相关性研究设计，无法确定所观察到的电生理模式是意识体验的"原因"还是"结果"。
- **性能和确定性边界**：0.80的AUC表明脑电信号包含概率性信息，但未达到确定性预测水平——不能将性能解读为意识的确定性"指纹"。

---

（完）
