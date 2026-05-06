---
title: Inter-hemispheric connections modulate splitting in a computational model of the bilateral SCN
title_zh: 半球间连接调节双侧视交叉上核（SCN）计算模型中的分裂现象
authors: "Zemlianova, K., McDaniel, J., Lander, A. G., Nwaezeapu, J., Gutierrez, G. J."
date: 2026-05-05
pdf: "https://www.biorxiv.org/content/10.64898/2026.04.30.722022v1.full.pdf"
tags: ["query:slp-ns"]
score: 9.0
evidence: 视交叉上核对休息/觉醒周期的调节
tldr: 本研究探讨了双侧视交叉上核（SCN）之间的半球间连接在“分裂”现象中的作用。研究人员构建了一个包含左、右核心区和壳区的四节点计算模型，通过模拟不同光照条件和分叉分析，发现模型在缺乏强光诱导或兴奋性半球间连接时会自动进入分裂状态。结果表明，半球间连接的强度和极性对维持同步至关重要，暗示分裂现象可能涉及SCN连接的可塑性。
source: biorxiv
selection_source: fresh_fetch
motivation: 旨在探究连接左右视交叉上核（SCN）的连合纤维在昼夜节律“分裂”现象（即左右SCN不同步）中的具体作用。
method: 构建了一个包含左右核心区和壳区的四节点SCN计算模型，并结合不同光照条件下的数值模拟与分叉分析进行研究。
result: 发现模型在没有强光夹带或兴奋性半球间连接的情况下会自动分裂，且连接强度和极性对动力学转换的影响远大于光照强度。
conclusion: 研究表明半球间连接的兴奋性对维持自由运行行为至关重要，且节律分裂可能源于SCN半球间连接的可塑性变化。
---

## 摘要
分裂现象最初在仓鼠中被观察到，在长时间暴露于持续光照后，仓鼠在一个主观日内表现出两个睡眠/觉醒周期。分裂是左右视交叉上核（SCN）失去同步的结果。虽然已知分裂活动的特征是左右 SCN 之间以及每个半球内的核心区（core）和壳层区（shell）之间存在反相关系，但连接左右 SCN 的连合纤维投射（commissural projections）的作用尚不清楚。在本研究中，我们调查了半球间连接对双侧 SCN 计算模型的分裂和非分裂动力学的影响。我们的模型包含 4 个节点，分别对应左右两侧的核心区和壳层区。我们在不同的光照条件下模拟了该双侧模型，并测量了其周期以及 4 个节点之间的相位关系。为了进一步表征系统的动力学，我们进行了分岔分析。我们发现，除非受到强光/黑暗周期的夹带，或者具有兴奋性半球间连接，否则该双侧模型会自动发生分裂。这表明兴奋性交叉连接对于自由运行行为可能具有重要意义。我们发现，不同强度的持续光照仅在非常有限的条件下使模型在分裂和非分裂活动之间转换，而对侧连接的强度和极性在这种动力学转换中起着更大的作用。这些发现表明，分裂可能涉及 SCN 半球间连接的可塑性。

## Abstract
The phenomenon of splitting was originally observed in hamsters which, after prolonged exposure to constant light, exhibit two rest/wake cycles within a subjective day. Splitting is a consequence of the left and right suprachiasmatic nuclei (SCN) falling out of synchrony. While it is known that split activity is characterized by an antiphase relationship between the left and right SCN and between the core and shell within each hemisphere, the role of the commissural projections that connect the right and left SCN is not known. In the present study, we investigate the impact of the inter-hemispheric connections on the split and unsplit dynamics of a computational model of the bilateral SCN. Our model has 4 nodes corresponding to each right and left core and shell. We simulated our bilateral model under different lighting conditions and measured its period and the phase relationships among the 4 nodes. To further characterize the dynamics of the system, we performed a bifurcation analysis. We found that the bilateral model automatically splits unless entrained by bright light/dark cycles, or unless it has excitatory inter-hemispheric connections. This suggests that excitatory cross-connections may be important for freerunning behavior. We found that constant light of varying intensities transitions the model between split and unsplit activity only in very limited conditions, but the strength and polarity of the contralateral connections play a much greater role in this dynamical transition. These findings suggest that splitting may involve plasticity of the inter-hemispheric connections of the SCN.

---

## 论文详细总结（自动生成）

这是一份关于论文《Inter-hemispheric connections modulate splitting in a computational model of the bilateral SCN》（半球间连接调节双侧视交叉上核计算模型中的分裂现象）的结构化总结：

