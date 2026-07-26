---
title: Serotonin induces DOWN states across the anesthetized mouse forebrain
title_zh: 血清素诱导麻醉小鼠前脑的DOWN状态
authors: "Grossmann, R., Meijas, J. F., International Brain Laboratory,, Mainen, Z. F., Meijer, G. T."
date: 2026-07-20
pdf: "https://www.biorxiv.org/content/10.64898/2026.07.14.738517v1.full.pdf"
tags: ["query:slp-ns"]
score: 8.0
evidence: 血清素诱导与睡眠慢波相关的DOWN状态
tldr: 5-羟色胺对前脑网络状态的影响存在争议，光遗传fMRI显示抑制活动而电刺激报告UP状态。本研究结合光遗传5-HT刺激与Neuropixel大规模记录，发现选择性5-HT释放诱导前脑皮层和纹状体出现DOWN状态，中脑动态几乎不受影响。多区域计算模型表明，这种转换源于网络同步而非直接DRN输入。成果揭示了5-HT通过全局网络同步调控慢振荡的新机制。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-14-738517-v1/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1344, \"height\": 1378, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-14-738517-v1/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1756, \"height\": 1765, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-14-738517-v1/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1788, \"height\": 1358, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-14-738517-v1/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1733, \"height\": 1003, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-14-738517-v1/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1724, \"height\": 583, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-14-738517-v1/fig-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 1766, \"height\": 439, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-14-738517-v1/fig-007.webp\", \"caption\": \"\", \"page\": 0, \"index\": 7, \"width\": 1759, \"height\": 631, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-14-738517-v1/fig-008.webp\", \"caption\": \"\", \"page\": 0, \"index\": 8, \"width\": 1779, \"height\": 548, \"label\": \"Figure\"}]"
tables_json: "[{\"url\": \"assets/tables/biorxiv/biorxiv-10-64898-2026-07-14-738517-v1/table-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1361, \"height\": 460, \"label\": \"Table\"}]"
motivation: 解决5-HT对前脑网络状态调控的争议，明确其诱导DOWN状态还是UP状态。
method: 结合光遗传5-HT刺激与Neuropixel大规模记录，分析小鼠前脑多区域神经活动，并用计算模型模拟。
result: 5-HT释放诱导前脑皮层和纹状体DOWN状态，中脑动态几乎不变，且转换源于网络同步。
conclusion: 5-HT通过全局网络同步而非直接DRN输入诱导前脑DOWN状态。
---

## 摘要
中缝背核（DRN）的血清素能神经元广泛投射到前脑，但它们对全局网络状态的影响仍存在争议。血清素被认为调节慢振荡，即所谓的UP和DOWN状态，这些状态出现在睡眠和轻度麻醉期间。虽然光遗传学fMRI表明血清素（5-HT）抑制全脑活动，但经典的电气刺激研究报告了皮层UP状态的诱导。为了解决这一矛盾，我们将光遗传学5-HT刺激与轻度麻醉小鼠前脑的大规模Neuropixel记录相结合。我们证明选择性5-HT释放一致地在皮层和纹状体诱导DOWN状态，而中脑动力学基本不受影响。一个基于生物学合理连接的多区域计算模型表明，在某些区域，这些转变源于网络水平的同步化，而非直接的DRN输入。

## Abstract
Serotonergic neurons in the dorsal raphe nucleus (DRN) project extensively throughout the forebrain, yet their influence on global network states remains controversial. Serotonin is implicated in regulating slow-oscillations, so-called UP and DOWN states, which occur during sleep and light anesthesia. While optogenetic fMRI suggests that serotonin (5-HT) suppresses brain-wide activity, classical electrical stimulation studies report the induction of cortical UP states. To resolve this discrepancy, we combined optogenetic 5-HT stimulation with large-scale Neuropixel recordings across the forebrain of lightly anesthetized mice. We demonstrate that selective 5-HT release consistently induces DOWN states across the cortex and striatum, while leaving midbrain dynamics largely unaffected. A multi-area computational model constrained by biologically plausible connectivity, indicates that in certain regions the transitions arises from network-level synchronization rather than direct DRN input.

---

## 论文详细总结（自动生成）

好的，请查收对给定论文的结构化、深入、客观的总结。

### 论文详细总结

#### 1. 核心问题与整体含义

