---
title: "Sleep-modulated disinhibition enables replay for memory consolidation, accelerated by ripples"
title_zh: 睡眠调节的去抑制促进记忆巩固中的重现，并由波纹波加速
authors: "Dutta, S."
date: 2026-04-11
pdf: "https://www.biorxiv.org/content/10.64898/2025.12.09.693276v3.full.pdf"
tags: ["query:slp-ns"]
score: 9.0
evidence: 慢波睡眠与记忆巩固的神经机制
tldr: 本研究通过构建内嗅皮层-海马-皮层网络的生物物理详细模型，揭示了“去抑制”是驱动记忆巩固的核心机制。研究发现，睡眠期间神经调制引起的抑制减弱会触发神经元重现（replay）和锐波纹（ripples），进而促进记忆从海马向皮层的转移。模型不仅统一了生理和病理状态下的波纹多样性，还证明了即使在没有波纹的情况下，重现仍能维持较慢的巩固进程，强调了去抑制在增强记忆和实现海马独立性中的关键作用。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2025-12-09-693276-v3/fig-001.webp\", \"caption\": \"Fig 2: Transition to slow-wave sleep activates K+-dependent disinhibition that enables spontaneous time-compressed replay via inter-assembly delay. a Time courses of average extracellular K+, 〈 [K+]o 〉 , and average firing rate of entorhinal and hippocampal regions. Top: Temporal evolution of ⟨[K+]o⟩ from ‘Background’ neurons when [K+]Buffer is decreased from 3.5 to 3.0 mM at 100 s to initiate the transition from ‘awake’ to ‘slow-wave sleep’ dynamics. Middle & bottom: Average firing rates, ⟨ψ⟩, during normal MEC dynamics (middle) and during silenced MEC dynamics by enhanced inhibition (bottom). Arrows labeled ‘b’ to ‘g’ point to the timestamps of rasters in panels b to g. b–g Top: 1200 ms raster plot of spikes from all neurons at the respective timestamps from panel a. Bottom: Zoom of the 400 ms box from the top panel showing exemplars of replays with lengths 2–4. h Bar plot showing the logarithm of total number of CA1 replays of lengths 2–4 during time-courses in panel a. i Left: Sequential replay with inter-assembly delay. Right: Disrupted replay sequence without inter-assembly delay. Colors represent brain regions as in Fig. 1.\", \"page\": 6, \"index\": 1, \"width\": 940, \"height\": 794}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2025-12-09-693276-v3/fig-002.webp\", \"caption\": \"Fig 6: Disabling K+-dependent CA1 disinhibition underlies MEC-input-dependent quiet wakefulness replay through MEC-mediated disinhibition. a,b Row 1: Schematics of feedforward excitatory inputs (arrows) from MEC and CA3 (column 1), CA3-only (column 2), or MEC-only (column 3) to CA1 excitatory and inhibitory neurons; absent (panel a) or present (panel b) inhibitory link (round arrowheads) from MEC- to CA3-receiving CA1 interneurons (I1 → I2 = 50), enabling MEC-mediated disinhibition of excitatory CA1 neurons and gating CA3 input to CA1. Rows 2–7: Replay dynamics, with K+-dependent disinhibition enabled (rows 2–4) or disabled (rows 5–7), in 300-ms raster plots (rows 2, 5), CA1 local field potentials (rows 3, 6), and time– frequency analyses (rows 4, 7). Colors denote brain regions as in Fig. 1.\", \"page\": 10, \"index\": 2, \"width\": 939, \"height\": 798}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2025-12-09-693276-v3/fig-003.webp\", \"caption\": \"Fig 4: Different levels of lateral inhibition unify ripple diversity. a Mean power of CA1 ripple-associated replays (all lengths, including 1) increases as lateral inhibition (LI) decreases, computed over 200-s simulations. b 300-ms raster plot (row 1), CA1 local field potential (row 2), and CA1 frequency-time analysis (row 3) at 100% LI (ripple chain; left), 50% LI (long-duration ripple; middle), and 0% LI (pathological ripple; right). MEC is silenced to eliminate its inputs to CA3 and CA1, thereby isolating CA3 modulation of CA1. Colors represent brain regions as in Fig. 1.\", \"page\": 8, \"index\": 3, \"width\": 924, \"height\": 248}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2025-12-09-693276-v3/fig-004.webp\", \"caption\": \"Fig 1: Entorhinal-hippocampal-cortical circuit model, awake/sleep dynamics, and stimulation-driven encoding. a Left: Schematic of the entorhinal-hippocampal-cortical circuit driven by background neural activity. Brain regions: medial entorhinal cortex (MEC, green), dentate gyrus (DG, yellow), CA3 (purple), CA1 (red), cortical regions (CR, blue-green), unmodeled brain regions (Background, black). Black solid arrows denote effective pre-encoding connections (MEC→DG, MEC→CA3, MEC→CA1, CA3→CA1). Gray solid arrow (CA1→CR) indicates anatomical connection with strong feedforward inhibition during wakefulness. Dashed arrows show ineffective (weak) pre-encoding connections (DG→CA3; recurrent in MEC, CA3, CR). Lightning bolt on MEC signifies stimulation initiating encoding. Right top: Dynamic synaptic updates for feedforward inhibition. Neurons: presynaptic excitatory (‘pre’, unfilled circle), postsynaptic excitatory (‘post’, unfilled circle) or inhibitory (gray filled circle). Updates: ∆w± from ‘pre’ to excitatory ‘post’ drives A∆w± to ‘pre’→inhibitory ‘post’ and B∆w± to inhibitory ‘post’→excitatory ‘post’, where A = a/M , B = b/M , M is the number of interneurons in the feedforward inhibition path from ‘pre’ to ‘post’, and a, b are scaling constants. Right bottom: Dynamic synaptic updates for feedback and lateral inhibition. Neurons: excitatory in the assembly of ‘post’ (‘self’, middle unfilled circle), in other assemblies (‘other’, left/right unfilled circles), assembly-specific inhibitory neuron (ASIN, filled circle). Updates: ∆w± to ‘post’ drives c∆w± to ‘post’→ASIN, D∆w± to ASIN→‘self’ (feedback), F∆w± to ASIN→‘other’ (lateral), where D = d/N , F = f/N , N is the number of neurons in the assembly, and c, d, f are scaling constants. Arrows: excitatory; round arrowheads: inhibitory. b Extracellular potassium buffer ([K+]Buffer) decrease (3.5 to 3.0 mM) transitions the dynamics from ‘awake’ to ‘slow-wave sleep’ via disinhibition. Top: Raster plots of spikes from 435 neurons (1–336 excitatory, 337–435 inhibitory) showing ‘awake’ (asynchronous-irregular; left) and ‘slow-wave sleep’ (up-down; right) dynamics before encoding. Bottom: Respective local field potential activity, (Φ), from ‘Background’ neurons. Gray lines trace the upper and lower envelopes. c Top: Stimulation pattern mimicking exploration from locations A to D with phase precession for 16 MEC neurons over 1.125 s. Each gray 8-Hz cycle (9 cycles, 125 ms each) is organized into four phases, with colored letters (blue A, orange B, green C, pink D: locations; black X: none) marking burst stimulation (three spikes) in the four neurons of each location-specific cell assembly, advancing to earlier phases with successive cycles. Bottom: Raster plot over 5 s during four complete stimulations of locations (MEC cell assemblies in green) ‘A’ to ‘D’. Inhibitory neurons at top with gray shading. Background activity (black) is asynchronous irregular (‘awake’). MEC stimulation drives downstream activity via effective connections (panel a). Inset: Zoomed view of the latter part of the second stimulation (boxed), showing delayed activation in downstream regions for locations C and D. d Top: Time course of changes (∆) in mean excitatory-to-excitatory synaptic weights for connections in panel a during stimulation-driven encoding (⟨∆w⟩, solid: fast overall [labile + stable] governed by spike-timing-dependent plasticity; ⟨∆w̃⟩, dashed: slow stable governed by protein-mediated stabilization; ⟨∆w⟩ − ⟨∆w̃⟩, shading: labile component). The 5-min stimulation period (from 30 s to 330 s) represents repeated sequential exploration of locations ‘A’ to ‘D’. Middle & bottom: Matrices showing overall weights, w, between neurons before (middle) and after (bottom) the stimulation-driven encoding; white indicates no connection.\", \"page\": 4, \"index\": 4, \"width\": 941, \"height\": 794}]"
motivation: 旨在阐明记忆巩固过程中，神经去抑制如何驱动突触和系统层面的记忆转移与整合。
method: 开发了一个包含内嗅皮层、海马和皮层的生物物理详细网络模型，模拟慢波睡眠中的神经调制变化。
result: 发现去抑制能触发时间压缩的序列重现，且皮层去抑制是记忆从海马成功转移至皮层的关键。
conclusion: 去抑制是实现记忆巩固和海马独立性的核心机制，为理解记忆障碍及开发治疗手段提供了新视角。
---