### 1. 论文的核心问题与整体含义
*   **研究背景**：哺乳动物的昼夜节律由大脑中的视交叉上核（SCN）控制。正常情况下，左右两侧 SCN 是同步的。但在特定条件（如长时间暴露于持续光照 LL）下，某些动物（如仓鼠）会出现“分裂”（Splitting）现象，即一个主观日内出现两个活动高峰，这对应于左右 SCN 失去了同步，呈现出约 180 度的反相运动。
*   **核心问题**：虽然已知 SCN 内部存在核心区（Core）和壳层区（Shell）的区分，但连接左右半球的“连合纤维”（Commissural projections）在维持同步或诱导分裂中的具体作用尚不明确。
*   **整体含义**：本研究旨在通过计算建模，探讨半球间连接的强度和极性（兴奋或抑制）如何影响 SCN 的同步状态，从而揭示生物节律分裂的潜在动力学机制。

### 2. 论文提出的方法论
*   **核心思想**：构建一个简化的四节点（4-node）计算模型，代表左核心（LC）、左壳（LS）、右核心（RC）和右壳（RS），通过常微分方程（ODE）模拟其相互作用。
*   **关键技术细节**：
    *   **单节点模型**：采用经典的 **Goodwin 振荡器**，模拟 mRNA 与蛋白质之间的负反馈回路。
    *   **网络拓扑**：
        *   **同侧连接**：核心区向壳层区发送兴奋性信号。
        *   **对侧（半球间）连接**：包括核心-核心、壳-壳以及核心-壳之间的交叉连接。
    *   **光照输入**：光照强度（L）作为参数直接作用于左右核心区的 mRNA 转录速率。
*   **分析流程**：
    1.  **数值模拟**：在不同光照条件（LD 12:12 周期或 LL 持续光照）下运行模型。
    2.  **分叉分析（Bifurcation Analysis）**：利用动力系统理论，寻找系统从同步态切换到分裂态的临界参数点。

### 3. 实验设计
*   **场景设置**：
    *   **光/暗周期（LD）**：测试模型在外部强迫节律下的夹带能力。
    *   **持续光照（LL）**：模拟自由运行状态，观察不同光强对分裂的影响。
*   **对比变量**：
    *   **连接极性**：对比半球间连接为兴奋性（Excitatory）与抑制性（Inhibitory）时的动力学差异。
    *   **连接强度**：扫描不同耦合系数（$g_{cc}, g_{ss}$ 等）对相位关系的影响。
*   **Benchmark**：以生物实验中观察到的仓鼠分裂行为特征（左右反相、核心/壳层相位差）作为模型有效性的衡量标准。

### 4. 资源与算力
*   **算力说明**：论文中未明确提及具体的 GPU 型号或大规模计算集群。
*   **工具使用**：研究使用了 **Python**（Matplotlib, NumPy）进行数值模拟，并使用 **XPPAUT** 软件进行分叉分析。由于是基于少量 ODE 的模型，该研究对算力要求较低，普通工作站即可完成。

### 5. 实验数量与充分性
*   **实验规模**：研究进行了大量的参数扫描（Parameter Sweeps），涵盖了从弱耦合到强耦合、从低光强到高光强的多种组合。
*   **充分性**：通过分叉图（Bifurcation diagrams）系统地展示了系统状态的转换边界，而非仅仅依靠个别案例的模拟。这种方法在动力学研究中被认为是充分且严谨的。
*   **客观性**：模型不仅重现了分裂现象，还探讨了为何在某些参数下无法维持同步，提供了正反两方面的论证。

### 6. 主要结论与发现
*   **兴奋性连接维持同步**：强有力的半球间兴奋性连接是维持左右 SCN 同步（非分裂）的关键。
*   **自动分裂倾向**：在缺乏强光夹带或当半球间连接变为抑制性时，模型会自动进入分裂状态（左右反相）。
*   **光照的间接作用**：持续光照强度本身并不直接导致分裂，而是通过改变振荡器的内部参数，使系统更容易跨越分叉点进入分裂区。
*   **可塑性假说**：研究提出，生物体内的分裂现象可能源于 SCN 半球间连接的功能性可塑性（例如神经递质性质的改变或突触强度的调整）。

### 7. 优点
*   **模型简洁高效**：用 4 个节点抓住了双侧 SCN 的核心解剖特征，易于进行深入的数学分析。
*   **理论与现象结合**：成功解释了为什么分裂状态在生物学上是稳定的，并为“分裂”提供了明确的动力学定义。
*   **预测性**：提出了关于半球间连接极性的假说，为未来的电生理实验提供了可验证的方向。

### 8. 不足与局限
*   **高度简化**：SCN 包含约两万个神经元，将其简化为 4 个节点忽略了神经元群体的异质性和局部同步的复杂性。
*   **缺乏实验验证**：结论主要基于计算推导，目前尚缺乏直接的生物学实验（如光遗传学干预连合纤维）来证实半球间连接在分裂过程中的极性变化。
*   **物种局限性**：模型主要基于仓鼠的数据，而不同物种（如小鼠或大鼠）在 LL 条件下的反应存在显著差异，模型的普适性有待进一步探讨。

（完）
