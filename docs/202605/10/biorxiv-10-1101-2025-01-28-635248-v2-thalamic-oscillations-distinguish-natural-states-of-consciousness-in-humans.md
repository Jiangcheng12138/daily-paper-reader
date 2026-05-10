---
title: Thalamic oscillations distinguish natural states of consciousness in humans
title_zh: 丘脑振荡区分人类的自然意识状态
authors: "Chowdhury, A., Wu, X., Beilner, T., Schreiner, T., Koeglsperger, T., Mehrkens, J.-H., Remi, J., Vollmar, C., Kaufmann, E., Staudigl, T."
date: 2026-05-10
pdf: "https://www.biorxiv.org/content/10.1101/2025.01.28.635248v2.full.pdf"
tags: ["query:slp-ns"]
score: 10.0
evidence: REM 和非 REM 睡眠期间的丘脑振荡
tldr: 丘脑被认为调节人类意识状态，但其电生理机制尚不明确。本研究通过直接记录人类丘脑的电活动，发现了一种频率在19-45 Hz之间的特异性振荡。该振荡仅在清醒和快速眼动（REM）睡眠中出现，而在非快速眼动（NREM）睡眠中消失。这一发现揭示了中央丘脑在区分意识状态中的关键作用，为理解意识机制及治疗意识障碍提供了新的电生理指标。
source: biorxiv
selection_source: fresh_fetch
motivation: 旨在探索人类丘脑在调节清醒与睡眠等自然意识状态中的底层电生理机制。
method: 利用罕见的临床机会，直接获取并分析了人类丘脑内部的深部电生理记录数据。
result: 在中央丘脑发现了一种19-45 Hz的特异性振荡，该振荡仅在清醒和REM睡眠中活跃，并能区分REM睡眠的微状态。
conclusion: 该研究确定了区分意识状态的独特丘脑振荡特征，强调了中央丘脑在维持意识中的核心地位及其潜在的临床治疗价值。
---

## 摘要
自然意识状态被认为受丘脑等深层脑结构的调节。然而，关于人类相关的底层电生理学知之甚少。在此，利用直接从人类丘脑记录的罕见机会，我们发现了一种此前未见报道的、频率约为 19-45 Hz 的脑状态特异性振荡。这种振荡仅在快速眼动（REM）睡眠和清醒期间出现，而在非快速眼动（Non-REM）睡眠期间消失。19-45 Hz 振荡进一步区分了 REM 睡眠的微状态，与眼球运动爆发同时发生，并且是中央丘脑（Central Thalamus）所特有的，该结构与引起全局脑状态转换有关。在中央丘脑发现这种区分意识状态的独特振荡特征，为进一步研究丘脑对人类意识状态的贡献开辟了道路，并可能有助于改进治疗意识障碍的干预措施。

## Abstract
Natural states of consciousness are thought to be regulated by deep brain structures such as the thalamus. However, very little is known about the underlying electrophysiology in humans. Here, using a rare opportunity to directly record from the human thalamus, we identify a hitherto-unreported brain-state-specific oscillation of approximately 19-45 Hz. This oscillation is present only during Rapid Eye Movement (REM) sleep and wakefulness, while being absent during Non-REM sleep. The 19-45 oscillation further distinguishes REM sleep microstates, co-occurring with bursts of eye movements, and is specific to the Central Thalamus, a structure implicated in causing global brain state transitions. The discovery of a distinct oscillatory signature in the Central Thalamus that distinguishes conscious states opens up avenues to further investigate thalamic contributions to states of consciousness in humans and potentially to refine interventions to treat disorders of consciousness.

---

## 论文详细总结（自动生成）

这篇论文题为《Thalamic oscillations distinguish natural states of consciousness in humans》，发表于 *bioRxiv*（2025年5月版本）。以下是对该研究的结构化总结：

### 1. 核心问题与整体含义
*   **研究动机**：丘脑被认为是调节意识状态（如清醒、睡眠）的核心结构，但由于获取人类丘脑直接电生理记录的机会极少，科学界对人类丘脑在不同意识状态下的底层电生理特征知之甚少。
*   **核心问题**：是否存在特定的丘脑振荡模式能够区分人类的自然意识状态（清醒、REM睡眠、NREM睡眠）？
*   **整体含义**：研究发现了一种此前未被报道的、频率在 **19-45 Hz** 之间的快速丘脑振荡，它特异性地出现在清醒和快速眼动（REM）睡眠中，而在非快速眼动（NREM）睡眠中消失。这一发现为理解意识的神经机制提供了关键的电生理指标。

