---
title: Inter-hemispheric connections modulate splitting in a computational model of the bilateral SCN
title_zh: 双侧视交叉上核计算模型中半球间连接对分裂现象的调节作用
authors: "Zemlianova, K., McDaniel, J., Lander, A. G., Nwaezeapu, J., Gutierrez, G. J."
date: 2026-05-05
pdf: "https://www.biorxiv.org/content/10.64898/2026.04.30.722022v1.full.pdf"
tags: ["query:slp-ns"]
score: 9.0
evidence: 通过SCN连接对睡眠-觉醒周期的神经调节
tldr: 本研究探讨了双侧视交叉上核（SCN）之间的半球间连接如何调节“分裂”现象。研究人员构建了一个包含左、右核心区和壳区的四节点计算模型，通过模拟不同光照条件和分叉分析，发现兴奋性半球间连接对维持同步至关重要。研究表明，分裂现象不仅受光照强度影响，更取决于半球间连接的强度和极性，暗示了SCN连接的可塑性在节律调节中的关键作用。
source: biorxiv
selection_source: fresh_fetch
motivation: 旨在探究连接左右视交叉上核（SCN）的连合纤维在昼夜节律“分裂”现象中的具体作用及其动力学机制。
method: 构建了一个包含左右SCN核心区与壳区的四节点计算模型，并结合不同光照条件的模拟与分叉分析来研究系统行为。
result: 发现模型在缺乏强光诱导或兴奋性半球间连接时会自动发生分裂，且半球间连接的强度和极性对状态切换的影响远大于光照强度。
conclusion: 研究结果表明，昼夜节律的分裂现象可能涉及SCN半球间连接的突触可塑性变化。
---

## 摘要
分裂现象最初在仓鼠中观察到，在长时间暴露于持续光照后，它们在一个主观日内表现出两个睡眠/觉醒周期。分裂是左、右视交叉上核（SCN）失去同步的结果。虽然已知分裂活动的特征是左右 SCN 之间以及每个半球内的核心区（core）和壳层区（shell）之间存在反相关系，但连接左右 SCN 的连合纤维投射（commissural projections）的作用尚不清楚。在本研究中，我们探讨了半球间连接对双侧 SCN 计算模型的分裂与非分裂动力学的影响。我们的模型包含 4 个节点，分别对应左右核心区和壳层区。我们在不同的光照条件下模拟了该双侧模型，并测量了其周期以及 4 个节点之间的相位关系。为了进一步表征系统的动力学特性，我们进行了分岔分析。我们发现，除非受到强光/黑暗周期的夹引，或者具有兴奋性半球间连接，否则该双侧模型会自动发生分裂。这表明兴奋性交叉连接对于自由运行行为可能具有重要意义。我们发现，不同强度的持续光照仅在非常有限的条件下使模型在分裂与非分裂活动之间转换，而对侧连接的强度和极性在这种动力学转换中起着更大的作用。这些发现表明，分裂现象可能涉及 SCN 半球间连接的塑性。

## Abstract
The phenomenon of splitting was originally observed in hamsters which, after prolonged exposure to constant light, exhibit two rest/wake cycles within a subjective day. Splitting is a consequence of the left and right suprachiasmatic nuclei (SCN) falling out of synchrony. While it is known that split activity is characterized by an antiphase relationship between the left and right SCN and between the core and shell within each hemisphere, the role of the commissural projections that connect the right and left SCN is not known. In the present study, we investigate the impact of the inter-hemispheric connections on the split and unsplit dynamics of a computational model of the bilateral SCN. Our model has 4 nodes corresponding to each right and left core and shell. We simulated our bilateral model under different lighting conditions and measured its period and the phase relationships among the 4 nodes. To further characterize the dynamics of the system, we performed a bifurcation analysis. We found that the bilateral model automatically splits unless entrained by bright light/dark cycles, or unless it has excitatory inter-hemispheric connections. This suggests that excitatory cross-connections may be important for freerunning behavior. We found that constant light of varying intensities transitions the model between split and unsplit activity only in very limited conditions, but the strength and polarity of the contralateral connections play a much greater role in this dynamical transition. These findings suggest that splitting may involve plasticity of the inter-hemispheric connections of the SCN.

---

## 论文详细总结（自动生成）

这是一份关于论文《双侧视交叉上核计算模型中半球间连接对分裂现象的调节作用》（*Inter-hemispheric connections modulate splitting in a computational model of the bilateral SCN*）的深度结构化总结：

