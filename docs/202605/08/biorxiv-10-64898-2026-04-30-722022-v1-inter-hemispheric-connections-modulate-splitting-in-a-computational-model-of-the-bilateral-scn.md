---
title: Inter-hemispheric connections modulate splitting in a computational model of the bilateral SCN
title_zh: 双侧视交叉上核计算模型中半球间连接对分裂现象的调节作用
authors: "Zemlianova, K., McDaniel, J., Lander, A. G., Nwaezeapu, J., Gutierrez, G. J."
date: 2026-05-05
pdf: "https://www.biorxiv.org/content/10.64898/2026.04.30.722022v1.full.pdf"
tags: ["query:slp-ns"]
score: 9.0
evidence: 仓鼠视交叉上核连接与休息/觉醒周期
tldr: 本研究探讨了双侧视交叉上核（SCN）间连接在昼夜节律“分裂”现象中的作用。通过构建包含左右核心与外壳的四节点计算模型，模拟不同光照条件并进行分岔分析。研究发现，兴奋性半球间连接对维持同步至关重要，而分裂现象可能源于这些连接的塑性变化，而非仅受光照强度影响，为理解生物钟同步机制提供了新视角。
source: biorxiv
selection_source: fresh_fetch
motivation: 旨在探究连接左右视交叉上核（SCN）的连合纤维在昼夜节律分裂现象（即左右SCN失步）中的具体作用及其动力学机制。
method: 构建了一个包含左右核心和外壳四个节点的双侧SCN计算模型，并结合不同光照模拟与分岔分析来研究其周期和相位关系。
result: 研究发现模型在缺乏兴奋性半球间连接时会自动分裂，且半球间连接的强度和极性对状态切换的影响远大于光照强度的变化。
conclusion: 昼夜节律的分裂现象可能涉及SCN半球间连接的塑性改变，强调了跨半球相互作用在维持节律同步中的关键地位。
---

## 摘要
分裂现象最初在仓鼠中观察到，在长时间暴露于持续光照后，它们在一个主观日内表现出两个睡眠/觉醒周期。分裂是左、右视交叉上核（SCN）失去同步的结果。虽然已知分裂活动的特征是左右 SCN 之间以及每个半球内的核心区（core）和壳层区（shell）之间存在反相关系，但连接左右 SCN 的连合纤维投射（commissural projections）的作用尚不清楚。在本研究中，我们探讨了半球间连接对双侧 SCN 计算模型的分裂与非分裂动力学的影响。我们的模型包含 4 个节点，分别对应左右核心区和壳层区。我们在不同的光照条件下模拟了该双侧模型，并测量了其周期以及 4 个节点之间的相位关系。为了进一步表征系统的动力学特性，我们进行了分岔分析。我们发现，除非受到强光/黑暗周期的夹引，或者具有兴奋性半球间连接，否则该双侧模型会自动发生分裂。这表明兴奋性交叉连接对于自由运行行为可能具有重要意义。我们发现，不同强度的持续光照仅在非常有限的条件下使模型在分裂与非分裂活动之间转换，而对侧连接的强度和极性在这种动力学转换中起着更大的作用。这些发现表明，分裂现象可能涉及 SCN 半球间连接的塑性。

## Abstract
The phenomenon of splitting was originally observed in hamsters which, after prolonged exposure to constant light, exhibit two rest/wake cycles within a subjective day. Splitting is a consequence of the left and right suprachiasmatic nuclei (SCN) falling out of synchrony. While it is known that split activity is characterized by an antiphase relationship between the left and right SCN and between the core and shell within each hemisphere, the role of the commissural projections that connect the right and left SCN is not known. In the present study, we investigate the impact of the inter-hemispheric connections on the split and unsplit dynamics of a computational model of the bilateral SCN. Our model has 4 nodes corresponding to each right and left core and shell. We simulated our bilateral model under different lighting conditions and measured its period and the phase relationships among the 4 nodes. To further characterize the dynamics of the system, we performed a bifurcation analysis. We found that the bilateral model automatically splits unless entrained by bright light/dark cycles, or unless it has excitatory inter-hemispheric connections. This suggests that excitatory cross-connections may be important for freerunning behavior. We found that constant light of varying intensities transitions the model between split and unsplit activity only in very limited conditions, but the strength and polarity of the contralateral connections play a much greater role in this dynamical transition. These findings suggest that splitting may involve plasticity of the inter-hemispheric connections of the SCN.

---

## 论文详细总结（自动生成）

这是一份关于论文《Inter-hemispheric connections modulate splitting in a computational model of the bilateral SCN》的结构化深入总结：