### 2. 方法论
*   **核心思想**：利用癫痫患者植入深部脑刺激（DBS）电极后的外化记录期，直接获取丘脑场电位（LFP），并结合头皮EEG进行多模态分析。
*   **关键技术细节**：
    *   **爆发检测算法（Burst Detection）**：开发了一种无需预设频段的自适应算法。通过 Morlet 小波变换生成时频图，识别振幅超过中位数 3 倍且持续至少 5 个周期的信号，从而区分真正的振荡与宽带噪声。
    *   **睡眠分期**：依据 AASM 标准，利用头皮 EEG 对清醒、NREM（N2+N3）和 REM 阶段进行人工标注。
    *   **眼动检测**：利用额叶 EEG 通道（F7-F8）的电压变化率自动检测 REM 睡眠期间的快速眼动（EM）。
    *   **解剖定位**：结合术前 MRI 和术后 CT，利用 LeadDBS 和 Freesurfer 算法将电极触点精确映射到丘脑子核团（如中央丘脑、前腹核 AV 等）。

### 3. 实验设计
*   **数据集/对象**：17 名药物难治性癫痫患者，均在丘脑前核（ANT）区域植入双侧 DBS 电极。
*   **场景**：中位时长约 40 小时的连续记录，涵盖完整的昼夜觉醒-睡眠周期。
*   **对比维度**：
    *   **状态对比**：清醒 vs. REM vs. NREM。
    *   **微状态对比**：REM 睡眠中的相位性（Phasic，伴随眼动）vs. 紧张性（Tonic，无眼动）。
    *   **解剖对比**：中央丘脑（Central Thalamus）邻近区域 vs. 其他丘脑核团（如 AV 核）。
*   **Benchmark**：以 NREM 睡眠中已知的纺锤波（11-17 Hz）作为基准对照，验证记录质量和算法有效性。

### 4. 资源与算力
*   **算力说明**：论文未明确提及具体的 GPU 型号或训练时长。
*   **软件工具**：分析主要基于 Python 环境，使用了 MNE-Python（脑电处理）、Scikit-learn（逻辑回归）、FOOOF（功率谱分解）等开源工具。

### 5. 实验数量与充分性
*   **实验规模**：分析了 105 个丘脑双极通道的数据。
*   **统计充分性**：
    *   使用了**块自助法（Block Bootstrapping）**在群体水平上估计不确定性，确保结果不受个别患者影响。
    *   对 14 名检测到快速振荡的患者进行了深入的 REM 微状态相关性分析。
    *   进行了逻辑回归分析，验证解剖位置与信号检测概率的关系。
*   **客观性**：实验设计包含了对非周期性信号（1/f）的剔除，并对谐波干扰进行了严格过滤，实验结论较为客观、公平。

### 6. 主要结论与发现
*   **发现新振荡**：在人类丘脑中发现 19-45 Hz 振荡，该信号是清醒和 REM 睡眠的共同特征，但在 NREM 睡眠中显著缺失。
*   **REM 微状态关联**：该振荡的爆发频率与 REM 睡眠中的眼动爆发高度同步，能够区分相位性 REM 和紧张性 REM。
*   **解剖特异性**：该振荡主要源于**中央丘脑**。电极距离中央丘脑越近，检测到该信号的概率越高。
*   **功能连接**：在清醒和 REM 期间，丘脑与皮层在该频段表现出显著增强的功能连接（wPLI 指标）。
*   **唤醒关联**：在部分患者中观察到该振荡频率与瞳孔直径（唤醒水平的指标）呈正相关。

### 7. 亮点
*   **数据稀缺性**：直接获取人类丘脑内部的长期电生理数据，具有极高的学术价值。
*   **算法鲁棒性**：自适应爆发检测算法有效解决了不同个体间振荡频率存在差异的问题。
*   **临床启示**：为意识障碍（DOC）患者的 DBS 治疗提供了潜在的反馈信号和刺激频率参考。

### 8. 不足与局限
*   **样本偏差**：受试者均为癫痫患者，虽然通过多种统计手段排除了癫痫放电的影响，但其丘脑回路可能与健康人存在差异。
*   **EEG 覆盖限制**：头皮 EEG 电极数量有限且分布稀疏，难以精确描绘丘脑振荡在皮层的完整投影图。
*   **因果性缺失**：目前的研究属于观察性研究，尚未通过干预手段（如直接刺激该频段）证明该振荡对意识状态转换的因果作用。
*   **意识内容**：研究仅关注意识的“状态”（State），未涉及意识的“内容”（Content，如梦境的具体感知）。

（完）