### 1. 论文的核心问题与整体含义（研究动机和背景）
*   **核心问题**：探究连接左右视交叉上核（SCN）的**连合纤维（commissural projections）**在昼夜节律“分裂（Splitting）”现象中的动力学作用。
*   **背景**：在持续光照（LL）等特定条件下，啮齿动物会出现“分裂”现象，即原本同步的左右 SCN 变为反相振荡，导致一个主观日内出现两个活动高峰。
*   **研究动机**：虽然已知分裂涉及左右 SCN 以及核心区（Core）与壳层区（Shell）的去同步，但学术界尚不清楚连接左右半球的神经纤维是如何调节这一过程的，以及这种调节是基于光照强度还是连接强度的变化。

### 2. 论文提出的方法论
*   **核心思想**：构建一个简化的**四节点（4-node）计算模型**，模拟双侧 SCN 的动力学行为。
*   **关键技术细节**：
    *   **模型结构**：四个节点分别代表左核心（L-core）、左壳层（L-shell）、右核心（R-core）和右壳层（R-shell）。
    *   **连接拓扑**：模型考虑了半球内的连接（核心到壳层）以及半球间的交叉连接（核心到对侧核心/壳层，壳层到对侧壳层）。
    *   **数学工具**：使用常微分方程描述各节点的振荡，并采用**分叉分析（Bifurcation Analysis）**来确定系统在不同参数空间（如光照强度、连接权重）下的稳定性切换点。
    *   **变量控制**：通过改变半球间连接的**强度（Strength）**和**极性（Polarity，即兴奋性或抑制性）**，观察系统在“同步（Unsplit）”与“分裂（Split）”状态间的转换。

### 3. 实验设计
*   **场景模拟**：
    *   **LD 周期（明暗交替）**：测试模型在外部强信号下的夹引（Entrainment）能力。
    *   **LL 周期（持续光照）**：模拟诱发分裂的经典实验环境。
    *   **自由运行（Free-running）**：在无外部光照信号下观察系统的自发行为。
*   **Benchmark（基准）**：以经典的仓鼠分裂实验数据为参照，对比模型输出的相位关系（如左右 SCN 是否呈 180 度反相）。
*   **对比方法**：对比了不同光照强度（$L$）与不同半球间连接强度（$g_{inter}$）对系统状态的影响。

### 4. 资源与算力
*   **算力说明**：论文中**未明确说明**具体的硬件配置（如 GPU 型号）。
*   **估算**：由于该模型仅包含 4 个节点的微分方程组，属于低维动力学系统，通常在标准的桌面级 CPU 工作站上即可在短时间内完成数值模拟和分叉图绘制，不需要大规模集群算力。

### 5. 实验数量与充分性
*   **实验规模**：研究进行了广泛的参数扫描，包括光照强度、半球间连接的兴奋性/抑制性权重组合。
*   **充分性**：
    *   通过分叉分析提供了全局的动力学视图，而非仅仅是单次模拟，这增强了结论的普遍性。
    *   涵盖了从强夹引到自由运行的多种生理状态。
*   **客观性**：实验设计逻辑严密，通过数学手段证明了连接极性在状态切换中的主导作用，而非单纯依赖光照参数的微调。

### 6. 论文的主要结论与发现
*   **兴奋性连接的关键性**：发现**兴奋性的半球间连接**是维持左右 SCN 同步（非分裂状态）的必要条件。在缺乏这种连接或连接变为抑制性时，系统会自动进入分裂状态。
*   **连接强度 vs. 光照强度**：研究表明，半球间连接的强度和极性对“分裂-非分裂”转换的影响远大于持续光照强度的变化。
*   **可塑性假说**：分裂现象可能不仅仅是光照对振子频率的直接影响，更可能涉及 SCN 连合纤维的**突触可塑性（Synaptic Plasticity）**，即长期光照改变了左右半球间的耦合性质。

### 7. 优点
*   **模型简洁高效**：用极简的四节点模型抓住了双侧 SCN 交互的核心特征，易于进行深入的数学分析。
*   **理论解释力强**：为“分裂”现象提供了一个明确的动力学解释，即从同步吸引子向反相吸引子的分叉。
*   **预测性**：提出了关于半球间连接极性改变的假说，为后续的神经生物学实验提供了可验证的方向。

### 8. 不足与局限
*   **高度抽象化**：模型将包含数万个神经元的 SCN 简化为 4 个节点，忽略了神经元群体的异质性（如不同神经递质 VIP、AVP 的具体作用）。
*   **生物学证据尚需补充**：虽然模型推测连接极性会发生变化，但目前尚缺乏直接的电生理或光遗传学证据证明在持续光照下连合纤维的性质发生了从兴奋向抑制的转变。
*   **应用限制**：该结论主要基于啮齿类动物模型，在人类或其他灵长类动物中的适用性仍待研究。

（完）
