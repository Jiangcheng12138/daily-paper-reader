---
title: Nighttime sleep promotes mechanosensory habituation in Drosophila
title_zh: 夜间睡眠促进果蝇的机械感觉习惯化
authors: "Lowe, S. A., Wilson, A. D., Chen, K.-F., Jepson, J. E."
date: 2026-04-29
pdf: "https://www.biorxiv.org/content/10.1101/2025.11.17.688779v2.full.pdf"
tags: ["query:slp-ns"]
score: 9.0
evidence: 睡眠促进果蝇的记忆和习惯化
tldr: 本研究探讨了睡眠对果蝇非联合学习（习惯化）的影响。通过自动化机械刺激系统，研究发现缺乏神经钙传感器 Neurocalcin 的果蝇因夜间睡眠不足导致白天习惯化受损。通过睡眠压缩疗法恢复其夜间睡眠可修复该缺陷。研究表明，夜间睡眠通过促进感觉回路中的突触下调来增强习惯化能力，揭示了睡眠在基础记忆形式中的关键作用。
source: biorxiv
selection_source: fresh_fetch
motivation: 探究睡眠是否以及如何影响生物体最基础的非联合学习形式——习惯化。
method: 利用自动化系统对果蝇进行长期的机械刺激习惯化测量，并结合 Neurocalcin 突变体及睡眠干预手段进行实验。
result: 发现夜间睡眠不足会损害白天的习惯化能力，而通过增加夜间睡眠或睡眠压缩疗法可以恢复或增强这种能力。
conclusion: 夜间睡眠通过促进感觉回路的突触下调来增强机械刺激习惯化，证明了睡眠对非联合记忆的重要性。
---

## 摘要
睡眠是一种高度保守的行为，它促进了跨物种的情景记忆、程序性记忆和/或关联性记忆模式，这一过程被假设涉及觉醒期间增强的突触的结构性下调。习惯化是一种古老的非关联性记忆形式，其中刺激的重复会导致行为反应减弱，它被认为是此类复杂学习形式的前提。然而，睡眠是否也影响生物体的习惯化能力尚不清楚。在本研究中，我们利用果蝇（Drosophila）探讨了这一问题。我们描述了一个自动化系统，该系统可以对成年果蝇对机械刺激的习惯化进行长期模拟测量。利用该平台，我们发现缺乏神经元钙传感器 Neurocalcin 的果蝇（其表现为夜间睡眠特异性减少）在白天的机械感觉习惯化受损。通过模拟一种治疗失眠的方法，我们证明压缩夜间时长既能恢复 Neurocalcin 突变体的巩固性夜间睡眠，又能使习惯化恢复正常。相反，在没有睡眠缺陷的野生型果蝇中，缩短夜间长度会减少总夜间睡眠并破坏白天的习惯化。在野生型果蝇中，暴露于更长的夜晚会增加总体的夜间睡眠，并增强感觉回路中的突触下调。显著的是，这种效应在 Neurocalcin 突变体中消失了，因为它们在这些条件下并未表现出睡眠增加。总之，我们的研究结果揭示了夜间睡眠在促进习惯化中的作用，并表明这可能是通过促进突触下调实现的。

## Abstract
Sleep is a highly conserved behaviour that facilitates episodic, procedural, and/or associative modes of memory across species, a process hypothesised to involve structural downscaling of synapses potentiated during waking episodes. Habituation, an ancient form of non-associative memory in which repetition of a stimulus leads to diminishing behavioural responses, is considered a prerequisite for such complex forms of learning. Yet whether sleep also influences the capacity of organisms to habituate is poorly understood. Here we examine this question using the fruit fly, Drosophila. We describe an automated system that yields long-term analogue measurements of habituation to mechanosensory stimuli in adult flies. Using this platform, we find that Drosophila lacking neuronal calcium sensor Neurocalcin, which exhibit reduced sleep specifically during the night, display impaired mechanosensory habituation during the day. Mimicking a method used to treat insomnia, we show that compressing nighttime duration both restores consolidated night sleep and renormalises habituation in Neurocalcin mutants. Conversely, in wild type flies without sleep deficits, decreasing night length reduces total night sleep and disrupts daytime habituation. In wild type flies, exposure to longer nights, which increases overall night sleep, enhances synaptic downscaling in sensory circuits. Strikingly, this effect is abolished in Neurocalcin mutants, which do not exhibit increased sleep under these conditions. Collectively, our findings reveal a role for nighttime sleep in facilitating habituation and suggest that this may occur by promoting synaptic downscaling.

---

## 论文详细总结（自动生成）

这是一份关于论文《Nighttime sleep promotes mechanosensory habituation in *Drosophila*》（夜间睡眠促进果蝇的机械感觉习惯化）的结构化深入总结：

### 1. 核心问题与整体含义
*   **研究动机**：睡眠对关联性记忆（如条件反射）和复杂学习的促进作用已广为人知，其核心机制被认为是“突触稳态假设”（SHY），即睡眠通过下调觉醒期间增强的突触来维持神经系统平衡。然而，**习惯化（Habituation）**作为一种最基础、最古老的非关联性记忆形式（对重复无关刺激的反应减弱），是否也受睡眠调节尚不明确。
*   **核心问题**：夜间睡眠质量是否直接影响生物体在白天的习惯化能力？其背后的神经生物学机制（如突触下调）是什么？

