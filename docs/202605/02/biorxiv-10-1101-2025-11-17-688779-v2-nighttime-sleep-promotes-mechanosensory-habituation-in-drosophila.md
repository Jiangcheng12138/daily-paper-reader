---
title: Nighttime sleep promotes mechanosensory habituation in Drosophila
title_zh: 夜间睡眠促进黑腹果蝇的机械感觉习惯化
authors: "Lowe, S. A., Wilson, A. D., Chen, K.-F., Jepson, J. E."
date: 2026-04-29
pdf: "https://www.biorxiv.org/content/10.1101/2025.11.17.688779v2.full.pdf"
tags: ["query:slp-ns"]
score: 9.0
evidence: 夜间睡眠促进机械感觉习惯化
tldr: 本研究探讨了睡眠对果蝇非联合型记忆（习惯化）的影响。通过开发自动化机械感觉习惯化测量系统，研究发现缺乏Neurocalcin蛋白且夜间睡眠不足的果蝇，其白天的习惯化能力显著受损。通过压缩夜间时长以巩固睡眠，可恢复突变体的习惯化能力；而缩短野生型果蝇的睡眠则会破坏该能力。研究表明，充足的夜间睡眠能促进感觉回路的突触下调，从而增强习惯化学习，揭示了睡眠在基础学习过程中的关键作用。
source: biorxiv
selection_source: fresh_fetch
motivation: 探究睡眠是否以及如何影响生物体最基础的学习形式——非联合型学习（习惯化）。
method: 利用自动化系统对果蝇进行长期的机械感觉习惯化测量，并结合Neurocalcin突变体及睡眠干预手段进行实验。
result: 发现夜间睡眠不足会导致果蝇白天的习惯化能力受损，而通过增加或巩固夜间睡眠可恢复该能力并促进突触下调。
conclusion: 夜间睡眠通过促进感觉回路中的突触下调，在增强果蝇的习惯化学习中发挥着关键作用。
---

## 摘要
睡眠是一种高度保守的行为，在不同物种中促进情景记忆、程序性记忆和/或联想记忆，这一过程被假设涉及清醒期间增强的突触的结构性下调。习惯化是一种古老的非联想记忆形式，其中刺激的重复导致行为反应减弱，被认为是此类复杂学习形式的前提。然而，睡眠是否也影响生物体的习惯化能力尚不清楚。在本研究中，我们利用黑腹果蝇（Drosophila）探讨了这一问题。我们描述了一个自动化系统，该系统可对成年果蝇对机械刺激的习惯化进行长期模拟测量。利用该平台，我们发现缺乏神经元钙传感器 Neurocalcin 的果蝇（其夜间睡眠特异性减少）在白天的机械感觉习惯化表现出受损。通过模仿治疗失眠的方法，我们证明压缩夜间时长既能恢复巩固的夜间睡眠，又能使 Neurocalcin 突变体的习惯化恢复正常。相反，在没有睡眠缺陷的野生型果蝇中，缩短夜间长度会减少总夜间睡眠并破坏白天的习惯化。在野生型果蝇中，延长夜间时长以增加总夜间睡眠，会增强感觉回路中的突触下调。显著的是，这种效应在 Neurocalcin 突变体中消失了，因为它们在这些条件下并未表现出睡眠增加。总之，我们的研究结果揭示了夜间睡眠在促进习惯化中的作用，并表明这可能是通过促进突触下调实现的。

## Abstract
Sleep is a highly conserved behaviour that facilitates episodic, procedural, and/or associative modes of memory across species, a process hypothesised to involve structural downscaling of synapses potentiated during waking episodes. Habituation, an ancient form of non-associative memory in which repetition of a stimulus leads to diminishing behavioural responses, is considered a prerequisite for such complex forms of learning. Yet whether sleep also influences the capacity of organisms to habituate is poorly understood. Here we examine this question using the fruit fly, Drosophila. We describe an automated system that yields long-term analogue measurements of habituation to mechanosensory stimuli in adult flies. Using this platform, we find that Drosophila lacking neuronal calcium sensor Neurocalcin, which exhibit reduced sleep specifically during the night, display impaired mechanosensory habituation during the day. Mimicking a method used to treat insomnia, we show that compressing nighttime duration both restores consolidated night sleep and renormalises habituation in Neurocalcin mutants. Conversely, in wild type flies without sleep deficits, decreasing night length reduces total night sleep and disrupts daytime habituation. In wild type flies, exposure to longer nights, which increases overall night sleep, enhances synaptic downscaling in sensory circuits. Strikingly, this effect is abolished in Neurocalcin mutants, which do not exhibit increased sleep under these conditions. Collectively, our findings reveal a role for nighttime sleep in facilitating habituation and suggest that this may occur by promoting synaptic downscaling.

---

## 论文详细总结（自动生成）

这篇论文探讨了睡眠与最基础的学习形式——**习惯化（Habituation）**之间的因果关系。以下是对该研究的结构化总结：

