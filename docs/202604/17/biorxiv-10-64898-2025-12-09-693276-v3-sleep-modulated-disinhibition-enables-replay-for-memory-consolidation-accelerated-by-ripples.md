---
title: "Sleep-modulated disinhibition enables replay for memory consolidation, accelerated by ripples"
title_zh: 睡眠调节的去抑制促进记忆巩固中的重现，并由波纹波加速
authors: "Dutta, S."
date: 2026-04-11
pdf: "https://www.biorxiv.org/content/10.64898/2025.12.09.693276v3.full.pdf"
tags: ["query:slp-ns"]
score: 9.0
evidence: 慢波睡眠与记忆巩固的神经机制
tldr: 本研究通过构建内嗅皮层-海马-皮层网络的生物物理模型，揭示了去抑制（disinhibition）在记忆巩固中的核心作用。研究发现，睡眠期间神经调制引起的去抑制触发了神经元重现（replay）和尖波波纹（ripples），促进了记忆从海马向皮层的转移。研究表明，虽然波纹能加速巩固过程，但去抑制才是驱动重现和系统整合的关键机制，这一发现为理解记忆形成及治疗记忆障碍提供了新视角。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2025-12-09-693276-v3/fig-001.webp\", \"caption\": \"Fig 2: Transition to slow-wave sleep activates K+-dependent disinhibition that enables spontaneous time-compressed replay via inter-assembly delay. a Time courses of average extracellular K+, 〈 [K+]o 〉 , and average firing rate of entorhinal and hippocampal regions. Top: Temporal evolution of ⟨[K+]o⟩ from ‘Background’ neurons when [K+]Buffer is decreased from 3.5 to 3.0 mM at 100 s to initiate the transition from ‘awake’ to ‘slow-wave sleep’ dynamics. Middle & bottom: Average firing rates, ⟨ψ⟩, during normal MEC dynamics (middle) and during silenced MEC dynamics by enhanced inhibition (bottom). Arrows labeled ‘b’ to ‘g’ point to the timestamps of rasters in panels b to g. b–g Top: 1200 ms raster plot of spikes from all neurons at the respective timestamps from panel a. Bottom: Zoom of the 400 ms box from the top panel showing exemplars of replays with lengths 2–4. h Bar plot showing the logarithm of total number of CA1 replays of lengths 2–4 during time-courses in panel a. i Left: Sequential replay with inter-assembly delay. Right: Disrupted replay sequence without inter-assembly delay. Colors represent brain regions as in Fig. 1.\", \"page\": 6, \"index\": 1, \"width\": 940, \"height\": 794}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2025-12-09-693276-v3/fig-002.webp\", \"caption\": \"Fig 6: Disabling K+-dependent CA1 disinhibition underlies MEC-input-dependent quiet wakefulness replay through MEC-mediated disinhibition. a,b Row 1: Schematics of feedforward excitatory inputs (arrows) from MEC and CA3 (column 1), CA3-only (column 2), or MEC-only (column 3) to CA1 excitatory and inhibitory neurons; absent (panel a) or present (panel b) inhibitory link (round arrowheads) from MEC- to CA3-receiving CA1 interneurons (I1 → I2 = 50), enabling MEC-mediated disinhibition of excitatory CA1 neurons and gating CA3 input to CA1. Rows 2–7: Replay dynamics, with K+-dependent disinhibition enabled (rows 2–4) or disabled (rows 5–7), in 300-ms raster plots (rows 2, 5), CA1 local field potentials (rows 3, 6), and time– frequency analyses (rows 4, 7). Colors denote brain regions as in Fig. 1.\", \"page\": 10, \"index\": 2, \"width\": 939, \"height\": 798}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2025-12-09-693276-v3/fig-003.webp\", \"caption\": \"Fig 4: Different levels of lateral inhibition unify ripple diversity. a Mean power of CA1 ripple-associated replays (all lengths, including 1) increases as lateral inhibition (LI) decreases, computed over 200-s simulations. b 300-ms raster plot (row 1), CA1 local field potential (row 2), and CA1 frequency-time analysis (row 3) at 100% LI (ripple chain; left), 50% LI (long-duration ripple; middle), and 0% LI (pathological ripple; right). MEC is silenced to eliminate its inputs to CA3 and CA1, thereby isolating CA3 modulation of CA1. Colors represent brain regions as in Fig. 1.\", \"page\": 8, \"index\": 3, \"width\": 924, \"height\": 248}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2025-12-09-693276-v3/fig-004.webp\", \"caption\": \"Fig 1: Entorhinal-hippocampal-cortical circuit model, awake/sleep dynamics, and stimulation-driven encoding. a Left: Schematic of the entorhinal-hippocampal-cortical circuit driven by background neural activity. Brain regions: medial entorhinal cortex (MEC, green), dentate gyrus (DG, yellow), CA3 (purple), CA1 (red), cortical regions (CR, blue-green), unmodeled brain regions (Background, black). Black solid arrows denote effective pre-encoding connections (MEC→DG, MEC→CA3, MEC→CA1, CA3→CA1). Gray solid arrow (CA1→CR) indicates anatomical connection with strong feedforward inhibition during wakefulness. Dashed arrows show ineffective (weak) pre-encoding connections (DG→CA3; recurrent in MEC, CA3, CR). Lightning bolt on MEC signifies stimulation initiating encoding. Right top: Dynamic synaptic updates for feedforward inhibition. Neurons: presynaptic excitatory (‘pre’, unfilled circle), postsynaptic excitatory (‘post’, unfilled circle) or inhibitory (gray filled circle). Updates: ∆w± from ‘pre’ to excitatory ‘post’ drives A∆w± to ‘pre’→inhibitory ‘post’ and B∆w± to inhibitory ‘post’→excitatory ‘post’, where A = a/M , B = b/M , M is the number of interneurons in the feedforward inhibition path from ‘pre’ to ‘post’, and a, b are scaling constants. Right bottom: Dynamic synaptic updates for feedback and lateral inhibition. Neurons: excitatory in the assembly of ‘post’ (‘self’, middle unfilled circle), in other assemblies (‘other’, left/right unfilled circles), assembly-specific inhibitory neuron (ASIN, filled circle). Updates: ∆w± to ‘post’ drives c∆w± to ‘post’→ASIN, D∆w± to ASIN→‘self’ (feedback), F∆w± to ASIN→‘other’ (lateral), where D = d/N , F = f/N , N is the number of neurons in the assembly, and c, d, f are scaling constants. Arrows: excitatory; round arrowheads: inhibitory. b Extracellular potassium buffer ([K+]Buffer) decrease (3.5 to 3.0 mM) transitions the dynamics from ‘awake’ to ‘slow-wave sleep’ via disinhibition. Top: Raster plots of spikes from 435 neurons (1–336 excitatory, 337–435 inhibitory) showing ‘awake’ (asynchronous-irregular; left) and ‘slow-wave sleep’ (up-down; right) dynamics before encoding. Bottom: Respective local field potential activity, (Φ), from ‘Background’ neurons. Gray lines trace the upper and lower envelopes. c Top: Stimulation pattern mimicking exploration from locations A to D with phase precession for 16 MEC neurons over 1.125 s. Each gray 8-Hz cycle (9 cycles, 125 ms each) is organized into four phases, with colored letters (blue A, orange B, green C, pink D: locations; black X: none) marking burst stimulation (three spikes) in the four neurons of each location-specific cell assembly, advancing to earlier phases with successive cycles. Bottom: Raster plot over 5 s during four complete stimulations of locations (MEC cell assemblies in green) ‘A’ to ‘D’. Inhibitory neurons at top with gray shading. Background activity (black) is asynchronous irregular (‘awake’). MEC stimulation drives downstream activity via effective connections (panel a). Inset: Zoomed view of the latter part of the second stimulation (boxed), showing delayed activation in downstream regions for locations C and D. d Top: Time course of changes (∆) in mean excitatory-to-excitatory synaptic weights for connections in panel a during stimulation-driven encoding (⟨∆w⟩, solid: fast overall [labile + stable] governed by spike-timing-dependent plasticity; ⟨∆w̃⟩, dashed: slow stable governed by protein-mediated stabilization; ⟨∆w⟩ − ⟨∆w̃⟩, shading: labile component). The 5-min stimulation period (from 30 s to 330 s) represents repeated sequential exploration of locations ‘A’ to ‘D’. Middle & bottom: Matrices showing overall weights, w, between neurons before (middle) and after (bottom) the stimulation-driven encoding; white indicates no connection.\", \"page\": 4, \"index\": 4, \"width\": 941, \"height\": 794}]"
motivation: 旨在探索记忆巩固过程中神经元重现和系统整合背后的具体生物物理机制。
method: 开发了一个包含内嗅皮层、海马和皮层的高精度生物物理网络模型，模拟不同神经调制状态下的神经活动。
result: 发现去抑制机制驱动了空间序列的自发重现，且皮层去抑制是实现海马向皮层记忆转移的关键。
conclusion: 去抑制是记忆巩固的核心驱动力，它通过协调重现和波纹活动促进海马独立性，为记忆障碍的治疗提供了潜在靶点。
---