### 2. 方法论
*   **核心思想**：利用果蝇作为模型生物，通过遗传学手段特异性干扰夜间睡眠，并开发高通量自动化系统定量测量机械感觉习惯化，进而观察睡眠与习惯化之间的因果关系。
*   **关键技术细节**：
    *   **DART 系统（Drosophila ARousal Tracking）**：结合视频追踪与电机驱动，以 10 分钟为间隔发送 20 次相同的机械振动刺激，记录果蝇的运动反应衰减。
    *   **遗传模型**：使用 **Neurocalcin (Nca)** 缺失突变体。该突变体的独特之处在于它仅在夜间表现出睡眠减少和碎片化，而白天睡眠正常，是研究夜间睡眠功能的理想模型。
    *   **睡眠压缩疗法（Sleep Restriction Therapy）**：模拟人类失眠治疗，通过缩短光照周期中的夜晚时长（如从 16h 缩短至 8h），强制提高睡眠效率，观察其对突变体行为的修复作用。
    *   **突触成像**：利用免疫荧光技术定量分析脑部突触活性区蛋白 **Bruchpilot (BRP)** 的表达水平，作为突触强度的分子指标。

### 3. 实验设计
*   **实验场景**：受控的实验室环境，利用 DART 和 Zantiks 两种不同的自动化平台进行交叉验证。
*   **Benchmark 与对比对象**：
    *   **对照组**：野生型果蝇（iso31）。
    *   **实验组**：两种独立的 *Nca* 零突变体（$Nca^{KO1}$ 和 $Nca^{KO2}$）。
    *   **环境干预**：长夜（L8:D16） vs 短夜（L16:D8）环境。
    *   **刺激特异性测试**：在机械刺激习惯化后引入视觉刺激（Lights-off），验证反应减弱是由于习惯化而非疲劳或感觉损伤。
*   **验证维度**：自发恢复测试、重复训练后的习惯化增强测试、不同刺激强度的敏感度测试。

### 4. 资源与算力
*   **硬件设备**：使用了 DART 系统、Zantiks MWP 单元、DAM5H（多射线果蝇活动监测器）以及 Zeiss LSM 980 共聚焦显微镜。
*   **算力说明**：论文未涉及深度学习或大规模计算模拟，因此未提及 GPU 型号或训练时长。数据处理主要依赖于 DART 软件、ImageJ 图像分析和 R 语言（phaseR 包）进行统计分析。

### 5. 实验数量与充分性
*   **实验规模**：每组实验通常包含 20-80 只果蝇，涵盖了多个独立的生物学重复。
*   **充分性评价**：
    *   **非常充分**：研究不仅观察了现象，还通过“睡眠压缩”进行了功能恢复实验，并从分子层面（BRP 蛋白）提供了机制解释。
    *   **客观公平**：使用了两种独立的突变体品系排除背景干扰；通过视觉刺激实验排除了运动疲劳的干扰；采用了跨平台（DART 和 Zantiks）验证，确保了结果的稳健性。

### 6. 主要结论与发现
*   **睡眠促进习惯化**：夜间睡眠不足（*Nca* 突变体）会导致白天的机械感觉习惯化显著受损。
*   **睡眠质量是关键**：通过缩短夜晚时长来“压缩”并巩固夜间睡眠，可以完全修复 *Nca* 突变体的习惯化缺陷。
*   **突触下调机制**：在野生型中，长夜（睡眠多）会导致感觉回路（如触角叶）中 BRP 蛋白水平下降（突触下调）；而 *Nca* 突变体由于夜间睡眠质量差，无法实现这种下调，导致突触水平维持在高位，从而阻碍了习惯化的形成。
*   **双向关系**：缩短野生型果蝇的夜间睡眠同样会损害其白天的习惯化能力。

### 7. 优点与亮点
*   **行为学创新**：开发并验证了一套高通量的成年果蝇机械习惯化定量评价体系，填补了该领域的研究空白。
*   **临床相关性**：巧妙地将人类失眠的“睡眠限制疗法”应用于果蝇模型，证明了睡眠巩固（而非单纯的时长）对认知功能的重要性。
*   **机制深入**：将宏观的行为表现与微观的突触稳态（SHY 假设）联系起来，提供了从基因到行为的完整逻辑链。

### 8. 不足与局限
*   **回路特异性有待加强**：虽然观察到了触角叶（嗅觉中枢）的突触变化，但对于直接介导“机械感觉-运动”的具体神经回路尚未完全定位。
*   **性别偏差**：实验主要在雄性果蝇中进行，尚未探讨睡眠对雌性果蝇习惯化影响是否存在性别差异。
*   **因果链条的细节**：虽然证明了睡眠与突触下调的相关性，但尚未通过光遗传学等手段在睡眠期间直接人为诱导突触下调来观察是否能替代睡眠的作用。

（完）
