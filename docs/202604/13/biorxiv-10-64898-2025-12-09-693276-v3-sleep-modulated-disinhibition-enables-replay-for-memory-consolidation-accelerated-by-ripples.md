---
title: "Sleep-modulated disinhibition enables replay for memory consolidation, accelerated by ripples"
title_zh: 睡眠调节的去抑制使记忆巩固的重现成为可能，并由涟漪波加速
authors: "Dutta, S."
date: 2026-04-11
pdf: "https://www.biorxiv.org/content/10.64898/2025.12.09.693276v3.full.pdf"
tags: ["query:slp-ns"]
score: 10.0
evidence: 慢波睡眠和记忆重现的神经调节机制
tldr: 本研究通过构建内嗅皮层-海马-皮层网络的生物物理详细模型，揭示了去抑制（disinhibition）是驱动记忆巩固的核心机制。研究发现，睡眠期间神经调制引起的抑制减弱会触发自发性序列重现和波纹波，促进记忆从海马向皮层的转移。此外，研究阐明了波纹波对巩固的加速作用，并指出内嗅皮层介导的去抑制在静息觉醒状态下的补偿作用，为理解记忆形成和治疗记忆障碍提供了重要理论依据。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2025-12-09-693276-v3/fig-001.webp\", \"caption\": \"Fig 2: Transition to slow-wave sleep activates K+-dependent disinhibition that enables spontaneous time-compressed replay via inter-assembly delay. a Time courses of average extracellular K+, 〈 [K+]o 〉 , and average firing rate of entorhinal and hippocampal regions. Top: Temporal evolution of ⟨[K+]o⟩ from ‘Background’ neurons when [K+]Buffer is decreased from 3.5 to 3.0 mM at 100 s to initiate the transition from ‘awake’ to ‘slow-wave sleep’ dynamics. Middle & bottom: Average firing rates, ⟨ψ⟩, during normal MEC dynamics (middle) and during silenced MEC dynamics by enhanced inhibition (bottom). Arrows labeled ‘b’ to ‘g’ point to the timestamps of rasters in panels b to g. b–g Top: 1200 ms raster plot of spikes from all neurons at the respective timestamps from panel a. Bottom: Zoom of the 400 ms box from the top panel showing exemplars of replays with lengths 2–4. h Bar plot showing the logarithm of total number of CA1 replays of lengths 2–4 during time-courses in panel a. i Left: Sequential replay with inter-assembly delay. Right: Disrupted replay sequence without inter-assembly delay. Colors represent brain regions as in Fig. 1.\", \"page\": 6, \"index\": 1, \"width\": 940, \"height\": 794}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2025-12-09-693276-v3/fig-002.webp\", \"caption\": \"Fig 6: Disabling K+-dependent CA1 disinhibition underlies MEC-input-dependent quiet wakefulness replay through MEC-mediated disinhibition. a,b Row 1: Schematics of feedforward excitatory inputs (arrows) from MEC and CA3 (column 1), CA3-only (column 2), or MEC-only (column 3) to CA1 excitatory and inhibitory neurons; absent (panel a) or present (panel b) inhibitory link (round arrowheads) from MEC- to CA3-receiving CA1 interneurons (I1 → I2 = 50), enabling MEC-mediated disinhibition of excitatory CA1 neurons and gating CA3 input to CA1. Rows 2–7: Replay dynamics, with K+-dependent disinhibition enabled (rows 2–4) or disabled (rows 5–7), in 300-ms raster plots (rows 2, 5), CA1 local field potentials (rows 3, 6), and time– frequency analyses (rows 4, 7). Colors denote brain regions as in Fig. 1.\", \"page\": 10, \"index\": 2, \"width\": 939, \"height\": 798}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2025-12-09-693276-v3/fig-003.webp\", \"caption\": \"Fig 4: Different levels of lateral inhibition unify ripple diversity. a Mean power of CA1 ripple-associated replays (all lengths, including 1) increases as lateral inhibition (LI) decreases, computed over 200-s simulations. b 300-ms raster plot (row 1), CA1 local field potential (row 2), and CA1 frequency-time analysis (row 3) at 100% LI (ripple chain; left), 50% LI (long-duration ripple; middle), and 0% LI (pathological ripple; right). MEC is silenced to eliminate its inputs to CA3 and CA1, thereby isolating CA3 modulation of CA1. Colors represent brain regions as in Fig. 1.\", \"page\": 8, \"index\": 3, \"width\": 924, \"height\": 248}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2025-12-09-693276-v3/fig-004.webp\", \"caption\": \"Fig 1: Entorhinal-hippocampal-cortical circuit model, awake/sleep dynamics, and stimulation-driven encoding. a Left: Schematic of the entorhinal-hippocampal-cortical circuit driven by background neural activity. Brain regions: medial entorhinal cortex (MEC, green), dentate gyrus (DG, yellow), CA3 (purple), CA1 (red), cortical regions (CR, blue-green), unmodeled brain regions (Background, black). Black solid arrows denote effective pre-encoding connections (MEC→DG, MEC→CA3, MEC→CA1, CA3→CA1). Gray solid arrow (CA1→CR) indicates anatomical connection with strong feedforward inhibition during wakefulness. Dashed arrows show ineffective (weak) pre-encoding connections (DG→CA3; recurrent in MEC, CA3, CR). Lightning bolt on MEC signifies stimulation initiating encoding. Right top: Dynamic synaptic updates for feedforward inhibition. Neurons: presynaptic excitatory (‘pre’, unfilled circle), postsynaptic excitatory (‘post’, unfilled circle) or inhibitory (gray filled circle). Updates: ∆w± from ‘pre’ to excitatory ‘post’ drives A∆w± to ‘pre’→inhibitory ‘post’ and B∆w± to inhibitory ‘post’→excitatory ‘post’, where A = a/M , B = b/M , M is the number of interneurons in the feedforward inhibition path from ‘pre’ to ‘post’, and a, b are scaling constants. Right bottom: Dynamic synaptic updates for feedback and lateral inhibition. Neurons: excitatory in the assembly of ‘post’ (‘self’, middle unfilled circle), in other assemblies (‘other’, left/right unfilled circles), assembly-specific inhibitory neuron (ASIN, filled circle). Updates: ∆w± to ‘post’ drives c∆w± to ‘post’→ASIN, D∆w± to ASIN→‘self’ (feedback), F∆w± to ASIN→‘other’ (lateral), where D = d/N , F = f/N , N is the number of neurons in the assembly, and c, d, f are scaling constants. Arrows: excitatory; round arrowheads: inhibitory. b Extracellular potassium buffer ([K+]Buffer) decrease (3.5 to 3.0 mM) transitions the dynamics from ‘awake’ to ‘slow-wave sleep’ via disinhibition. Top: Raster plots of spikes from 435 neurons (1–336 excitatory, 337–435 inhibitory) showing ‘awake’ (asynchronous-irregular; left) and ‘slow-wave sleep’ (up-down; right) dynamics before encoding. Bottom: Respective local field potential activity, (Φ), from ‘Background’ neurons. Gray lines trace the upper and lower envelopes. c Top: Stimulation pattern mimicking exploration from locations A to D with phase precession for 16 MEC neurons over 1.125 s. Each gray 8-Hz cycle (9 cycles, 125 ms each) is organized into four phases, with colored letters (blue A, orange B, green C, pink D: locations; black X: none) marking burst stimulation (three spikes) in the four neurons of each location-specific cell assembly, advancing to earlier phases with successive cycles. Bottom: Raster plot over 5 s during four complete stimulations of locations (MEC cell assemblies in green) ‘A’ to ‘D’. Inhibitory neurons at top with gray shading. Background activity (black) is asynchronous irregular (‘awake’). MEC stimulation drives downstream activity via effective connections (panel a). Inset: Zoomed view of the latter part of the second stimulation (boxed), showing delayed activation in downstream regions for locations C and D. d Top: Time course of changes (∆) in mean excitatory-to-excitatory synaptic weights for connections in panel a during stimulation-driven encoding (⟨∆w⟩, solid: fast overall [labile + stable] governed by spike-timing-dependent plasticity; ⟨∆w̃⟩, dashed: slow stable governed by protein-mediated stabilization; ⟨∆w⟩ − ⟨∆w̃⟩, shading: labile component). The 5-min stimulation period (from 30 s to 330 s) represents repeated sequential exploration of locations ‘A’ to ‘D’. Middle & bottom: Matrices showing overall weights, w, between neurons before (middle) and after (bottom) the stimulation-driven encoding; white indicates no connection.\", \"page\": 4, \"index\": 4, \"width\": 941, \"height\": 794}]"
motivation: 旨在阐明记忆巩固中模糊的神经机制，特别是去抑制如何调节海马与皮层间的记忆转移。
method: 开发了一个整合内嗅皮层、海马和皮层的生物物理详细计算模型，模拟不同生理状态下的神经动力学。
result: 发现去抑制能触发空间序列重现，波纹波虽非重现必需但能加速巩固，且皮层去抑制是记忆转移的关键。
conclusion: 去抑制是跨状态驱动记忆巩固和海马独立性的核心要素，为记忆障碍的干预提供了潜在的治疗路径。
---