## 摘要
记忆巩固涉及复杂的神经机制。本研究开发了一个生物物理细节丰富的内嗅皮层-海马-皮层网络模型，揭示了去抑制驱动突触和系统巩固。通过神经调节减弱抑制作用向慢波睡眠过渡，会产生上下状态以及对相位前移编码的空间序列进行自发且时间压缩的重现。侧向抑制水平统一了生理性和病理性波纹波（ripples）的多样性。皮层去抑制实现了记忆从海马的转移。减弱的传入 CA1 突触消除了波纹波但保留了重现，这为减轻波纹波干扰提出了策略。即使没有波纹波，重现也能维持系统巩固，尽管速度较慢；过度的减弱会导致巩固停止，但可以通过增强海马到皮层的连接性来挽救。内侧内嗅皮层（MEC）介导的 CA1 去抑制补偿了减弱的神经调节 CA1 去抑制，模拟了依赖于 MEC 输入的安静觉醒重现；在觉醒期间的这种配置下，人工诱导去抑制会触发驱动巩固的重现和波纹波，强调了去抑制在不同状态下的普适作用。这些见解阐明了去抑制在铭刻记忆和促进海马独立性方面的核心地位，调和了实验观察结果，提出了可测试的预测，并为记忆障碍确定了治疗途径。