### 1. 核心问题与整体含义
*   **研究动机**：睡眠对复杂记忆（如联想记忆）的巩固作用已广为人知，其核心机制被认为是“突触稳态假设”（SHY），即睡眠通过下调清醒时增强的突触连接来维持神经系统平衡。然而，作为所有学习基础的“非联想记忆”——习惯化，是否也受睡眠调节，目前尚不清楚。
*   **核心问题**：夜间睡眠质量是否直接影响生物体在白天的机械感觉习惯化能力？

### 2. 方法论
*   **核心思想**：通过遗传学手段特异性干扰夜间睡眠，并结合高通量自动化行为监测系统，量化习惯化速率与睡眠质量的相关性。
*   **关键技术细节**：
    *   **DART 系统**：利用“果蝇唤醒追踪”（DART）系统，通过摄像头实时追踪果蝇位移，并由计算机控制电机产生精确的机械振动刺激。
    *   **习惯化协议**：每隔 10 分钟给予一次机械刺激（共 20 次），记录果蝇在刺激后 1 分钟内的平均峰值速度。
    *   **睡眠干预（睡眠限制疗法）**：借鉴人类失眠治疗中的“压缩睡眠时间”方法，通过改变光照周期（如 16h 光照: 8h 黑暗）来巩固突变体的夜间睡眠。
    *   **突触标记量化**：利用免疫荧光技术标记突触前活性区蛋白 Bruchpilot (BRP)，作为突触强度的分子指标。

### 3. 实验设计
*   **实验对象**：黑腹果蝇（野生型 iso31，以及 *Neurocalcin* 基因敲除突变体 $Nca^{KO}$）。
*   **对比场景**：
    *   **长夜环境（L8:D16）**：模拟冬季，突变体在此环境下表现出严重的夜间睡眠碎片化。
    *   **短夜环境（L16:D8）**：模拟夏季，用于测试睡眠巩固对习惯化的修复作用。
*   **Benchmark 与验证**：
    *   通过自发恢复、重复训练增强、刺激特异性（视觉刺激对比）三项指标，验证了该行为下降属于真正的“习惯化”，而非疲劳或损伤。
    *   使用了 **Zantiks MWP** 自动化追踪系统进行跨平台验证，确保结果的可靠性。

### 4. 资源与算力
*   **硬件设备**：实验主要依赖于 DART 系统、Zantiks MWP 系统、DAM5H 多束红外活动监测器以及 Zeiss LSM 980 共聚焦显微镜。
*   **算力说明**：论文未涉及深度学习训练，因此未提及 GPU 算力。数据处理主要涉及视频追踪算法和图像强度定量分析（ImageJ）。

### 5. 实验数量与充分性
*   **实验规模**：
    *   行为学实验样本量充足（每组通常包含 20-80 只果蝇）。
    *   包含了两个独立的 $Nca$ 突变品系（$Nca^{KO1}$ 和 $Nca^{KO2}$）以排除遗传背景干扰。
    *   进行了多维度的消融与对照实验，包括刺激强度敏感性测试、昼夜节律对比、以及不同脑区的免疫组化分析。
*   **评价**：实验设计非常充分且客观。通过“短夜修复实验”成功实现了功能获得（Gain-of-function）式的验证，逻辑链条完整。

### 6. 主要结论与发现
*   **睡眠促进习惯化**：夜间睡眠不足（由 $Nca$ 缺失引起）会导致白天的机械感觉习惯化速率显著减慢。
*   **睡眠质量是关键**：通过压缩夜间时长，虽然总睡眠时间不一定增加，但提高了睡眠的巩固程度，从而恢复了突变体的习惯化能力。
*   **突触下调机制**：在野生型中，长夜（更多睡眠）会导致感觉回路（如触角叶）中 BRP 蛋白水平下降（突触下调）；而睡眠不足的突变体无法完成这一过程，导致突触水平维持在高位，进而阻碍了习惯化的产生。

### 7. 优点与亮点
*   **跨学科借鉴**：巧妙地将人类失眠的临床治疗策略（睡眠限制）应用到果蝇模型中，证明了睡眠质量而非单纯的时长对认知的重要性。
*   **高通量量化**：开发并验证了一套标准化的成年果蝇机械习惯化测量协议，填补了该领域的研究空白。
*   **机制深入**：不仅观察到行为改变，还通过分子标记（BRP）将宏观行为与微观的突触稳态假设联系起来。

### 8. 不足与局限
*   **回路特异性有待明确**：虽然观察到了触角叶（嗅觉中枢）的突触变化，但机械感觉习惯化的核心回路（如介导运动反馈的具体神经元）尚未被完全精确定位。
*   **物种局限性**：虽然习惯化是保守的，但果蝇的睡眠结构与哺乳动物存在差异，结论向人类转化时需谨慎。
*   **性别偏差**：实验主要在雄性果蝇中进行，未讨论是否存在性别差异。

（完）