## 摘要
记忆巩固涉及复杂的神经机制。本研究开发了一个生物物理细节丰富的内嗅-海马-皮层网络模型，揭示了去抑制驱动突触和系统巩固。通过神经调节减弱抑制作用向慢波睡眠过渡，会产生上-下状态（up-down states）以及对以相位进动（phase precession）编码的空间序列进行自发的、时间压缩的重现。侧向抑制水平统一了生理性和病理性涟漪波（ripples）的多样性。皮层去抑制使得记忆能够从海马体转移。减弱的传入 CA1 突触消除了涟漪波但保留了重现，这为减轻涟漪波干扰提出了策略。即使没有涟漪波，重现也能维持系统巩固，尽管速度较慢；过度的减弱会导致巩固停止，但可以通过增强海马到皮层的连接性来挽救。内侧内嗅皮层（MEC）介导的 CA1 去抑制补偿了减弱的神经调节性 CA1 去抑制，模拟了依赖 MEC 输入的安静觉醒重现；在觉醒期间的这种配置下，人工诱导去抑制会触发驱动巩固的重现和涟漪波，强调了去抑制在不同状态下的普适性作用。这些见解阐明了去抑制在铭记记忆和促进海马独立性方面的核心地位，调和了实证观察，提出了可验证的预测，并为记忆障碍的治疗指明了方向。

