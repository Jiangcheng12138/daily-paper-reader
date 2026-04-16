---
title: "Sleep-modulated disinhibition enables replay for memory consolidation, accelerated by ripples"
title_zh: 睡眠调节的去抑制使记忆巩固的重现成为可能，并由涟漪波加速
authors: "Dutta, S."
date: 2026-04-11
pdf: "https://www.biorxiv.org/content/10.64898/2025.12.09.693276v3.full.pdf"
tags: ["query:slp-ns"]
score: 9.0
evidence: 慢波睡眠与记忆巩固的神经机制
tldr: 本研究通过构建内嗅皮层-海马-皮层网络的生物物理详细模型，揭示了去抑制（disinhibition）是驱动记忆巩固的核心机制。研究发现，睡眠期间神经调节引起的抑制减弱会触发自发性记忆重现和尖波波纹（ripples），进而促进记忆从海马向皮层的转移。虽然波纹波能显著加速巩固过程，但去抑制本身才是实现海马独立性的关键，且该机制在清醒状态下的记忆重现中同样适用。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2025-12-09-693276-v3/fig-001.webp\", \"caption\": \"Fig 2: Transition to slow-wave sleep activates K+-dependent disinhibition that enables spontaneous time-compressed replay via inter-assembly delay. a Time courses of average extracellular K+, 〈 [K+]o 〉 , and average firing rate of entorhinal and hippocampal regions. Top: Temporal evolution of ⟨[K+]o⟩ from ‘Background’ neurons when [K+]Buffer is decreased from 3.5 to 3.0 mM at 100 s to initiate the transition from ‘awake’ to ‘slow-wave sleep’ dynamics. Middle & bottom: Average firing rates, ⟨ψ⟩, during normal MEC dynamics (middle) and during silenced MEC dynamics by enhanced inhibition (bottom). Arrows labeled ‘b’ to ‘g’ point to the timestamps of rasters in panels b to g. b–g Top: 1200 ms raster plot of spikes from all neurons at the respective timestamps from panel a. Bottom: Zoom of the 400 ms box from the top panel showing exemplars of replays with lengths 2–4. h Bar plot showing the logarithm of total number of CA1 replays of lengths 2–4 during time-courses in panel a. i Left: Sequential replay with inter-assembly delay. Right: Disrupted replay sequence without inter-assembly delay. Colors represent brain regions as in Fig. 1.\", \"page\": 6, \"index\": 1, \"width\": 940, \"height\": 794}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2025-12-09-693276-v3/fig-002.webp\", \"caption\": \"Fig 6: Disabling K+-dependent CA1 disinhibition underlies MEC-input-dependent quiet wakefulness replay through MEC-mediated disinhibition. a,b Row 1: Schematics of feedforward excitatory inputs (arrows) from MEC and CA3 (column 1), CA3-only (column 2), or MEC-only (column 3) to CA1 excitatory and inhibitory neurons; absent (panel a) or present (panel b) inhibitory link (round arrowheads) from MEC- to CA3-receiving CA1 interneurons (I1 → I2 = 50), enabling MEC-mediated disinhibition of excitatory CA1 neurons and gating CA3 input to CA1. Rows 2–7: Replay dynamics, with K+-dependent disinhibition enabled (rows 2–4) or disabled (rows 5–7), in 300-ms raster plots (rows 2, 5), CA1 local field potentials (rows 3, 6), and time– frequency analyses (rows 4, 7). Colors denote brain regions as in Fig. 1.\", \"page\": 10, \"index\": 2, \"width\": 939, \"height\": 798}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2025-12-09-693276-v3/fig-003.webp\", \"caption\": \"Fig 4: Different levels of lateral inhibition unify ripple diversity. a Mean power of CA1 ripple-associated replays (all lengths, including 1) increases as lateral inhibition (LI) decreases, computed over 200-s simulations. b 300-ms raster plot (row 1), CA1 local field potential (row 2), and CA1 frequency-time analysis (row 3) at 100% LI (ripple chain; left), 50% LI (long-duration ripple; middle), and 0% LI (pathological ripple; right). MEC is silenced to eliminate its inputs to CA3 and CA1, thereby isolating CA3 modulation of CA1. Colors represent brain regions as in Fig. 1.\", \"page\": 8, \"index\": 3, \"width\": 924, \"height\": 248}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2025-12-09-693276-v3/fig-004.webp\", \"caption\": \"Fig 1: Entorhinal-hippocampal-cortical circuit model, awake/sleep dynamics, and stimulation-driven encoding. a Left: Schematic of the entorhinal-hippocampal-cortical circuit driven by background neural activity. Brain regions: medial entorhinal cortex (MEC, green), dentate gyrus (DG, yellow), CA3 (purple), CA1 (red), cortical regions (CR, blue-green), unmodeled brain regions (Background, black). Black solid arrows denote effective pre-encoding connections (MEC→DG, MEC→CA3, MEC→CA1, CA3→CA1). Gray solid arrow (CA1→CR) indicates anatomical connection with strong feedforward inhibition during wakefulness. Dashed arrows show ineffective (weak) pre-encoding connections (DG→CA3; recurrent in MEC, CA3, CR). Lightning bolt on MEC signifies stimulation initiating encoding. Right top: Dynamic synaptic updates for feedforward inhibition. Neurons: presynaptic excitatory (‘pre’, unfilled circle), postsynaptic excitatory (‘post’, unfilled circle) or inhibitory (gray filled circle). Updates: ∆w± from ‘pre’ to excitatory ‘post’ drives A∆w± to ‘pre’→inhibitory ‘post’ and B∆w± to inhibitory ‘post’→excitatory ‘post’, where A = a/M , B = b/M , M is the number of interneurons in the feedforward inhibition path from ‘pre’ to ‘post’, and a, b are scaling constants. Right bottom: Dynamic synaptic updates for feedback and lateral inhibition. Neurons: excitatory in the assembly of ‘post’ (‘self’, middle unfilled circle), in other assemblies (‘other’, left/right unfilled circles), assembly-specific inhibitory neuron (ASIN, filled circle). Updates: ∆w± to ‘post’ drives c∆w± to ‘post’→ASIN, D∆w± to ASIN→‘self’ (feedback), F∆w± to ASIN→‘other’ (lateral), where D = d/N , F = f/N , N is the number of neurons in the assembly, and c, d, f are scaling constants. Arrows: excitatory; round arrowheads: inhibitory. b Extracellular potassium buffer ([K+]Buffer) decrease (3.5 to 3.0 mM) transitions the dynamics from ‘awake’ to ‘slow-wave sleep’ via disinhibition. Top: Raster plots of spikes from 435 neurons (1–336 excitatory, 337–435 inhibitory) showing ‘awake’ (asynchronous-irregular; left) and ‘slow-wave sleep’ (up-down; right) dynamics before encoding. Bottom: Respective local field potential activity, (Φ), from ‘Background’ neurons. Gray lines trace the upper and lower envelopes. c Top: Stimulation pattern mimicking exploration from locations A to D with phase precession for 16 MEC neurons over 1.125 s. Each gray 8-Hz cycle (9 cycles, 125 ms each) is organized into four phases, with colored letters (blue A, orange B, green C, pink D: locations; black X: none) marking burst stimulation (three spikes) in the four neurons of each location-specific cell assembly, advancing to earlier phases with successive cycles. Bottom: Raster plot over 5 s during four complete stimulations of locations (MEC cell assemblies in green) ‘A’ to ‘D’. Inhibitory neurons at top with gray shading. Background activity (black) is asynchronous irregular (‘awake’). MEC stimulation drives downstream activity via effective connections (panel a). Inset: Zoomed view of the latter part of the second stimulation (boxed), showing delayed activation in downstream regions for locations C and D. d Top: Time course of changes (∆) in mean excitatory-to-excitatory synaptic weights for connections in panel a during stimulation-driven encoding (⟨∆w⟩, solid: fast overall [labile + stable] governed by spike-timing-dependent plasticity; ⟨∆w̃⟩, dashed: slow stable governed by protein-mediated stabilization; ⟨∆w⟩ − ⟨∆w̃⟩, shading: labile component). The 5-min stimulation period (from 30 s to 330 s) represents repeated sequential exploration of locations ‘A’ to ‘D’. Middle & bottom: Matrices showing overall weights, w, between neurons before (middle) and after (bottom) the stimulation-driven encoding; white indicates no connection.\", \"page\": 4, \"index\": 4, \"width\": 941, \"height\": 794}]"
motivation: 旨在阐明记忆巩固过程中，神经回路如何通过特定的抑制调节机制实现海马体到皮层的记忆转移。
method: 开发了一个整合内嗅皮层、海马体和皮层的生物物理详细计算模型，模拟慢波睡眠中的神经调节变化。
result: 发现去抑制不仅能产生记忆重现和波纹波，还能通过皮层去抑制实现记忆转移，且波纹波对巩固起加速作用而非绝对必要。
conclusion: 去抑制是记忆巩固和海马独立性的中心机制，为理解记忆形成及治疗记忆障碍提供了新的理论框架和潜在途径。
---

