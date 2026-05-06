---
title: Yawning reveals energy-dynamics mismatch and neural inertia across state transitions
authors: "Meng, X., Sun, Q., Li, M., Li, X., Liang, G., Qin, L., Tan, W."
date: 2026-04-29
pdf: "https://www.biorxiv.org/content/10.64898/2026.04.26.720882v1.full.pdf"
tags: ["query:slp-ns"]
score: 9.0
evidence: 觉醒状态转换过程中的神经动力学
tldr: 本研究通过比格犬模型和人类临床数据，结合EEG、EMG及EMD-HHT分析，探讨了打哈欠在意识状态转换中的神经动力学。研究发现打哈欠并非简单的被动反射，而是与一种被称为“能量-动力学失配”（EDM）的瞬态脑态特征紧密相关，即局部高频活动增加与全局网络灵活性下降并存。这一发现揭示了打哈欠是克服神经惯性、维持信息整合的补偿性过程，为监测觉醒状态和脑机接口开发提供了潜在的生物标志物。
source: biorxiv
selection_source: fresh_fetch
motivation: 旨在探究打哈欠在脑网络组织大规模变化过程中的精确神经动力学机制，挑战传统的被动反射模型。
method: 采用比格犬模型进行同步EEG/EMG记录，并利用希尔伯特-黄变换分析丙泊酚麻醉及清醒状态下的神经信号，随后在人类队列中进行验证。
result: 发现打哈欠伴随着局部伽马频段功率上升与全局网络灵活性下降的“能量-动力学失配”特征，且绝大多数事件发生于麻醉苏醒期。
conclusion: 打哈欠是应对网络不稳定性的一种主动补偿机制，反映了大脑在克服神经惯性以维持信息整合时的“控制努力”。
---

## Abstract
Yawning is a highly conserved behavior, yet its neural dynamics across arousal state transitions remain poorly understood. Classical reflex models fail to account for the precise timing of yawns during large-scale changes in brain network organization. Here, we investigated the neural signatures of yawning using simultaneous electroencephalography (EEG), electromyography (EMG), and kinematic recordings in a beagle model during wakefulness and propofol anesthesia. Propofol-associated yawning exhibited marked temporal asymmetry, with 89.2% of events occurring during emergence from anesthesia. To resolve the fast neural dynamics surrounding these events, we applied empirical mode decomposition coupled with the Hilbert-Huang transform (EMD-HHT) analyses. Across induction, recovery, and wakefulness, yawning was consistently associated with a transient decoupling between local and global network dynamics: a brief increase in local {gamma}-band power coincided with a drop in network flexibility, quantified by instantaneous frequency volatility; IFV). We termed this reproducible motif as "Energy-Dynamics Mismatch" (EDM). A machine learning classifier leveraging EDM features reliably decoded the brain state immediately preceding yawning. We further validated the presence of this signature in an independent human cohort during anesthesia induction. These findings indicate that yawning is not a passive reflex, but is tightly linked to moments of network instability during state transitions. From a computational perspective, EDG may reflect a transient "control effort" that preserves information integration in the presence of "neural inertia." This dynamic signature may provide a quantitative biomarker for monitoring arousal transitions brain-computer interface (BCI) interface state-alerting.

Significance StatementYawning is a ubiquitous and evolutionarily conserved behavior, yet its neural basis remains elusive. Using high-resolution neural recordings in a cross-species model, we show that yawning is not a passive reflex, but reliably coincides with a distinct, transient brain-state signature. Specifically, yawning occurs when local high-frequency cortical activity briefly increases while global network flexibility decreases - a pattern we term an "Energy-Dynamics Mismatch" (EDM). We propose that EDM reflects a compensatory neural process engaged during moments of network instability, consistent with overcoming neural inertia to preserve information integration. By identifying this conserved neural marker, this work advances the biological understanding of yawning and suggests a potential biomarker for detecting critical brain states in future BCI.

---

## 论文详细总结（自动生成）

这篇论文深入探讨了打哈欠这一进化保守行为背后的神经动力学机制，挑战了传统的被动反射理论。以下是对该论文的结构化总结：

### 1. 核心问题与整体含义
*   **研究动机**：尽管打哈欠在脊椎动物中普遍存在，且常发生在觉醒状态转换（如睡眠-觉醒循环、麻醉苏醒）期间，但其精确的神经触发机制尚不清楚。
*   **核心问题**：传统的散热或呼吸反射模型无法解释打哈欠在脑网络重组窗口内的精确时机。研究者试图探究打哈欠是否反映了大脑在克服“神经惯性”（Neural Inertia）以实现状态转换时的一种主动神经计算过程。