## 摘要
记忆巩固涉及复杂的神经机制。本研究开发了一个生物物理细节丰富的内嗅皮层-海马-皮层网络模型，揭示了去抑制驱动突触和系统巩固。通过神经调节减弱抑制作用向慢波睡眠过渡，会产生上下状态以及对相位前移编码的空间序列进行自发且时间压缩的重现。侧向抑制水平统一了生理性和病理性波纹波（ripples）的多样性。皮层去抑制实现了记忆从海马的转移。减弱的传入 CA1 突触消除了波纹波但保留了重现，这为减轻波纹波干扰提出了策略。即使没有波纹波，重现也能维持系统巩固，尽管速度较慢；过度的减弱会导致巩固停止，但可以通过增强海马到皮层的连接性来挽救。内侧内嗅皮层（MEC）介导的 CA1 去抑制补偿了减弱的神经调节 CA1 去抑制，模拟了依赖于 MEC 输入的安静觉醒重现；在觉醒期间的这种配置下，人工诱导去抑制会触发驱动巩固的重现和波纹波，强调了去抑制在不同状态下的普适作用。这些见解阐明了去抑制在铭刻记忆和促进海马独立性方面的核心地位，调和了实验观察结果，提出了可测试的预测，并为记忆障碍确定了治疗途径。