## 摘要
记忆巩固涉及复杂的神经机制。在本研究中，我们开发了一个生物物理细节丰富的内嗅皮层-海马-皮层网络模型，揭示了去抑制驱动突触和系统巩固。通过神经调节减弱抑制作用向慢波睡眠过渡，会产生上下状态（up-down states）以及对以相位前移（phase precession）编码的空间序列进行自发的、时间压缩的重现（replays）。侧向抑制水平统一了生理性和病理性涟漪波（ripples）的多样性。皮层去抑制使记忆能够从海马体转移。减弱 CA1 传入突触会消除涟漪波但保留重现，这为减轻涟漪波干扰提出了策略。即使没有涟漪波，重现也能维持系统巩固，尽管速度较慢；过度减弱会导致巩固停止，但可以通过增强海马到皮层的连接性来挽救。内侧内嗅皮层（MEC）介导的 CA1 去抑制补偿了减弱的神经调节性 CA1 去抑制，模拟了依赖 MEC 输入的安静觉醒重现；在觉醒期间的这种配置下，人工诱导去抑制会触发驱动巩固的重现和涟漪波，强调了去抑制在不同状态下的普适作用。这些见解阐明了去抑制在铭刻记忆和促进海马独立性方面的核心地位，调和了实证观察，提出了可测试的预测，并为记忆障碍找到了治疗途径。