- **研究动机**：血清素（5-HT）是一种重要的神经调质，被认为参与调节睡眠和麻醉状态下大脑的慢振荡（UP和DOWN状态）。然而，现有文献对该效应的描述充满矛盾：光遗传fMRI研究显示血清素抑制全脑活动，而经典的电刺激研究则报告其诱导了皮层UP状态。这种矛盾阻碍了我们对血清素如何调控全局网络状态的理解。
- **核心问题**：选择性激活中缝背核（DRN）的血清素能神经元，对麻醉小鼠前脑的神经活动和UP-DOWN动态产生何种影响？
- **整体含义**：该研究旨在通过高时空分辨率的大规模电生理记录，解决血清素作用争议，并揭示其作用机制，特别是其影响是否源于直接的DRN输入还是通过网络同步化间接发生。研究结果支持血清素诱导**全球性的DOWN状态**，且深层机制涉及网络间的**同步化**。

#### 2. 方法论

- **核心思想**：结合光遗传学实现对DRN血清素能神经元的**选择性激活**，同时利用Neuropixel探针进行**大规模、跨脑区**的同步电生理记录，以高时间分辨率捕捉细胞水平的UP-DOWN状态动态，并辅以计算模型验证机制。
- **关键技术细节**:
    1.  **动物模型**：使用SERT-Cre小鼠，在DRN注射表达Channelrhodopsin (ChR2) 的病毒，实现血清素能神经元特异性表达。
    2.  **光遗传刺激**：通过植入的光纤向DRN传递蓝色光脉冲（465 nm，10 ms脉冲，主要使用25 Hz，持续1秒），以激活血清素释放。
    3.  **神经记录**：急性期使用Neuropixel探针进行多脑区记录（包括前额叶皮层、视觉皮层、纹状体、丘脑、海马、杏仁核和中脑等），每个小鼠进行7次推进，覆盖8个主要区域。通过后处理，基于Di-I标记追踪探针轨迹并映射到标准Allen脑图谱。
    4.  **数据分析**：
        - **单神经元分析**：计算调制指数（Modulation Index, MI）和ZETA检验评估神经元是否被显著调节。
        - **UP-DOWN状态量化**：应用**两状态隐马尔可夫模型（HMM）** 从刺激对齐的尖峰速率中推断DOWN状态的概率。
        - **计算模型**：构建多区域双稳态发放率模型。每个脑区由局部的兴奋-抑制（EI）电路和适应性机制(A)构成。脑区间的投射强度及DRN对各区域的投射强度均来自**Allen小鼠脑连接组图谱**。通过改变耦合强度G来探究网络同步化的作用。模拟5-HT刺激时，主要采用**抑制兴奋性（E-）** 的方法。
- **公式或算法流程**:
    - 调制指数: `MI = 2(auROC - 0.5)`，auROC为刺激前后尖峰计数的接收者操作特征曲线下面积。
    - 发放率模型局部电路:
        - `τE d(rE)/dt = -rE(t) + φE(JEE rE - JEI rI - a + σξE)`
        - `τI d(rI)/dt = -rI(t) + φI(JIE rE - JII rI + σξI)`
        - `τa da/dt = -a(t) + βrE(t)`
        - 其中 `φX(x) = gX [x - θX]_+` 为阈值线性传递函数。
    - 模拟5-HT输入: `IxDRN(t) = S * Dx * u(t)`，其中`Dx`为由Allen图谱确定的DRN投射密度，`u(t)`为模拟5-HT时序动态的函数，`S`为刺激强度。

#### 3. 实验设计

- **数据集**：
    - **实验数据**：来自7只SERT-Cre小鼠的Neuropixel电生理记录，在轻度异氟烷麻醉下进行。记录了皮层、纹状体、丘脑、海马、杏仁核、中脑等区域的单细胞活动。
    - **结构数据**：Allen小鼠脑连接组图谱提供脑区间（inter-areal）和DRN到各区域（DRN-to-region）的投射密度数据；Allen脑图谱提供的5-HT受体表达数据。
- **Benchmark / 对照**：
    - **内部对照**：对2只病毒注射失败（无ChR2表达）的小鼠进行了相同的实验，作为光遗传刺激的**光学效应控制**。
    - **基线比较**：在分析DOWN状态概率变化时，以刺激前-1到0秒的基线水平作为参照，进行t检验。
    - **状态子类型分析**：将刺激发生时间分为“刺激开始时处于UP状态”和“刺激开始时处于DOWN状态”，以分别考察其对状态转换和状态维持的作用。
- **对比方法**：该研究本身并没有对比其他公有的方法，而是通过设计多种刺激频率（1, 5, 10, 25 Hz）、比较有无ChR2表达的对照组，以及在计算模型中测试不同机制（E-, I+, E+, I-）来论证其核心观点。

#### 4. 资源与算力