## Abstract
Memory consolidation involves elusive neural mechanisms. Here, we develop a biophysically detailed model of the entorhinal-hippocampal-cortical network to reveal that disinhibition drives synaptic and systems consolidation. Transitioning to slow-wave sleep via neuromodulatory dampening of inhibition generates up-down states and spontaneous, time-compressed replays of spatial sequences encoded with phase precession. Lateral inhibition levels unify physiological and pathological ripple diversity. Cortical disinhibition enables memory transfer from hippocampus. Weakened afferent CA1 synapses eliminate ripples but spare replays, proposing strategies to mitigate ripple disruptions. Replays sustain systems consolidation even without ripples, albeit slower; excessive weakening halts it, rescuable by enhanced hippocampal-to-cortical connectivity. Medial entorhinal cortex (MEC)-mediated CA1 disinhibition compensates for attenuated neuromodulatory CA1 disinhibition, mimicking MEC-input-dependent quiet wakefulness replay; under this configuration during wakefulness, artificially inducing disinhibition triggers replays and ripples that drive consolidation, underscoring disinhibitions state-agnostic role. These insights elucidate disinhibitions centrality in engraining memories and fostering hippocampal independence, reconciling empirical observations, yielding testable predictions, and identifying therapeutic avenues for memory disorders.

---

## 论文详细总结（自动生成）

这是一份关于论文《Sleep-modulated disinhibition enables replay for memory consolidation, accelerated by ripples》的深度结构化总结：

### 1. 核心问题与整体含义
*   **研究动机**：记忆巩固（包括海马内的突触巩固和向皮层转移的系统巩固）的精确神经机制尚不明确。特别是，虽然锐波纹（SWRs）通常被认为与记忆重现（Replay）和巩固相关，但“无波纹重现”的存在挑战了传统观点。
*   **核心问题**：什么机制启动并调节了睡眠中的自发重现？波纹波在巩固中是否必不可少？去抑制（Disinhibition）在跨脑区记忆转移中扮演什么角色？
*   **整体含义**：论文提出“去抑制”是驱动记忆巩固的核心生物物理机制，它不仅统一了不同睡眠/觉醒状态下的重现现象，还解释了波纹波的多样性及其与重现的解耦关系。

### 2. 方法论：核心思想与技术细节
*   **核心思想**：构建一个生物物理详细的**内嗅皮层-海马-皮层（MEC-DG-CA3-CA1-CR）**闭环网络模型，通过模拟细胞外离子动态（尤其是钾离子 $K^+$）和神经调节因子的变化，驱动系统从觉醒态向慢波睡眠（SWS）转换。
*   **关键技术细节**：
    *   **神经元模型**：采用 Hodgkin-Huxley 类型的随机神经元模型，包含钠、钾、氯离子电流及泵电流。
    *   **离子动态**：模拟细胞外钾离子浓度 $[K^+]_o$ 的波动。睡眠时 $[K^+]_o$ 降低，导致神经元兴奋性下降，并通过特定因子诱发抑制性突触减弱（即去抑制）。
    *   **可塑性规则**：使用三元组脉冲时间依赖可塑性（Triplet-STDP）处理兴奋性突触，并配合动态的前馈、反馈和侧向抑制更新规则。
    *   **突触稳定化**：引入蛋白质介导的突触标记与捕获机制（Synaptic Tagging and Capture），模拟从易失性（Labile）权重向稳定（Stable）权重的转化。
    *   **编码方式**：在觉醒模拟阶段，通过相位前移（Phase Precession）脉冲串刺激 MEC 组合，编码空间序列。