## Abstract
Memory consolidation involves elusive neural mechanisms. Here, we develop a biophysically detailed model of the entorhinal-hippocampal-cortical network to reveal that disinhibition drives synaptic and systems consolidation. Transitioning to slow-wave sleep via neuromodulatory dampening of inhibition generates up-down states and spontaneous, time-compressed replays of spatial sequences encoded with phase precession. Lateral inhibition levels unify physiological and pathological ripple diversity. Cortical disinhibition enables memory transfer from hippocampus. Weakened afferent CA1 synapses eliminate ripples but spare replays, proposing strategies to mitigate ripple disruptions. Replays sustain systems consolidation even without ripples, albeit slower; excessive weakening halts it, rescuable by enhanced hippocampal-to-cortical connectivity. Medial entorhinal cortex (MEC)-mediated CA1 disinhibition compensates for attenuated neuromodulatory CA1 disinhibition, mimicking MEC-input-dependent quiet wakefulness replay; under this configuration during wakefulness, artificially inducing disinhibition triggers replays and ripples that drive consolidation, underscoring disinhibitions state-agnostic role. These insights elucidate disinhibitions centrality in engraining memories and fostering hippocampal independence, reconciling empirical observations, yielding testable predictions, and identifying therapeutic avenues for memory disorders.

---

## 论文详细总结（自动生成）

### 论文总结：睡眠调节的去抑制使记忆巩固的重现成为可能，并由涟漪波加速

#### 1. 核心问题与整体含义（研究动机和背景）
记忆巩固是将瞬时经验转化为长期记忆的过程，涉及**突触巩固**（海马局部稳定）和**系统巩固**（海马向皮层转移）。尽管已知慢波睡眠（SWS）期间的**记忆重现（Replay）**和**尖波涟漪（SWRs/Ripples）**对此至关重要，但其核心触发机制仍不明确。
*   **研究动机**：传统观点认为涟漪波启动了重现，但近期发现存在“无涟漪的重现”。此外，睡眠状态下抑制性回路的改变如何精确控制记忆转移仍缺乏统一的生物物理框架。
*   **核心问题**：什么机制驱动了重现的产生？涟漪波在巩固中是必要条件还是加速手段？去抑制（Disinhibition）在不同脑态（睡眠与觉醒）中扮演什么角色？

