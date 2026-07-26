---
title: Serotonin induces DOWN states across the anesthetized mouse forebrain
title_zh: 血清素诱导麻醉小鼠前脑的DOWN状态
authors: "Grossmann, R., Meijas, J. F., International Brain Laboratory,, Mainen, Z. F., Meijer, G. T."
date: 2026-07-21
pdf: "https://www.biorxiv.org/content/10.64898/2026.07.14.738517v2.full.pdf"
tags: ["query:slp-ns"]
score: 10.0
evidence: 血清素诱导与睡眠相关的DOWN状态
tldr: 五羟色胺（5-HT）在睡眠和麻醉中调节脑状态，但其全局影响存在争议。本研究结合光遗传刺激与大规模神经探针记录，发现选择性释放5-HT可一致诱导前脑（皮层和纹状体）的DOWN状态，而中脑动态基本不变。基于生物可解释连接的多区域计算模型表明，这种转变源于网络同步而非直接DRN输入，揭示了5-HT对全局脑状态的新机制。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-14-738517-v2/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1344, \"height\": 1378, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-14-738517-v2/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1756, \"height\": 1765, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-14-738517-v2/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1788, \"height\": 1358, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-14-738517-v2/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1733, \"height\": 1003, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-14-738517-v2/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1724, \"height\": 583, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-14-738517-v2/fig-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 1766, \"height\": 439, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-14-738517-v2/fig-007.webp\", \"caption\": \"\", \"page\": 0, \"index\": 7, \"width\": 1759, \"height\": 631, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-14-738517-v2/fig-008.webp\", \"caption\": \"\", \"page\": 0, \"index\": 8, \"width\": 1779, \"height\": 548, \"label\": \"Figure\"}]"
tables_json: "[{\"url\": \"assets/tables/biorxiv/biorxiv-10-64898-2026-07-14-738517-v2/table-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1361, \"height\": 460, \"label\": \"Table\"}]"
motivation: 前期研究对5-HT调节全局脑状态存在矛盾，电刺激诱导UP状态而光遗传fMRI显示抑制，需解决分歧。
method: 在轻度麻醉小鼠中，结合光遗传5-HT刺激与跨前脑的Neuropixel大规模电生理记录，并构建多区域计算模型。
result: 选择性5-HT释放一致诱导皮层和纹状体的DOWN状态，中脑动态几乎不受影响。
conclusion: 5-HT通过网络同步机制而非直接输入诱导前脑DOWN状态，解决了先前矛盾，阐明了5-HT调控全局脑状态的新机制。
---

## 摘要
中缝背核（DRN）的血清素能神经元广泛投射至前脑，但它们对全局网络状态的影响仍存在争议。血清素被认为调节慢振荡，即所谓的UP和DOWN状态，这些状态在睡眠和轻度麻醉期间出现。虽然光遗传fMRI表明血清素（5-HT）抑制全脑活动，但经典电刺激研究报告诱导了皮层UP状态。为解决这一矛盾，我们将光遗传5-HT刺激与轻麻醉小鼠前脑的大规模Neuropixel记录相结合。我们证明选择性5-HT释放一致地诱导皮层和纹状体的DOWN状态，而中脑动力学基本不受影响。一个基于生物可信连接的多区域计算模型表明，在某些区域，这种转变源于网络级同步而非直接的DRN输入。

## Abstract
Serotonergic neurons in the dorsal raphe nucleus (DRN) project extensively throughout the forebrain, yet their influence on global network states remains controversial. Serotonin is implicated in regulating slow-oscillations, so-called UP and DOWN states, which occur during sleep and light anesthesia. While optogenetic fMRI suggests that serotonin (5-HT) suppresses brain-wide activity, classical electrical stimulation studies report the induction of cortical UP states. To resolve this discrepancy, we combined optogenetic 5-HT stimulation with large-scale Neuropixel recordings across the forebrain of lightly anesthetized mice. We demonstrate that selective 5-HT release consistently induces DOWN states across the cortex and striatum, while leaving midbrain dynamics largely unaffected. A multi-area computational model constrained by biologically plausible connectivity, indicates that in certain regions the transitions arises from network-level synchronization rather than direct DRN input.

