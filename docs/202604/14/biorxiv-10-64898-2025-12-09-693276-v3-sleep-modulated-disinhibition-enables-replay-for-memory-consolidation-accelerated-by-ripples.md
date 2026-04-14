---
title: "Sleep-modulated disinhibition enables replay for memory consolidation, accelerated by ripples"
title_zh: 睡眠调节的去抑制使记忆巩固的重现成为可能，并由涟漪波加速
authors: "Dutta, S."
date: 2026-04-11
pdf: "https://www.biorxiv.org/content/10.64898/2025.12.09.693276v3.full.pdf"
tags: ["query:slp-ns"]
score: 9.0
evidence: 慢波睡眠期间记忆巩固的神经机制
tldr: 本研究利用海马-皮层网络生物物理模型，揭示了去抑制是驱动神经重现与记忆巩固的关键机制。研究发现睡眠状态下的抑制减弱触发了记忆从海马向皮层的转移，尖波涟漪虽能加速巩固但非绝对必要。该模型统一了生理与病理涟漪的多样性，并证明去抑制在不同生理状态下均能促进记忆强化，为记忆障碍治疗提供了新思路。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2025-12-09-693276-v3/fig-001.webp\", \"caption\": \"Fig 2: Transition to slow-wave sleep activates K+-dependent disinhibition that enables spontaneous time-compressed replay via inter-assembly delay. a Time courses of average extracellular K+, 〈 [K+]o 〉 , and average firing rate of entorhinal and hippocampal regions. Top: Temporal evolution of ⟨[K+]o⟩ from ‘Background’ neurons when [K+]Buffer is decreased from 3.5 to 3.0 mM at 100 s to initiate the transition from ‘awake’ to ‘slow-wave sleep’ dynamics. Middle & bottom: Average firing rates, ⟨ψ⟩, during normal MEC dynamics (middle) and during silenced MEC dynamics by enhanced inhibition (bottom). Arrows labeled ‘b’ to ‘g’ point to the timestamps of rasters in panels b to g. b–g Top: 1200 ms raster plot of spikes from all neurons at the respective timestamps from panel a. Bottom: Zoom of the 400 ms box from the top panel showing exemplars of replays with lengths 2–4. h Bar plot showing the logarithm of total number of CA1 replays of lengths 2–4 during time-courses in panel a. i Left: Sequential replay with inter-assembly delay. Right: Disrupted replay sequence without inter-assembly delay. Colors represent brain regions as in Fig. 1.\", \"page\": 6, \"index\": 1, \"width\": 940, \"height\": 794}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2025-12-09-693276-v3/fig-002.webp\", \"caption\": \"Fig 6: Disabling K+-dependent CA1 disinhibition underlies MEC-input-dependent quiet wakefulness replay through MEC-mediated disinhibition. a,b Row 1: Schematics of feedforward excitatory inputs (arrows) from MEC and CA3 (column 1), CA3-only (column 2), or MEC-only (column 3) to CA1 excitatory and inhibitory neurons; absent (panel a) or present (panel b) inhibitory link (round arrowheads) from MEC- to CA3-receiving CA1 interneurons (I1 → I2 = 50), enabling MEC-mediated disinhibition of excitatory CA1 neurons and gating CA3 input to CA1. Rows 2–7: Replay dynamics, with K+-dependent disinhibition enabled (rows 2–4) or disabled (rows 5–7), in 300-ms raster plots (rows 2, 5), CA1 local field potentials (rows 3, 6), and time– frequency analyses (rows 4, 7). Colors denote brain regions as in Fig. 1.\", \"page\": 10, \"index\": 2, \"width\": 939, \"height\": 798}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2025-12-09-693276-v3/fig-003.webp\", \"caption\": \"Fig 4: Different levels of lateral inhibition unify ripple diversity. a Mean power of CA1 ripple-associated replays (all lengths, including 1) increases as lateral inhibition (LI) decreases, computed over 200-s simulations. b 300-ms raster plot (row 1), CA1 local field potential (row 2), and CA1 frequency-time analysis (row 3) at 100% LI (ripple chain; left), 50% LI (long-duration ripple; middle), and 0% LI (pathological ripple; right). MEC is silenced to eliminate its inputs to CA3 and CA1, thereby isolating CA3 modulation of CA1. Colors represent brain regions as in Fig. 1.\", \"page\": 8, \"index\": 3, \"width\": 924, \"height\": 248}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2025-12-09-693276-v3/fig-004.webp\", \"caption\": \"Fig 1: Entorhinal-hippocampal-cortical circuit model, awake/sleep dynamics, and stimulation-driven encoding. a Left: Schematic of the entorhinal-hippocampal-cortical circuit driven by background neural activity. Brain regions: medial entorhinal cortex (MEC, green), dentate gyrus (DG, yellow), CA3 (purple), CA1 (red), cortical regions (CR, blue-green), unmodeled brain regions (Background, black). Black solid arrows denote effective pre-encoding connections (MEC→DG, MEC→CA3, MEC→CA1, CA3→CA1). Gray solid arrow (CA1→CR) indicates anatomical connection with strong feedforward inhibition during wakefulness. Dashed arrows show ineffective (weak) pre-encoding connections (DG→CA3; recurrent in MEC, CA3, CR). Lightning bolt on MEC signifies stimulation initiating encoding. Right top: Dynamic synaptic updates for feedforward inhibition. Neurons: presynaptic excitatory (‘pre’, unfilled circle), postsynaptic excitatory (‘post’, unfilled circle) or inhibitory (gray filled circle). Updates: ∆w± from ‘pre’ to excitatory ‘post’ drives A∆w± to ‘pre’→inhibitory ‘post’ and B∆w± to inhibitory ‘post’→excitatory ‘post’, where A = a/M , B = b/M , M is the number of interneurons in the feedforward inhibition path from ‘pre’ to ‘post’, and a, b are scaling constants. Right bottom: Dynamic synaptic updates for feedback and lateral inhibition. Neurons: excitatory in the assembly of ‘post’ (‘self’, middle unfilled circle), in other assemblies (‘other’, left/right unfilled circles), assembly-specific inhibitory neuron (ASIN, filled circle). Updates: ∆w± to ‘post’ drives c∆w± to ‘post’→ASIN, D∆w± to ASIN→‘self’ (feedback), F∆w± to ASIN→‘other’ (lateral), where D = d/N , F = f/N , N is the number of neurons in the assembly, and c, d, f are scaling constants. Arrows: excitatory; round arrowheads: inhibitory. b Extracellular potassium buffer ([K+]Buffer) decrease (3.5 to 3.0 mM) transitions the dynamics from ‘awake’ to ‘slow-wave sleep’ via disinhibition. Top: Raster plots of spikes from 435 neurons (1–336 excitatory, 337–435 inhibitory) showing ‘awake’ (asynchronous-irregular; left) and ‘slow-wave sleep’ (up-down; right) dynamics before encoding. Bottom: Respective local field potential activity, (Φ), from ‘Background’ neurons. Gray lines trace the upper and lower envelopes. c Top: Stimulation pattern mimicking exploration from locations A to D with phase precession for 16 MEC neurons over 1.125 s. Each gray 8-Hz cycle (9 cycles, 125 ms each) is organized into four phases, with colored letters (blue A, orange B, green C, pink D: locations; black X: none) marking burst stimulation (three spikes) in the four neurons of each location-specific cell assembly, advancing to earlier phases with successive cycles. Bottom: Raster plot over 5 s during four complete stimulations of locations (MEC cell assemblies in green) ‘A’ to ‘D’. Inhibitory neurons at top with gray shading. Background activity (black) is asynchronous irregular (‘awake’). MEC stimulation drives downstream activity via effective connections (panel a). Inset: Zoomed view of the latter part of the second stimulation (boxed), showing delayed activation in downstream regions for locations C and D. d Top: Time course of changes (∆) in mean excitatory-to-excitatory synaptic weights for connections in panel a during stimulation-driven encoding (⟨∆w⟩, solid: fast overall [labile + stable] governed by spike-timing-dependent plasticity; ⟨∆w̃⟩, dashed: slow stable governed by protein-mediated stabilization; ⟨∆w⟩ − ⟨∆w̃⟩, shading: labile component). The 5-min stimulation period (from 30 s to 330 s) represents repeated sequential exploration of locations ‘A’ to ‘D’. Middle & bottom: Matrices showing overall weights, w, between neurons before (middle) and after (bottom) the stimulation-driven encoding; white indicates no connection.\", \"page\": 4, \"index\": 4, \"width\": 941, \"height\": 794}]"
motivation: 探究海马-皮层网络中记忆巩固与神经重现发生的深层生物物理机制。
method: 开发了一个包含内嗅皮层、海马CA1区及皮层的精细生物物理网络模型。
result: 发现去抑制驱动了时空序列的自发重现，且尖波涟漪能显著加速记忆向皮层的转移。
conclusion: 去抑制是实现记忆巩固和海马独立性的核心要素，为干预记忆相关疾病提供了潜在靶点。
---

