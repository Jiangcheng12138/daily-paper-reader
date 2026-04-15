---
title: "Sleep-modulated disinhibition enables replay for memory consolidation, accelerated by ripples"
title_zh: 睡眠调节的去抑制促进记忆巩固的重现，并由涟漪波加速
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
记忆巩固涉及复杂的神经机制。在本研究中，我们开发了一个生物物理细节丰富的内嗅-海马-皮层网络模型，揭示了去抑制驱动突触和系统巩固。通过神经调节减弱抑制作用向慢波睡眠过渡，会产生上下状态（up-down states）以及对以相位前移（phase precession）编码的空间序列进行自发的、时间压缩的重现。侧向抑制水平统一了生理性和病理性涟漪（ripples）的多样性。皮层去抑制使得记忆能够从海马体转移。减弱的传入 CA1 突触消除了涟漪但保留了重现，这为减轻涟漪干扰提出了策略。即使没有涟漪，重现也能维持系统巩固，尽管速度较慢；过度的减弱会使其停止，但可以通过增强海马到皮层的连接性来挽救。内侧内嗅皮层（MEC）介导的 CA1 去抑制补偿了减弱的神经调节性 CA1 去抑制，模拟了依赖 MEC 输入的安静觉醒重现；在觉醒期间的这种配置下，人工诱导去抑制会触发驱动巩固的重现和涟漪，强调了去抑制在不同状态下的普适作用。这些见解阐明了去抑制在铭记记忆和促进海马独立性方面的核心地位，调和了实证观察，提出了可测试的预测，并为记忆障碍确定了治疗途径。

## Abstract
Memory consolidation involves elusive neural mechanisms. Here, we develop a biophysically detailed model of the entorhinal-hippocampal-cortical network to reveal that disinhibition drives synaptic and systems consolidation. Transitioning to slow-wave sleep via neuromodulatory dampening of inhibition generates up-down states and spontaneous, time-compressed replays of spatial sequences encoded with phase precession. Lateral inhibition levels unify physiological and pathological ripple diversity. Cortical disinhibition enables memory transfer from hippocampus. Weakened afferent CA1 synapses eliminate ripples but spare replays, proposing strategies to mitigate ripple disruptions. Replays sustain systems consolidation even without ripples, albeit slower; excessive weakening halts it, rescuable by enhanced hippocampal-to-cortical connectivity. Medial entorhinal cortex (MEC)-mediated CA1 disinhibition compensates for attenuated neuromodulatory CA1 disinhibition, mimicking MEC-input-dependent quiet wakefulness replay; under this configuration during wakefulness, artificially inducing disinhibition triggers replays and ripples that drive consolidation, underscoring disinhibitions state-agnostic role. These insights elucidate disinhibitions centrality in engraining memories and fostering hippocampal independence, reconciling empirical observations, yielding testable predictions, and identifying therapeutic avenues for memory disorders.

---

## 论文详细总结（自动生成）

这是一份关于论文《Sleep-modulated disinhibition enables replay for memory consolidation, accelerated by ripples》的深度结构化总结：

### 1. 论文的核心问题与整体含义（研究动机和背景）
论文探讨了**记忆巩固（Memory Consolidation）**的底层神经机制，即大脑如何将短暂的经历转化为长期记忆。这一过程分为**突触巩固**（局部海马增强）和**系统巩固**（海马向皮层转移）。
*   **研究动机**：尽管已知慢波睡眠（SWS）期间的“神经元重现”（Replay）和“尖波波纹”（SWRs）对巩固至关重要，但触发这些现象的生物物理机制仍不明确。
*   **核心争议**：传统观点认为波纹引发了重现，但近期发现存在“无波纹的重现”。论文旨在厘清**去抑制（Disinhibition）**、重现与波纹三者之间的因果关系，并解释记忆如何实现海马独立性。

### 2. 论文提出的方法论
作者开发了一个高度复杂的**内嗅-海马-皮层（MEC-DG-CA3-CA1-CR）生物物理网络模型**。
*   **核心思想**：通过神经调节引起的**去抑制**（即抑制性神经元活性的减弱）作为驱动记忆重现和巩固的核心开关。
*   **关键技术细节**：
    *   **神经元模型**：采用 Hodgkin-Huxley 动力学方程，模拟钠、钾、氯离子流及泵电流。
    *   **离子动力学**：引入细胞外钾离子（$[K^+]_o$）缓冲机制，通过降低钾浓度模拟从觉醒到睡眠的转换，进而诱发去抑制。
    *   **突触可塑性**：结合了**三元组尖峰定时依赖可塑性（Triplet-STDP）**和**蛋白质介导的突触稳定化（Tag-and-Capture）**，模拟突触从不稳定（labile）到稳定（stable）的转变。
    *   **编码机制**：利用**相位前移（Phase Precession）**在 MEC 中编码空间序列。
    *   **抑制系统**：设计了动态的前馈、反馈和侧向抑制（Lateral Inhibition）机制。