#### 2. 论文提出的方法论
作者开发了一个高度详细的**内嗅皮层-海马-皮层（MEC-DG-CA3-CA1-CR）网络生物物理模型**。
*   **核心思想**：通过神经调节引起的**去抑制**（即抑制性神经元活性的减弱）作为记忆重现和巩固的核心驱动力。
*   **关键技术细节**：
    *   **神经元模型**：采用 Hodgkin-Huxley 方程，模拟钠、钾、氯离子动力学。
    *   **脑态转换**：通过调节细胞外钾离子缓冲浓度（$[K^+]_{Buffer}$）模拟从觉醒到睡眠的过渡，进而诱发“上下状态”（Up-Down states）。
    *   **突触可塑性**：整合了**三元组尖峰定时依赖可塑性（Triplet-STDP）**和**蛋白质介导的突触稳定化机制**（模拟 Late-LTP），并包含棘突（Spine）的动态添加与移除。
    *   **抑制调节**：引入 $K^+$ 依赖的去抑制因子，调节前馈、反馈和侧向抑制的强度。

#### 3. 实验设计
研究通过模拟空间导航序列的编码与离线巩固来验证模型。
*   **场景设置**：模拟动物在四个位置（A-D）移动，MEC 神经元以**相位前移（Phase Precession）**模式放电进行编码。
*   **对比实验与消融研究**：
    *   **涟漪波贡献**：对比正常 CA3-CA1 连接（有涟漪）与减弱连接（无涟漪）下的重现与巩固速度。
    *   **侧向抑制（LI）影响**：改变 LI 强度（100%, 50%, 0%）以观察涟漪波从“链状”到“长时程”再到“病理性融合”的演变。
    *   **脑态对比**：模拟慢波睡眠（SWS）与安静觉醒（QW）下的重现机制，特别是 MEC 输入对 QW 重现的必要性。
    *   **系统巩固**：测试记忆从海马 CA1 向皮层区域（CR）转移的成功率及海马独立性。

#### 4. 资源与算力
*   **算力说明**：论文**未明确说明**具体的硬件型号（如 GPU/CPU 数量）或总训练时长。
*   **数值计算**：提到使用了随机 Heun 方法处理随机微分方程，确定性部分使用 Heun 和 Euler 方法，积分步长设为 0.025 ms。考虑到生物物理模型的复杂性，此类模拟通常对 CPU 单核性能和内存带宽有一定要求。

#### 5. 实验数量与充分性
*   **实验规模**：作者进行了多组参数扫描实验，包括不同脑区的抑制水平、突触权重缩放、侧向抑制强度等。
*   **充分性评价**：实验设计较为**充分且系统**。研究不仅复现了正常的生理现象（如时间压缩的重现），还成功模拟了病理状态（如精神分裂症样涟漪波）和极端消融情况（无涟漪重现），逻辑链条完整，客观性较强。

#### 6. 主要结论与发现
*   **去抑制是核心**：睡眠诱导的去抑制是启动自发重现和系统巩固的必要且充分条件。
*   **涟漪波的作用**：涟漪波并非重现的启动者，而是**加速器**。即使没有涟漪波，只要存在去抑制，重现仍能发生并完成巩固，但速度显著变慢。
*   **侧向抑制决定多样性**：侧向抑制的强度决定了涟漪波的形态（离散链状 vs. 融合长时程），过低的侧向抑制会导致序列信息丢失（病理性）。
*   **状态普适性**：安静觉醒下的重现依赖于 MEC 介导的去抑制来补偿神经调节的不足。人工诱导去抑制可以在觉醒状态下触发本属于睡眠的巩固过程。

#### 7. 优点
*   **机制统一性**：一个模型解释了从分子（离子通道、蛋白质合成）到回路（去抑制、侧向抑制）再到系统（海马-皮层转移）的跨尺度现象。
*   **前瞻性解释**：为“无涟漪重现”提供了坚实的生物物理基础，并调和了关于涟漪波是否必须的争议。
*   **临床价值**：提出了通过调节侧向抑制或增强皮层连接来修复记忆障碍（如阿尔茨海默病、精神分裂症）的潜在策略。

#### 8. 不足与局限
*   **模型规模**：神经元数量相对较少（数百个），可能无法完全捕捉大规模神经网络中的涌现特性。
*   **解剖简化**：忽略了某些反馈通路（如皮层向海马的反馈）和 REM 睡眠阶段的动态。
*   **参数依赖**：生物物理模型高度依赖参数设置，虽然文中引用了大量实验数据，但在不同物种间的泛化性仍需验证。
*   **算力细节缺失**：缺乏计算成本的描述，不利于其他研究者评估复现该模型所需的资源。

（完）