- 论文未明确提及使用的GPU型号、数量或模型训练时长等计算资源。考虑到其主要使用计算模型进行模拟，而非大规模深度学习模型，对算力的需求可能不高，但具体细节未披露。

#### 5. 实验数量与充分性

- **实验数量**：核心实验来自5只表达ChR2的小鼠，每只小鼠进行了7个Neuropixel探针推进，覆盖8个脑区，进行了多次（各50次）不同频率（4种）的刺激，数据量充足。加上2只对照小鼠，实验设计严谨。
- **充分性**：
    - **正面**：实验设计**较为全面**，覆盖了广泛的前脑区域，包括了关键对照（无ChR2表达）和不同刺激参数（频率）。对状态转换的深入分析（区分UP/DOWN起始）和对受体表达的相关性分析都加强了结论的可靠性。
    - **客观性/公平性**：数据分析使用了标准化的HMM和统计检验，结果客观。计算模型的参数通过拟合实验数据进行调节，验证了其复现实验现象的能力，并提供了一个探索机制的框架，这符合科学研究的公平性。
    - **局限性**：实验数量（n=5小鼠）属于中等规模。虽然脑区覆盖广，但每个脑区的神经元数量根据图1e显示，不同区域间差异很大（从几十到几百不等），这可能影响某些区域的统计效力。模型验证部分，其结论强烈依赖于模型参数的选择，对于未覆盖的机制（如闭环连接、谷氨酸共递质效应）是开放性问题。

#### 6. 主要结论与发现

1.  **血清素抑制神经活动并诱导DOWN状态**：选择性光遗传激活DRN血清素能神经元，在轻度麻醉下快速、一致地抑制了大多数前脑区域（皮层、纹状体、丘脑、海马、杏仁核）的神经活动，并诱导了显著的DOWN状态。
2.  **中脑豁免**：中脑在5-HT刺激下未表现出明显的DOWN状态诱导，表明其动力学模式具有区域特异性。
3.  **DRN投射强度与抑制程度无关**：实验数据中，5-HT诱导的抑制强度与DRN到该区域的解剖投射密度没有显著相关性。
4.  **机制：网络同步化至关重要**：计算模型揭示，当脑区间耦合强度高时，即使DRN投射很弱的区域（如视觉皮层）也会因网络其他区域的同步驱动而进入DOWN状态。这表明**下游区域的DOWN状态并非完全由直接的DRN输入决定，而是由网络层面的相互作用介导**。
5.  **受体相关性**：抑制幅度与5-HT1f和5-HT2a受体的表达水平呈显著正相关。
6.  **状态切换的双重模式**：血清素既能通过延长持续中的DOWN状态，也能通过促进从UP状态快速转换到DOWN状态来实现其效应。

#### 7. 优点

1.  **技术先进**：结合了光遗传学的高特异性与Neuropixel探针的高时空分辨率、大规模记录能力，首次在单细胞和全局网络尺度同时揭示了血清素的作用。
2.  **桥接鸿沟**：成功连接了此前fMRI和局部电生理研究之间的矛盾，提供了更完整的图景。
3.  **实验设计严谨**：包含了严格的光学对照（无ChR2表达小鼠）以及对不同刺激频率和状态起始条件的细致分析。
4.  **计算模型富有洞见**：模型不仅复现了实验结果，还通过参数调整（如耦合强度G）揭示了“网络同步化”这一非直观的深层机制，为理解血清素作用的传播方式提供了有力的理论解释。
5.  **数据开放共享**：数据和代码的公开增加了研究的可重复性和利用价值。

#### 8. 不足与局限

1.  **模型简化**：计算模型是开放环路架构（DRN只投射到下游，不收下游反馈），未考虑真实脑中的闭环交互。此外，模型中忽略了血清素能神经元可能共释放谷氨酸这一已知现象。
2.  **机制理解有限**：虽然模型提出了一种可能的机制，且显示了与受体表达的相关性，但**无法确证**5-HT1f和5-HT2a受体的具体作用，需要进一步的药理学实验验证。
3.  **状态推广性存疑**：研究在麻醉条件下进行，异氟烷诱导的UP-DOWN状态与自然非快速眼动（NREM）睡眠中的状态虽然相似，但并非完全等同，结论向清醒或自然睡眠状态推广需谨慎。
4.  **基因型和物种单一性**：研究仅在SERT-Cre小鼠品系中进行，验证了其在C57Bl/6背景下的效应。没有在非转基因动物（如野生型小鼠）或其他物种（如大鼠）中验证，存在物种/品系特异性风险。
5.  **样本量局限**：虽然记录了大量神经元，但有效的实验动物数量（n=5）相对较小，个别小鼠的影响可能较大。

（完）
