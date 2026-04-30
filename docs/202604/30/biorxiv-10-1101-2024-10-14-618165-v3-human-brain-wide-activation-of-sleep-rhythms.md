---
title: Human Brain-Wide Activation of Sleep Rhythms
title_zh: 人类全脑睡眠节律的激活
authors: "Wang, H., Zou, Q., Zhang, J., Gao, J.-H., Liu, Y."
date: 2026-04-22
pdf: "https://www.biorxiv.org/content/10.1101/2024.10.14.618165v3.full.pdf"
tags: ["query:slp-ns"]
score: 10.0
evidence: 睡眠节律的大脑激活与非快速眼动睡眠阶段
tldr: 本研究通过对107名参与者进行同步EEG-fMRI监测，探讨了人类睡眠节律（慢波振荡与快纺锤波）的全脑激活机制。研究发现在深睡期慢波与纺锤波存在强耦合，并伴随丘脑和海马体的显著激活，以及海马-丘脑-前额叶皮层的功能连接增强。这些发现揭示了丘脑在协调海马-皮层通信中的核心作用，为睡眠支持记忆巩固的机制提供了新见解。
source: biorxiv
selection_source: fresh_fetch
motivation: 旨在探索人类睡眠节律相关的全脑激活模式及其在记忆巩固中的功能意义。
method: 对107名受试者在夜间睡眠期间进行了同步脑电图（EEG）和功能磁共振成像（fMRI）监测。
result: 研究发现慢波振荡与快纺锤波紧密耦合，并显著增强了丘脑、海马体以及内侧前额叶之间的功能连接。
conclusion: 丘脑是睡眠期间海马-皮层通信的关键协调者，通过同步神经节律支持情境记忆的巩固过程。
---

## 摘要
在睡眠期间，我们的大脑经历高度同步的活动，由不同的神经节律协调。目前关于这些睡眠节律相关的脑激活知之甚少，对其功能意义的了解则更少。在本研究中，我们通过对 107 名参与者在夜间小睡（前半夜）期间采用同步脑电图 (EEG) 和功能磁共振成像 (fMRI)，研究了人类睡眠节律背后的全脑激活。我们在深度非快速眼动 (NREM) 睡眠（N2/3 阶段）期间发现了慢波振荡 (SOs) 与快纺锤波之间的强耦合，纺锤波峰值一致出现在 SO 上行状态 (UP-state) 之前。这种 SO-纺锤波耦合与丘脑和海马体的激活升高有关，同时伴随着从海马体到丘脑以及从丘脑到内侧前额叶皮层 (mPFC) 的功能连接增强。一项开放式认知状态解码分析表明，这些激活可能与情境记忆过程有关，但与任务相关网络不同。总之，这些发现强调了丘脑是睡眠期间海马-皮层通信的关键协调者，并为同步睡眠节律支持记忆巩固的机制提供了新见解。

## Abstract
During sleep, our brain undergoes highly synchronized activity, orchestrated by distinct neural rhythms. Little is known about the associated brain activation during these sleep rhythms, and even less about their functional implications. In this study, we investigated the brain-wide activation underlying human sleep rhythms by employing simultaneous electroencephalography (EEG) and functional magnetic resonance imaging (fMRI) in 107 participants during nocturnal nap (first half of the night). We identified robust coupling between slow oscillations (SOs) and fast spindles during deep non-rapid eye movement (NREM) sleep (N2/3 stages), with spindle peaks consistently occurring just before the SO UP-state. This SO-spindle coupling was linked to elevated activation in both the thalamus and hippocampus, alongside increased functional connectivity from the hippocampus to the thalamus and from the thalamus to the medial prefrontal cortex (mPFC). An open-ended cognitive state decoding analysis suggested that these activations may relate to episodic memory processes, yet were distinct from task-related networks. Together, these findings highlight the thalamus as a key coordinator of hippocampal-cortical communication during sleep and provide new insights into the mechanisms by which synchronized sleep rhythms may support memory consolidation.

---

## 论文详细总结（自动生成）

这篇论文《Human Brain-Wide Activation of Sleep Rhythms》由北京师范大学和北京大学的研究团队合作完成，发表于 bioRxiv。以下是对该研究的结构化总结：

### 1. 核心问题与整体含义（研究动机和背景）
*   **核心问题**：在非快速眼动（NREM）睡眠期间，大脑产生的慢波振荡（SO）和睡眠纺锤波（Spindle）是如何在全脑范围内协调激活的？它们之间的耦合如何支持海马体与皮层之间的通信？
*   **背景**：现有的“三重耦合”假说认为 SO、纺锤波和海马涟漪（Ripples）的同步是记忆巩固的基础。然而，由于技术限制，人类活体大脑中这些节律相关的全脑空间激活模式及功能连接路径仍不清晰。本研究旨在填补这一空白，揭示丘脑在其中的协调作用。