### 3. 实验设计与对比
*   **场景模拟**：
    *   **编码阶段**：模拟动物在空间环境中的探索，通过 MEC 刺激在海马回路中形成序列记忆。
    *   **巩固阶段**：模拟慢波睡眠，观察自发重现、波纹波产生及向皮层（CR）的转移。
    *   **安静觉醒（QW）**：模拟觉醒状态下的重现，研究 MEC 输入对 CA1 重现的门控作用。
*   **对比与消融实验**：
    *   **有无波纹对比**：通过减弱 CA3→CA1 的兴奋性输入，对比“有波纹重现”与“无波纹重现”的巩固速度。
    *   **侧向抑制（LI）梯度**：测试 100%、50%、0% LI 对波纹波形态（链状、长时程、病理性）的影响。
    *   **脑区干预**：消融 MEC 输入、禁用 CA1 去抑制、人工诱导皮层去抑制等，验证各路径在记忆转移中的必要性。
*   **Benchmark**：主要对比已发表的电生理实验数据（如 Yamamoto & Tonegawa 2017 关于 MEC 依赖性的研究，以及 Widloski & Foster 2025 关于无波纹重现的研究）。

### 4. 资源与算力
*   **算力说明**：论文**未明确说明**具体的 GPU 型号或计算集群配置。
*   **计算复杂度**：考虑到模型包含数百个 Hodgkin-Huxley 神经元、复杂的离子动力学方程以及长达数小时（模拟时间）的突触演化，其计算开销显著高于简化的积分发放（LIF）模型。数值积分步长设定为 0.025 ms。

### 5. 实验数量与充分性
*   **实验规模**：论文展示了约 7 组核心实验结果图表，涵盖了从细胞离子水平到系统行为水平的多个维度。
*   **充分性评价**：实验设计非常**充分且具有针对性**。作者不仅复现了正常的生理现象，还通过参数扫描（如改变侧向抑制强度、突触权重缩放）模拟了病理状态（如精神分裂症、阿尔茨海默症相关的波纹异常），增强了结论的客观性和说服力。

### 6. 主要结论与发现
*   **去抑制是核心**：睡眠诱导的去抑制是产生“上下状态”和自发重现的根本原因，而非传统的波纹波启动重现。
*   **波纹波与重现解耦**：波纹波能加速巩固，但并非必不可少。即使在 CA1 传入减弱导致波纹消失的情况下，重现依然能驱动突触和系统巩固（尽管速度变慢）。
*   **侧向抑制决定波纹多样性**：侧向抑制的强弱决定了波纹是离散的“链状”、连续的“长时程”还是无序的“病理性”爆发。
*   **皮层独立性**：皮层去抑制是海马记忆向皮层转移的“门票”，一旦转移完成，皮层重现可脱离海马独立存在。
*   **状态普适性**：去抑制机制在睡眠和安静觉醒中通用，MEC 介导的去抑制解释了觉醒重现对内嗅皮层输入的依赖性。

### 7. 优点
*   **生物物理精度高**：模型整合了离子动态、蛋白质合成、短/长期可塑性等多个尺度的生物学细节，远超一般的抽象神经网络模型。
*   **统一框架**：一个模型解释了重现、波纹波、系统巩固、相位前移以及多种病理现象，具有极强的解释力。
*   **临床关联**：为阿尔茨海默症（星形胶质细胞钾缓冲障碍）和精神分裂症（抑制性神经元功能障碍）提供了明确的机械论解释。

### 8. 不足与局限
*   **规模限制**：受限于计算资源，神经元数量（数百个）仍远小于真实大脑，可能无法完全模拟大规模记忆存储的竞争与干扰。
*   **反馈回路缺失**：模型简化了部分反馈路径（如皮层对海马的自上而下控制、CA3 对 DG 的反馈），这些路径在记忆检索和选择中可能很重要。
*   **REM 睡眠缺失**：研究集中在慢波睡眠（NREM），未涉及快速眼动睡眠（REM）在记忆剪枝或整合中的作用。

（完）