## 摘要
记忆巩固涉及复杂的神经机制。在这里，我们开发了一个生物物理细节丰富的内嗅皮层-海马-皮层网络模型，揭示了去抑制驱动突触和系统巩固。通过神经调节减弱抑制作用向慢波睡眠过渡，会产生上-下状态以及以相位前移编码的空间序列的自发、时间压缩式重现。侧向抑制水平统一了生理性和病理性涟漪波的多样性。皮层去抑制使记忆从海马体转移成为可能。减弱的传入 CA1 突触消除了涟漪波但保留了重现，这为减轻涟漪波干扰提出了策略。即使没有涟漪波，重现也能维持系统巩固，尽管速度较慢；过度的减弱会使其停止，但可以通过增强海马到皮层的连接性来挽救。内侧内嗅皮层 (MEC) 介导的 CA1 去抑制补偿了减弱的神经调节性 CA1 去抑制，模拟了依赖 MEC 输入的安静觉醒状态下的重现；在觉醒期间的这种配置下，人工诱导去抑制会触发驱动巩固的重现和涟漪波，强调了去抑制在不同状态下的普适性作用。这些见解阐明了去抑制在铭刻记忆和促进海马独立性方面的核心地位，调和了实验观察结果，提出了可验证的预测，并为记忆障碍指明了治疗途径。