## Abstract
Memory consolidation involves elusive neural mechanisms. Here, we develop a biophysically detailed model of the entorhinal-hippocampal-cortical network to reveal that disinhibition drives synaptic and systems consolidation. Transitioning to slow-wave sleep via neuromodulatory dampening of inhibition generates up-down states and spontaneous, time-compressed replays of spatial sequences encoded with phase precession. Lateral inhibition levels unify physiological and pathological ripple diversity. Cortical disinhibition enables memory transfer from hippocampus. Weakened afferent CA1 synapses eliminate ripples but spare replays, proposing strategies to mitigate ripple disruptions. Replays sustain systems consolidation even without ripples, albeit slower; excessive weakening halts it, rescuable by enhanced hippocampal-to-cortical connectivity. Medial entorhinal cortex (MEC)-mediated CA1 disinhibition compensates for attenuated neuromodulatory CA1 disinhibition, mimicking MEC-input-dependent quiet wakefulness replay; under this configuration during wakefulness, artificially inducing disinhibition triggers replays and ripples that drive consolidation, underscoring disinhibitions state-agnostic role. These insights elucidate disinhibitions centrality in engraining memories and fostering hippocampal independence, reconciling empirical observations, yielding testable predictions, and identifying therapeutic avenues for memory disorders.

---

## 论文详细总结（自动生成）

这是一份关于论文《Sleep-modulated disinhibition enables replay for memory consolidation, accelerated by ripples》（睡眠调节的去抑制促进记忆巩固中的重现，并由波纹波加速）的深度结构化总结：

### 1. 核心问题与整体含义（研究动机和背景）
*   **核心问题**：探索记忆巩固（Memory Consolidation）过程中，神经元“重现”（Replay）和“尖波波纹”（SWRs/Ripples）产生的具体生物物理机制，以及它们如何协同工作将记忆从海马体转移到大脑皮层。
*   **背景**：虽然已知睡眠期间的重现对记忆至关重要，但究竟是什么触发了这些自发的、时间压缩的序列活动，以及波纹波在其中扮演的是“驱动者”还是“加速器”角色，学术界尚存争议。