---

## 论文详细总结（自动生成）

# 论文总结

## 1. 论文的核心问题与整体含义（研究动机和背景）

- 血清素（5-HT）是一种重要的中枢神经调节物质，参与慢振荡（UP/DOWN状态）的调控，这些状态在睡眠和麻醉中至关重要，用于学习、记忆巩固和可塑性。
- 此前研究存在矛盾：光遗传fMRI表明5-HT抑制全脑活动，而经典电刺激DRN的研究却报告诱导了皮层UP状态。
- 作者希望解决这一争议，并探索5-HT对全局脑状态的作用机制——是直接驱动还是通过网络同步间接影响？这一问题的澄清有助于理解血清素在睡眠、麻醉及神经精神疾病中的功能。

## 2. 论文提出的方法论：核心思想、关键技术细节、公式或算法流程

- **核心思想**：结合光遗传选择性激活DRN血清素能神经元与大规模Neuropixel电生理记录，同时构建多区域计算模型，揭示5-HT诱导DOWN状态的网络机制。
- **关键技术细节**：
  - **动物模型**：SERT-Cre C57Bl/6小鼠，病毒注入ChR2，植入光纤。
  - **光遗传刺激**：蓝光（465 nm），5 mW，脉冲宽度10 ms，频率1/5/10/25 Hz，持续1 s，间隔随机（指数分布，均值6s）。
  - **Neuropixel记录**：急性记录，7个探针插入位置覆盖前脑（额叶皮层、视觉皮层、梨状皮层、杏仁核、纹状体、海马、丘脑、中脑），共5只表达ChR2的小鼠，2只作为对照。
  - **数据预处理与建模**：使用IBL自动流水线进行spike sorting，HMM（隐马尔可夫模型）量化UP/DOWN状态。计算模型为双稳态发放率模型，包含E-I回路和适应机制，使用Allen脑图谱的真实连接数据。
- **公式或算法流程（文字说明）**：
  - 局部电路动力学方程：含E、I两个群体，适应变量a，噪声项，阈值线性转移函数。
  - 全局网络通过投影密度矩阵连接，耦合强度G可调。
  - 5-HT刺激模拟：对E群体施加抑制性电流，强度与DRN投影密度成正比，时间曲线匹配实验观察。
  - 通过改变G从0到3，比较不同耦合强度下DOWN状态概率与DRN投影密度的相关性，识别由网络同步导致的间接效应。

## 3. 实验设计：使用了哪些数据集 / 场景，它的 benchmark 是什么，对比了哪些方法

- **数据集**：实验数据来自5只ChR2表达小鼠和2只对照小鼠的Neuropixel记录，涵盖8个脑区（额叶皮层、视觉皮层、梨状皮层、杏仁核、纹状体、海马、丘脑、中脑）。
- **场景**：轻度异氟烷麻醉下，光遗传刺激DRN，同时进行全脑范围电生理记录。刺激频率有1、5、10、25 Hz，每个频率重复50次。
- **基准/对比方法**：
  - 无刺激基线对比（随机jitter时间）。
  - 与刺激发生于UP或DOWN状态时的子集对比。
  - 对照小鼠（无ChR2表达）验证光伪迹。
  - 计算模型中对不同5-HT作用机制（E-、I+、E+、I-）进行对比。
  - 模型中进行耦合强度G=0（完全解耦）与G=3（强耦合）的对比。
  - 从Allen脑图谱获取DRN投影密度和5-HT受体表达数据，与实验抑制强度做相关性分析。

## 4. 资源与算力