### 2. 方法论：核心思想与技术细节
*   **核心思想**：利用**同步 EEG-fMRI 技术**，结合 EEG 的高时间分辨率（检测瞬时节律事件）和 fMRI 的高空间分辨率（定位脑区激活），在自然睡眠状态下捕捉神经节律的动态过程。
*   **关键技术流程**：
    1.  **EEG 预处理**：采用平均伪迹去除法（AAS）消除 MRI 梯度噪声，利用 ICA 去除心源性（BCG）和眼动伪迹。
    2.  **睡眠分期与节律检测**：使用 YASA 算法自动分期并经专家人工校验。针对 N2/3 阶段，基于振幅百分比阈值（75th percentile）检测 SO 和纺锤波。
    3.  **耦合定义**：将纺锤波峰值出现在 SO 槽值（DOWN-state）后 1.5 秒内的事件定义为“SO-纺锤波耦合”。
    4.  **fMRI 建模**：
        *   **GLM 分析**：将 EEG 检测到的 SO、纺锤波及耦合事件作为回归量，与血氧水平依赖（BOLD）信号进行卷积，识别相关激活脑区。
        *   **PPI 分析**：通过心理生理交互作用（PPI）分析，研究在耦合发生时，海马、丘脑和内侧前额叶（mPFC）之间功能连接的变化。
    5.  **认知解码**：利用 NeuroSynth 数据库进行元分析解码，推测激活模式对应的潜在认知功能。

### 3. 实验设计
*   **数据集与场景**：招募了 138 名健康受试者（最终有效样本 107 人），在前半夜进行约 3 小时的同步 EEG-fMRI 监测。
*   **对比维度**：
    *   **阶段对比**：比较 N1、N2/3 和 REM 阶段的节律密度与振幅。
    *   **事件对比**：对比“耦合事件”与“非耦合事件”引发的脑激活差异。
    *   **状态对比**：分析 SO 的上行状态（UP-state）与下行状态（DOWN-state）对 BOLD 信号的不同影响。
*   **Benchmark**：本研究属于探索性基础研究，主要对比对象为随机基准或孤立的节律事件。

### 4. 资源与算力
*   **硬件设备**：使用 3T Siemens Magnetom Prisma MRI 扫描仪和 64 通道 MR 兼容 EEG 系统。
*   **算力说明**：论文未明确提及具体的 GPU 型号或训练时长。由于该研究主要涉及信号处理和统计建模（使用 Python MNE, Nilearn, SPM12, fMRIPrep 等工具），其计算压力主要集中在 fMRI 预处理和大规模 GLM 运算上，而非深度学习训练。

### 5. 实验数量与充分性
*   **样本规模**：107 名受试者的大样本量在同步 EEG-fMRI 睡眠研究中具有显著优势，增强了结果的可重复性和统计效力。
*   **控制实验**：
    *   进行了**消融/敏感性分析**：通过改变 SO 检测的百分比阈值（71%-80%）验证结果的稳健性。
    *   **电极验证**：对比了 F3 和 Fz 电极检测结果的一致性。
    *   **排除干扰**：排除了睡眠时长不足或头动过大的受试者。
*   **充分性评价**：实验设计严谨，统计校正（FWE 校正）严格，实验证据较为充分。

### 6. 主要结论与发现
*   **时序特征**：纺锤波峰值倾向于出现在 SO 上行状态（UP-state）即将开始之前（相位约 -41.61°）。
*   **空间激活**：
    *   **SO** 与默认模式网络（DMN）的去激活相关。
    *   **纺锤波** 与丘脑、前扣带回和基底节的激活相关。
    *   **SO-纺锤波耦合** 特异性地引起了**海马体和丘脑**的显著激活。
*   **功能连接**：在耦合期间，**海马 -> 丘脑** 以及 **丘脑 -> mPFC** 的功能连接显著增强。
*   **核心结论**：丘脑不仅是纺锤波的产生器，更是协调海马-皮层通信的关键“中继站”，通过睡眠节律的同步化支持记忆巩固。

### 7. 优点与亮点
*   **多模态融合**：成功在人类身上实现了瞬时电生理节律与全脑空间动态的关联。
*   **大样本量**：107 人的样本量显著高于同类研究（通常为 20-30 人），提高了结论的客观性。
*   **连接组学视角**：不仅关注脑区激活，还通过 PPI 揭示了信息流向，支持了系统巩固理论。

### 8. 不足与局限
*   **缺乏行为验证**：研究未包含睡眠前后的记忆任务测试，因此关于“记忆巩固”的结论主要基于生理指标和元分析解码的推论。
*   **EEG 局限性**：头皮 EEG 无法直接检测到深层的海马涟漪（Ripples），只能通过海马 BOLD 信号间接推断。
*   **空间分辨率限制**：虽然使用了 fMRI，但受限于 3T 磁共振的体素大小，无法精细区分丘脑内部的小核团或海马的亚区。
*   **电极覆盖**：节律检测主要基于额叶单电极，未能充分利用全脑 EEG 的空间分布特征。

（完）