### 2. 方法论
*   **核心思想**：通过整合皮层能量（γ频段功率）和网络灵活性（瞬时频率波动率，IFV）两个维度，识别打哈欠前的微观神经特征。
*   **关键技术细节**：
    *   **实验模型**：建立比格犬丙泊酚麻醉-苏醒模型，利用其发达的皮层结构模拟人类脑网络动力学。
    *   **多模态记录**：同步采集硬膜外脑电图（EEG）、咬肌肌电图（EMG）及高精度运动学信号。
    *   **行为识别**：利用 **DeepLabCut** 算法对脸部矢量进行标记追踪，精确定义打哈欠的动力学起点（t=0）。
    *   **信号处理**：采用**经验模态分解（EMD）**与**希尔伯特-黄变换（HHT）**。相比传统傅里叶变换，该方法能解析非线性、非平稳信号在毫秒级的瞬时频率变化。
    *   **能量-动力学失配（EDM）定义**：指局部高频能量增加与网络灵活性（IFV）下降同时发生的瞬态脱节现象。

### 3. 实验设计
*   **数据集/场景**：
    *   **比格犬实验**：6只犬，每只进行3次标准化麻醉-苏醒循环，共获得36次完整记录和96次麻醉相关哈欠事件。
    *   **人类验证**：独立的人类临床队列（n=9），用于验证发现的跨物种普适性。
    *   **清醒状态实验**：在药物洗脱7天后记录100次自发性哈欠，排除药物干扰。
*   **对比方法（Benchmark）**：
    *   **严格匹配控制组**：通过在80维功率谱空间中计算欧氏距离，寻找与打哈欠期宏观脑态最接近的非打哈欠片段作为基准。
    *   **分类器**：使用随机森林（Random Forest）分类器对预哈欠微状态进行解码，并进行置换检验（Permutation test）。

### 4. 资源与算力
*   论文中未明确提及具体的 GPU 型号、数量或训练时长。由于主要涉及的是信号处理算法（EMD-HHT）和常规机器学习模型（随机森林），此类计算通常在标准科研工作站上即可完成。

### 5. 实验数量与充分性
*   **实验规模**：涵盖了诱导期、维持期、苏醒期及清醒状态，实验组数充足。
*   **充分性与客观性**：
    *   采用了跨物种（犬与人）的验证，增强了结论的生物学普遍性。
    *   使用了线性混合效应模型（LMM）处理重复测量数据，考虑了个体差异。
    *   通过动态时间规整（DTW）和自助法（Bootstrap）确保了轨迹比较的客观性。

### 6. 主要结论与发现
*   **时间不对称性**：丙泊酚诱导的哈欠具有显著的相位特异性，89.2% 发生在苏醒期，这与克服“神经惯性”以重启意识网络的需求相吻合。
*   **EDM 特征**：无论在麻醉还是清醒状态下，打哈欠前均会出现一致的“能量-动力学失配”——局部 γ 功率上升，而网络灵活性（IFV）骤降。
*   **控制努力（Control Effort）**：从计算角度看，EDM 反映了大脑在网络不稳定期间，为维持信息整合而付出的瞬态“控制努力”。
*   **生物标志物**：EDM 可作为监测觉醒状态转换和脑机接口（BCI）状态预警的定量生物标志物。

### 7. 优点
*   **技术先进性**：引入 EMD-HHT 分析，捕捉到了传统 EEG 分析无法识别的瞬态微观动力学特征。
*   **定义精确**：结合计算机视觉和电生理，消除了以往研究中对打哈欠起始点定义的模糊性。
*   **理论深度**：提出了 EDM 这一新概念，成功将宏观的药理学现象（神经惯性）与微观的神经动力学联系起来。

### 8. 不足与局限
*   **因果关系尚不明确**：目前属于观察性研究，尚未通过光遗传学等手段证明 EDM 与皮层下哈欠中枢（如下丘脑旁室核）之间的直接因果链。
*   **药物单一性**：主要基于丙泊酚模型，其他麻醉剂（如氯胺酮或吸入性麻醉药）下的表现是否一致仍需验证。
*   **人类样本量**：人类验证队列的样本量（n=9）相对较小，未来需更大规模的临床数据支持。

（完）