## Abstract
Memory consolidation involves elusive neural mechanisms. Here, we develop a biophysically detailed model of the entorhinal-hippocampal-cortical network to reveal that disinhibition drives synaptic and systems consolidation. Transitioning to slow-wave sleep via neuromodulatory dampening of inhibition generates up-down states and spontaneous, time-compressed replays of spatial sequences encoded with phase precession. Lateral inhibition levels unify physiological and pathological ripple diversity. Cortical disinhibition enables memory transfer from hippocampus. Weakened afferent CA1 synapses eliminate ripples but spare replays, proposing strategies to mitigate ripple disruptions. Replays sustain systems consolidation even without ripples, albeit slower; excessive weakening halts it, rescuable by enhanced hippocampal-to-cortical connectivity. Medial entorhinal cortex (MEC)-mediated CA1 disinhibition compensates for attenuated neuromodulatory CA1 disinhibition, mimicking MEC-input-dependent quiet wakefulness replay; under this configuration during wakefulness, artificially inducing disinhibition triggers replays and ripples that drive consolidation, underscoring disinhibition's state-agnostic role. These insights elucidate disinhibition's centrality in engraining memories and fostering hippocampal independence, reconciling empirical observations, yielding testable predictions, and identifying therapeutic avenues for memory disorders.

---

## 论文详细总结（自动生成）

这篇论文通过构建精细的生物物理模型，深入探讨了睡眠和觉醒状态下记忆巩固的神经机制。以下是对该论文的结构化总结：

### 1. 核心问题与整体含义（研究动机和背景）
*   **核心问题**：记忆巩固（包括局部突触巩固和跨区域系统巩固）是如何启动和调节的？特别是神经重现（Replay）与尖波涟漪（SWRs）之间的因果关系，以及“去抑制”在这些过程中的具体作用。
*   **研究背景**：传统观点认为涟漪波启动了重现，但近期实验发现了“无涟漪的重现”。此外，睡眠期间抑制性电路的变化如何影响海马与皮层间的通信仍不明确。论文旨在建立一个统一的生物物理框架，解释这些现象并调和现有的实验矛盾。