## Abstract
Memory consolidation involves elusive neural mechanisms. Here, we develop a biophysically detailed model of the entorhinal-hippocampal-cortical network to reveal that disinhibition drives synaptic and systems consolidation. Transitioning to slow-wave sleep via neuromodulatory dampening of inhibition generates up-down states and spontaneous, time-compressed replays of spatial sequences encoded with phase precession. Lateral inhibition levels unify physiological and pathological ripple diversity. Cortical disinhibition enables memory transfer from hippocampus. Weakened afferent CA1 synapses eliminate ripples but spare replays, proposing strategies to mitigate ripple disruptions. Replays sustain systems consolidation even without ripples, albeit slower; excessive weakening halts it, rescuable by enhanced hippocampal-to-cortical connectivity. Medial entorhinal cortex (MEC)-mediated CA1 disinhibition compensates for attenuated neuromodulatory CA1 disinhibition, mimicking MEC-input-dependent quiet wakefulness replay; under this configuration during wakefulness, artificially inducing disinhibition triggers replays and ripples that drive consolidation, underscoring disinhibition's state-agnostic role. These insights elucidate disinhibition's centrality in engraining memories and fostering hippocampal independence, reconciling empirical observations, yielding testable predictions, and identifying therapeutic avenues for memory disorders.

---

## 论文详细总结（自动生成）

这是一份关于论文《Sleep-modulated disinhibition enables replay for memory consolidation, accelerated by ripples》的深度结构化总结：

### 1. 核心问题与整体含义
*   **研究动机**：记忆巩固（突触巩固与系统巩固）是学习的核心，但其背后的神经机制，特别是海马体与皮层之间如何协调记忆转移，仍不明确。
*   **核心问题**：
    *   什么机制触发了睡眠期间的自发记忆重现（Replay）？
    *   尖波涟漪（SWRs）与记忆重现之间是何种关系？涟漪波是重现所必需的吗？
    *   记忆如何从海马体转移到皮层并实现“海马独立性”？
*   **整体含义**：论文提出“去抑制（Disinhibition）”是跨越不同生理状态（睡眠与觉醒）驱动记忆巩固的核心统一机制。

### 2. 方法论：核心思想与技术细节
*   **核心思想**：构建一个生物物理细节丰富的**内嗅-海马-皮层（MEC-DG-CA3-CA1-CR）**多区域计算模型，通过模拟神经调节引起的抑制水平变化来驱动记忆过程。
*   **关键技术细节**：
    *   **神经元模型**：采用 Hodgkin-Huxley 类型的随机神经元，包含钠、钾、氯离子动力学及泵电流。
    *   **状态切换机制**：通过降低细胞外钾离子缓冲浓度（$[K^+]_{Buffer}$）模拟从觉醒到慢波睡眠（SWS）的转变，这会导致神经元超极化并减弱抑制性突触效能（去抑制）。
    *   **可塑性规则**：使用三元组尖峰时间依赖可塑性（Triplet-STDP）处理兴奋性突触，并配合动态的前馈、反馈和侧向抑制更新规则。
    *   **记忆编码**：在觉醒态通过相位进动（Phase Precession）模式刺激 MEC 组合，将空间序列编码进网络。
    *   **突触稳定化**：引入蛋白质介导的标记与捕获机制（Synaptic Tagging and Capture），模拟从易损的早期 LTP 到稳定的晚期 LTP 的转变。