### 2. 方法论：核心思想与关键技术
*   **核心思想**：提出**“去抑制”（Disinhibition）**是驱动记忆巩固的核心引擎。研究认为，睡眠期间神经调制（如乙酰胆碱水平下降）导致的抑制性神经元活动减弱，释放了被编码的兴奋性神经元组合，从而触发重现。
*   **关键技术细节**：
    *   **多区域生物物理模型**：构建了一个包含内嗅皮层（MEC）、齿状回（DG）、CA3、CA1及皮层区域（CR）的大规模网络模型。
    *   **突触可塑性**：结合了基于脉冲计时的突触可塑性（STDP）和蛋白质介导的突触标记与捕获（STC）机制，模拟短期和长期记忆的形成。
    *   **神经调制模拟**：通过调节细胞外钾离子浓度（$[K^+]_o$）和抑制性突触强度，模拟从觉醒到慢波睡眠（SWS）的转换。
    *   **去抑制机制**：模型详细刻画了前馈抑制、反馈抑制和侧向抑制（Lateral Inhibition）在不同睡眠/觉醒状态下的动态变化。

### 3. 实验设计与对比
*   **场景模拟**：
    *   **编码阶段**：模拟大鼠在空间探索时的相位前移（Phase Precession）活动，将空间序列编码进突触权重。
    *   **巩固阶段**：模拟慢波睡眠和安静觉醒（Quiet Wakefulness）状态，观察自发重现。
*   **对比实验（消融实验）**：
    *   **有无波纹波对比**：通过削弱 CA3 到 CA1 的突触强度消除波纹波，观察重现和皮层学习是否依然存在。
    *   **抑制水平对比**：调节侧向抑制强度，观察其对生理性波纹与病理性波纹（如癫痫样放电）的影响。
    *   **输入源对比**：对比 MEC 输入驱动与海马自发驱动的重现机制。
*   **Benchmark**：以已发表的电生理实验数据（如重现的时间压缩倍数、波纹波频率等）作为验证模型准确性的基准。

### 4. 资源与算力
*   **算力说明**：论文中**未明确提及**具体的 GPU 型号、数量或总训练时长。
*   **实现方式**：通常此类生物物理模拟使用专门的神经元网络模拟器（如 NEURON, Brian2 或自定义 C++/Python 代码），计算量取决于神经元数量和模拟的生物学时长（文中模拟了长达数十分钟的巩固过程）。

### 5. 实验数量与充分性
*   **实验规模**：研究进行了多维度的参数扫描，包括抑制强度、突触权重、离子浓度等。
*   **充分性评价**：实验设计非常**充分且系统**。作者不仅模拟了正常的生理状态，还通过“病理性”参数设置验证了模型的边界（如侧向抑制缺失导致的病理性波纹）。
*   **客观性**：通过模拟多种实验观察到的现象（如安静觉醒下的重现、MEC 损伤的影响），证明了模型的普适性和客观性。

### 6. 主要结论与发现
*   **去抑制是关键**：睡眠诱导的去抑制是触发自发重现的必要条件，它允许神经元组合按编码顺序依次放电。
*   **波纹波的作用**：波纹波并非重现的先决条件，而是重现的“加速器”。即使没有波纹波，重现也能驱动皮层巩固，但效率较低。
*   **皮层独立性**：皮层的去抑制使得海马的重现能够有效地“教导”皮层，最终实现记忆的海马独立性。
*   **统一框架**：通过调节侧向抑制水平，可以统一解释从正常波纹到长时程波纹、再到病理性尖峰的多种现象。

### 7. 优点
*   **机制解释力强**：为“重现是如何自发产生的”这一经典问题提供了一个清晰的生物物理学解释（去抑制+组合间延迟）。
*   **跨状态统一性**：成功将慢波睡眠和安静觉醒下的重现机制统一在“去抑制”框架下。
*   **临床关联**：模型对病理性波纹的模拟为理解记忆障碍和癫痫提供了理论基础。

### 8. 不足与局限
*   **模型简化**：尽管细节丰富，但仍简化了某些生物学特性（如未详细区分所有类型的抑制性中间神经元）。
*   **空间维度限制**：主要关注一维空间序列的重现，对于更复杂的二维环境或非空间记忆的适用性有待进一步验证。
*   **预测验证**：部分理论预测（如特定抑制性神经元的精确调控对巩固的影响）仍需未来的光遗传学实验进一步证实。

（完）