### 2. 论文提出的方法论
*   **核心思想**：开发了一个包含内嗅皮层（MEC）、海马（DG, CA3, CA1）和皮层（CR）的多区域网络模型，通过**神经调节驱动的去抑制**（Disinhibition）来模拟从觉醒到慢波睡眠（SWS）的转换。
*   **关键技术细节**：
    *   **神经元模型**：基于 Hodgkin-Huxley 方程，包含 Na+、K+、Cl- 离子动力学及钠钾泵电流。
    *   **离子调节机制**：通过降低细胞外钾离子缓冲浓度（[K+]Buffer）模拟睡眠，导致神经元兴奋性下降和突触抑制减弱（去抑制）。
    *   **突触可塑性**：结合了**三元组 STDP**（triplet-STDP）规则、**蛋白质介导的突触稳定**（捕获标记假说）以及**棘突（Spine）的动态添加与移除**。
    *   **抑制性电路**：实现了动态的前馈抑制、反馈抑制和侧向抑制（LI），并随兴奋性突触的变化而同步更新。

### 3. 实验设计
*   **场景模拟**：
    *   **编码阶段**：模拟空间导航，通过 MEC 的相位前移（Phase Precession）脉冲刺激诱导序列编码。
    *   **巩固阶段**：模拟 SWS 期间的自发重现。
*   **对比实验与 Benchmark**：
    *   **涟漪波消融**：通过减弱 CA3→CA1 的兴奋性权重，观察在无涟漪情况下重现是否依然能驱动巩固。
    *   **侧向抑制调节**：对比 100%、50% 和 0% 的侧向抑制水平，模拟从正常涟漪链到病理性（如精神分裂症）涟漪的演变。
    *   **MEC 作用分析**：对比 MEC 正常与沉默状态下的重现特征。
    *   **状态对比**：模拟安静觉醒（QW）与 SWS 下重现对 MEC 输入的依赖性差异。

### 4. 资源与算力
*   **算力说明**：论文未明确提及具体的 GPU/CPU 型号或总训练时长。
*   **计算规模**：模型包含约 435 个详细的 Hodgkin-Huxley 神经元。数值积分采用随机 Heun 法（步长 0.025 ms），考虑到生物物理细节的复杂性，此类仿真通常具有较高的计算成本。

### 5. 实验数量与充分性
*   **实验组数**：论文涵盖了编码验证、睡眠转换、涟漪波多样性分析、系统巩固转移、安静觉醒机制模拟等约 7 大类核心实验。
*   **充分性评价**：实验设计非常充分且具有高度的逻辑性。作者不仅重现了正常的生理现象，还通过参数消融（如移除间隙延迟、改变抑制强度）成功模拟了多种病理状态（如阿尔茨海默症、精神分裂症相关的记忆障碍），实验结果与大量已发表的电生理数据高度吻合，具有很强的客观性。

### 6. 主要结论与发现
*   **去抑制是核心**：睡眠调节的去抑制是启动神经重现和记忆巩固的根本驱动力，而非涟漪波本身。
*   **涟漪波的加速作用**：涟漪波虽然不是重现的必要条件，但它能显著加速突触和系统层面的记忆巩固。
*   **侧向抑制决定多样性**：侧向抑制水平的差异解释了生理性涟漪链、长时程涟漪以及病理性无序涟漪的形成。
*   **状态逻辑统一**：MEC 介导的去抑制补偿了觉醒状态下较低的神经调节水平，解释了安静觉醒重现对 MEC 输入的特异性依赖。
*   **海马独立性**：成功的系统巩固使皮层能够独立于海马产生重现。

### 7. 优点
*   **生物物理精度高**：整合了从离子通道到结构可塑性的多尺度机制，远超一般的简化神经网络模型。
*   **解释力强**：一个模型同时解释了重现、涟漪波、相位前移、上-下状态以及多种脑疾病的记忆表征。
*   **预测性**：提出了关于“无涟漪重现”如何通过增强海马-皮层连接来挽救巩固缺陷的临床假设。

### 8. 不足与局限
*   **规模限制**：受限于生物物理细节的复杂性，网络规模（数百个神经元）较小，可能无法完全模拟大规模脑区的群体动力学。
*   **反馈缺失**：模型主要关注前馈路径，缺乏皮层对海马的反馈调节以及 CA3 对 DG 的反馈。
*   **简化假设**：未深入探讨 REM 睡眠在记忆巩固中的协同作用，且对环境显著性（Saliency）的建模较为抽象。

（完）