### 3. 实验设计与对比
*   **场景模拟**：
    *   **编码阶段**：模拟动物在空间环境 A-D 之间的移动。
    *   **巩固阶段**：模拟慢波睡眠（SWS）和安静觉醒（QW）状态。
*   **对比配置（Benchmark）**：
    *   **有无涟漪波对比**：通过调节 CA3 到 CA1 的兴奋性权重，对比“有涟漪重现”与“无涟漪重现”的巩固速度。
    *   **抑制水平对比**：改变侧向抑制（LI）强度（100%, 50%, 0%），观察对涟漪波形态（链状、长时程、病理性）的影响。
    *   **输入依赖性对比**：在 QW 状态下，对比有无 MEC 输入对 CA1 重现的影响，验证 MEC 介导的去抑制路径。
*   **消融实验**：移除区域间延迟、禁用 STDP 或蛋白质合成，观察对序列重现和长期记忆存储的影响。

### 4. 资源与算力
*   **算力说明**：论文**未明确说明**具体的硬件配置（如 GPU/CPU 型号）或总训练时长。
*   **模型规模**：模型包含约 435 个生物物理神经元，涉及多个脑区和复杂的突触连接。由于采用的是高精度的 Hodgkin-Huxley 方程和随机微分方程数值积分（Heun 方法，步长 0.025 ms），此类模拟通常具有较高的计算成本。

### 5. 实验数量与充分性
*   **实验组数**：论文展示了约 7 组核心实验结果，涵盖了从编码、睡眠重现、涟漪波多样性、皮层转移到觉醒重现的全过程。
*   **充分性评价**：
    *   **充分性**：实验设计非常全面，不仅模拟了正常生理状态，还探讨了病理性状态（如精神分裂症样涟漪波、阿尔茨海默症样的巩固中断）。
    *   **客观性**：通过参数扫描（如改变 CA3-CA1 权重、侧向抑制强度）展示了连续的动力学变化，而非单一结果，增强了结论的可靠性。
    *   **公平性**：对比实验在相同的背景噪声和神经元参数下进行，仅改变关键的调节因子（如抑制增益）。

### 6. 主要结论与发现
*   **去抑制是核心**：睡眠期间神经调节引起的抑制减弱是产生上-下状态和自发重现的根本原因。
*   **涟漪波的作用**：涟漪波并非重现的必要条件（存在无涟漪重现），但它能显著加速突触和系统的巩固过程。
*   **侧向抑制决定多样性**：侧向抑制的强弱决定了涟漪波是离散的、延长的还是病理性的融合状态。
*   **系统巩固路径**：皮层去抑制是海马记忆向皮层转移的“门控”，转移完成后皮层可实现海马独立的重现。
*   **状态普适性**：在觉醒态，通过 MEC 介导的微回路去抑制同样可以触发重现，解释了安静觉醒时的记忆处理。

### 7. 优点与亮点
*   **生物物理精度高**：整合了离子动力学、短时程/长时程可塑性、蛋白质合成和多种抑制回路，是目前较为详尽的系统级模型。
*   **统一框架**：一个模型解释了多种现象（重现、涟漪波、相位进动、系统巩固、病理性振荡），具有很强的理论整合力。
*   **临床关联**：为阿尔茨海默症、精神分裂症等疾病中的记忆障碍提供了明确的回路级解释和潜在干预靶点（如增强侧向抑制）。

### 8. 不足与局限
*   **规模限制**：神经元数量（数百个）相对于真实大脑仍较小，可能无法完全捕捉大规模群体编码的涌现特性。
*   **反馈回路缺失**：模型简化了部分反馈连接（如皮层对海马的反馈、CA3 对 DG 的反馈），这些连接在记忆检索和选择中可能很重要。
*   **遗忘机制简化**：虽然提到了海马独立性，但对长期遗忘（如神经发生驱动的遗忘）的模拟较为抽象。
*   **验证依赖性**：作为计算模型，其提出的“去抑制驱动上-下状态”等预测仍需更多光遗传学实验的直接验证。

（完）