- 论文未明确说明使用的GPU型号、数量、训练时长等算力资源。
- 实验部分涉及7只小鼠、连续4天记录、每只小鼠7个探针插入，使用IBL spike sorting流水线（可能依赖CPU/GPU，但未详述）。
- 计算模型基于MATLAB/Python实现，复杂度中等，未报告具体算力需求。

## 5. 实验数量与充分性

- **实验组数**：
  - 5只ChR2+小鼠，2只ChR2-对照。
  - 每个小鼠4天记录，共7个插入位点，每个位点记录50次刺激（4种频率，总共约200次刺激/小鼠）。
  - 计算模型：进行了不同的刺激机制（E-/I+/E+/I-）比较，耦合强度扫描（G=0到3），以及相关性/留一法分析。
- **充分性评价**：
  - 实验设计较充分：多种频率、对照、子集分析、多脑区覆盖。
  - 计算模型提供了机制验证，但仅基于8个高层面区域（n=8），统计效力有限。
  - 相关性分析（Fig S3）使用了更细致区域划分，但未提供多重比较校正。
  - 总体而言，实验对于揭示主要现象足够，但在机制解释上仍需更多药理学和因果验证。

## 6. 论文的主要结论与发现

- 选择性光遗传激活DRN血清素能神经元在轻度麻醉小鼠中**快速诱导前脑（皮层、纹状体、杏仁核、海马、丘脑）的DOWN状态**，而中脑不受影响。
- 这种抑制作用既包括延长已有的DOWN状态，也包括将UP状态迅速切换为DOWN状态。
- 5-HT诱导的抑制强度与DRN投影密度**无显著相关性**，但与5-HT1f和5-HT2a受体表达水平相关。
- 计算模型显示：在无网络耦合时，DOWN状态概率与DRN投影密度强相关；而引入真实脑区间连接后，如视觉皮层等无直接DRN输入的脑区仍可被诱导DOWN状态，说明网络同步起到了关键作用。
- 模型进一步表明，只有**抑制兴奋性群体（E-）**能有效诱导DOWN状态，而兴奋抑制性群体（I+）等其他方式效果不佳。

## 7. 优点

- **解决矛盾**：将全脑fMRI与局部电生理结果桥接，采用大规模高时空分辨率记录，清晰展示了5-HT诱导DOWN状态而非UP状态。
- **多模态结合**：光遗传+Neuropixel+计算模型，从现象到机制进行系统分析。
- **基于真实连接**：计算模型利用了Allen脑图谱的解剖学连接，增强了生物学可解释性。
- **控制实验完善**：包括无ChR2表达的对照小鼠、对不同刺激频率的分析、UP/DOWN状态起始条件的子集分析。
- **开放性**：数据和代码公开发布，促进可重复性。

## 8. 不足与局限

- **样本量小**：仅5只ChR2+小鼠，8个高层面区域，统计分析（如相关性）的统计效力有限，尤其留一法分析显示某些结果依赖特定区域。
- **麻醉状态是否可推广**：异氟烷诱导的UP/DOWN状态与自然非REM睡眠的异同仍有争议，结果可能不直接推广到清醒或睡眠状态。
- **模型简化**：计算模型为开环（无DRN反馈），且未包含体积传输、不同受体亚型分布等细节；模型参数针对脑区进行了调优，可能过度拟合。
- **机制证据不充分**：5-HT1f和5-HT2a受体的相关性仅基于Allen数据集的表达谱，缺乏直接药理学阻断/激活实验。
- **缺少行为/清醒条件**：论文未展示清醒状态下5-HT刺激的效应，仅在麻醉条件下；作者另一研究可能涉及但本文未包含。
- **HMM假阳性风险**：对于本身无UP/DOWN动力学的区域（杏仁核、海马），HMM检测到的“DOWN状态”更可能仅反映抑制而非真正的状态转换，作者已意识到此局限但缺乏进一步验证。

（完）