### 3. 实验设计
论文通过计算模拟构建了多个场景来验证假设：
*   **场景模拟**：
    1.  **编码阶段**：模拟动物在觉醒状态下探索空间位置 A-D。
    2.  **睡眠阶段**：降低钾缓冲浓度，观察自发的序列重现和波纹生成。
    3.  **系统转移**：观察海马序列如何通过重现转移至皮层（CR）。
*   **对比与 Benchmark**：
    *   **有波纹 vs 无波纹**：通过减弱 CA3 到 CA1 的兴奋性输入，模拟“无波纹重现”场景。
    *   **侧向抑制梯度**：调节侧向抑制强度（0%、50%、100%）以观察波纹形态（链状、长时程、病理性）。
    *   **MEC 状态**：对比 MEC 正常与被静默状态下海马重现的差异。
    *   **觉醒 vs 睡眠**：模拟安静觉醒（QW）状态下的重现机制。

### 4. 资源与算力
*   **算力说明**：论文**未明确提及**具体的硬件型号（如 GPU/CPU 数量）或总训练/模拟时长。
*   **数值计算细节**：文中详述了积分算法，使用随机 Heun 方法处理随机微分方程，步长（$\Delta t$）设定为 0.025 ms。这表明模型具有极高的时间分辨率，计算开销通常较大。

### 5. 实验数量与充分性
*   **实验规模**：作者进行了多维度的参数扫描和消融实验，包括：
    *   不同脑区（MEC, CA3, CA1, CR）的去抑制因子调节。
    *   突触权重演化的长时间序列追踪（数百秒至数小时尺度）。
    *   重现长度、频率及波纹功率的统计分析。
*   **充分性评价**：实验设计非常**充分且系统**。它不仅涵盖了正常的生理状态，还通过调节侧向抑制模拟了类似精神分裂症的病理性波纹，并解释了安静觉醒下的重现逻辑，具有很强的说服力和客观性。

### 6. 论文的主要结论与发现
1.  **去抑制是核心**：睡眠期间钾离子浓度下降导致的去抑制是产生“上下状态”和“自发重现”的根本原因。
2.  **重现与波纹可分离**：波纹能加速巩固，但不是重现的必要条件。即使在“无波纹”情况下，只要存在去抑制，重现仍能驱动记忆转移。
3.  **侧向抑制决定波纹多样性**：侧向抑制的强弱统一了从离散波纹链到长时程波纹，再到病理性融合波纹的各种形态。
4.  **系统巩固路径**：皮层的去抑制是海马记忆向皮层转移的“门控”，转移完成后皮层可实现海马独立重现。
5.  **状态普适性**：去抑制机制同样能解释安静觉醒状态下的重现，且 MEC 介导的去抑制在此时起到了补偿作用。

### 7. 优点
*   **生物物理精度高**：模型不仅停留在抽象网络，而是深入到离子浓度和蛋白质合成层面，能够解释多种电生理观测结果。
*   **统一框架**：一个模型同时解释了突触巩固、系统巩固、波纹多样性以及觉醒/睡眠状态切换，具有极高的理论整合度。
*   **临床关联**：为阿尔茨海默症、精神分裂症等记忆相关障碍提供了潜在的生物物理靶点（如侧向抑制和钾离子缓冲）。

### 8. 不足与局限
*   **反馈回路缺失**：模型简化了部分解剖连接，例如忽略了皮层对海马的反馈调节，这在真实的记忆检索中可能很重要。
*   **规模限制**：虽然生物物理细节丰富，但神经元数量（数百个）相比真实大脑仍较小，可能无法完全捕捉大规模群体编码的涌现特性。
*   **硬件细节不明**：缺乏计算资源说明，使得其他研究者难以评估复现该模型所需的计算成本。
*   **REM 睡眠缺失**：研究集中在慢波睡眠（NREM），未涉及快速眼动睡眠（REM）在记忆剪枝或整合中的协同作用。

（完）