### 1. 论文的核心问题与整体含义（研究动机和背景）
*   **核心问题**：研究连接大脑左右半球视交叉上核（SCN）的连合纤维（commissural connections）在昼夜节律“分裂”（Splitting）现象中的具体作用。
*   **背景**：
    *   **分裂现象**：金仓鼠在长时间持续光照（LL）下，原本约24小时的睡眠/觉醒周期会分裂为两个约12小时的周期。
    *   **生理基础**：这种现象源于左右两侧 SCN 失去同步，呈现反相（antiphase）活动，且每个半球内部的核心区（Core）与壳层区（Shell）也呈现反相。
    *   **研究缺口**：虽然已知 SCN 存在半球间投射，但这些连接如何调节分裂与同步状态的动力学转换尚不明确。

### 2. 论文提出的方法论
*   **核心思想**：基于经典的“门控起搏器模型”（Gated Pacemaker Model），将其从单侧扩展为包含左右半球的**四节点双侧模型**。
*   **关键技术细节**：
    *   **四节点结构**：模型包含左核心（$v_{Lcore}$）、左外壳（$v_{Lshell}$）、右核心（$v_{Rcore}$）、右外壳（$v_{Rshell}$）。
    *   **动力学方程**：使用一组常微分方程（ODEs）描述每个节点的活动（$v$）和神经递质门控变量（$z$）。
    *   **反馈机制**：引入一个“疲劳信号”（Fatigue, $F$），它整合左右外壳的平均活动，并反馈抑制核心区。
    *   **连接配置**：模型测试了三种连接方式：共享疲劳信号、外壳间互联（$w_{shell}$）和核心间互联（$w_{core}$）。
*   **分析工具**：利用 **XPPAUT** 软件进行分岔分析（Bifurcation Analysis），通过一维和二维分岔图探索系统在不同参数（光强、连接强度）下的稳定性。

### 3. 实验设计
*   **场景模拟**：
    *   **恒暗（DD）**：模拟自由运行节律。
    *   **光/暗循环（LD）**：测试模型对环境周期的夹引（Entrainment）能力。
    *   **恒光（LL）**：模拟诱发分裂的实验条件。
*   **Benchmark 与对比**：
    *   以经典的单侧 SCN 模型为基准。
    *   对比了**兴奋性**与**抑制性**半球间连接对相位关系的影响。
    *   测量指标包括：振荡周期、相对相位指数（RPI，衡量同步/反相程度）以及从同步到分裂的潜伏期。

### 4. 资源与算力
*   **软件环境**：Matlab（用于时间序列模拟）、Mathematica、XPPAUT（用于分岔分析）。
*   **硬件设备**：Mac Powerbook Pro 和 Mac Studio。
*   **算力说明**：文中未提及使用 GPU 或高性能计算集群。由于该模型仅包含 9 个核心微分方程，属于低计算量模型，常规个人电脑即可胜任。

### 5. 实验数量与充分性
*   **实验规模**：
    *   每个参数点通常进行 **100 次独立试验**，每次试验使用随机生成的初始条件，以验证结果的鲁棒性。
    *   模拟时长达 3000 小时，舍弃前 500 小时以确保系统达到稳态。
*   **充分性评价**：实验设计较为充分。作者不仅通过数值模拟展示了现象，还通过严谨的分岔分析（寻找 Hopf 分岔、Torus 分岔等）从数学层面解释了状态切换的原理。

### 6. 论文的主要结论与发现
*   **兴奋性连接是同步的关键**：在没有兴奋性半球间连接的情况下，模型在恒暗条件下会自动进入分裂状态。这说明生物体维持 24 小时同步节律需要左右半球间的兴奋性耦合。
*   **光强作用有限**：单纯改变持续光照的强度很难触发从同步到分裂的转换，除非在极窄的参数范围内。
*   **连接塑性假说**：分裂现象更有可能源于半球间连接强度或极性的**突触塑性改变**，而非仅仅是光照强度的直接驱动。
*   **双稳态区域**：分岔分析发现了分裂与非分裂模式共存的参数区域，解释了为什么不同个体在相同光照下表现不同。

### 7. 优点
*   **模型创新**：首次构建了能同时捕捉“左右反相”和“核壳反相”的四节点模型（即 4-node split），比之前的相位振子模型更贴近生理现实。
*   **理论深度**：结合了非线性动力学中的分岔理论，为生物实验观察到的现象提供了坚实的数学解释。
*   **预测性**：提出了关于半球间连接塑性的新假说，为未来的神经生物学实验指明了方向。

### 8. 不足与局限
*   **高度简化**：SCN 包含约两万个神经元，模型将其简化为 4 个节点，忽略了神经元群体的异质性和复杂的局部网络动力学。
*   **光照转换矛盾**：模型在恒暗下默认分裂（除非加兴奋连接），这与生物实验中“恒暗下通常同步、恒光下才分裂”的观察存在一定出入，说明模型对光照影响的建模仍有改进空间。
*   **参数依赖**：某些动力学行为（如双稳态）对参数（如 $w_{core}$）高度敏感，可能缺乏生物系统应有的鲁棒性。

（完）
