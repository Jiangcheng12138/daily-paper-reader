---
title: A preoptic circuit triggers rewarming from torpor
authors: "Ohba, A., Narushima, M., Shao, C., Hung, C., Uchida, H., Fukatsu, N., Angarag, U., Takemoto-Kimura, S., Yamanaka, A., Tainaka, K., Ono, D., Yamaguchi, Y., Wake, H., YAMAGUCHI, H."
date: 2026-05-05
pdf: "https://www.biorxiv.org/content/10.64898/2026.04.30.722109v1.full.pdf"
tags: ["query:tr-hb"]
score: 10.0
evidence: 视前区回路触发蛰伏后的复温
tldr: 本研究揭示了小鼠视前区（ADP）中表达促肾上腺皮质激素释放激素（Crh）的神经元是触发从休眠状态复温的关键。研究发现这些神经元在自然复温时被激活，且为限制休眠深度和时长所必需；通过闭环光遗传学激活该环路可迅速诱导棕色脂肪产热并恢复体温。这一发现定义了不同于常规冷防御的特异性复温环路，并可能在冬眠动物中具有保守性。
source: biorxiv
selection_source: fresh_fetch
motivation: 虽然诱导动物进入休眠状态的神经机制已有所发现，但触发主动复温并恢复正常体温的神经环路仍不明确。
method: 利用光遗传学、化学遗传学、热成像记录及神经示踪技术，研究小鼠视前区Crh神经元在禁食诱导休眠及复温过程中的功能。
result: 发现ADP区Crh神经元在复温时特异性激活，其通过投射至侧视前区优先诱导棕色脂肪组织产热，随后引发运动觉醒以恢复体温。
conclusion: 该研究确定了一个专门驱动从休眠中恢复的视前区神经环路，为理解和控制深度低温后的复温提供了神经生物学框架。
---

## Abstract
Torpor is an adaptive hypometabolic state that enables homeotherm to survive periods of energetic challenge. This strategy ranges from short bouts of daily torpor to prolonged hibernation. During torpor, animals markedly suppress metabolic rate, body temperature, heart rate, and respiration, while retaining the ability to rewarm. Torpor therefore comprises two critical transitions -entry into a hypometabolic state and active rewarming-both essential for organismal viability. Although neural mechanisms controlling torpor entry have begun to emerge, the circuits that initiate active rewarming and restore euthermia remain poorly defined. Here we identify corticotropin-releasing hormone (Crh)-expressing neurons in the anterodorsal preoptic area (ADP) as a key population for rewarming from fasting-induced torpor in mice. These neurons become active around natural rewarming and are selectively required to limit the depth and duration of torpor. Unlike pathways mediating acute cold defence, stress hyperthermia, or LPS-induced fever, this circuit is dedicated to promoting timely recovery to euthermia. Closed-loop optogenetic activation of ADPCrh neurons during torpor entry rapidly initiates rewarming, and thermographic recordings show that brown adipose tissue (BAT) thermogenesis precedes locomotor arousal. ADPCrh neurons are predominantly GABAergic and project monosynaptically to the lateral preoptic area, whose terminal activation is sufficient to increase body temperature and locomotor activity. Finally, we find robust activation of ADPCrh neurons during rewarming in a hibernator, suggesting conserved logic for exiting deep torpor. Together, our results define a discrete preoptic circuit that drives recovery from torpor and provide a framework for understanding and potentially controlling timely rewarming from profound hypothermia.

---

## 论文详细总结（自动生成）

这是一份关于论文《A preoptic circuit triggers rewarming from torpor》（视前区回路触发蛰伏后的复温）的结构化深入分析总结：

### 1. 论文的核心问题与整体含义
*   **研究动机：** 蛰伏（Torpor）是恒温动物为应对能量挑战（如寒冷、食物短缺）而采取的一种低代谢、低体温的适应性策略。虽然科学界对动物如何“进入”蛰伏状态的神经机制已有一定了解，但对于动物如何从这种极低代谢状态中“主动复温”并恢复正常体温的神经环路机制仍知之甚少。
*   **核心问题：** 究竟是哪一组神经元充当了触发复温的“开关”？这一过程是通用的冷防御机制，还是存在专门的复温调控路径？

### 2. 论文提出的方法论
*   **核心思想：** 通过全脑活动映射锁定复温相关的脑区，结合空间转录组学鉴定特定神经元亚群，并利用光/化学遗传学手段验证其在复温过程中的必要性与充分性。
*   **关键技术细节：**
    *   **全脑活动映射：** 使用 pS6（磷酸化 S6 核糖体蛋白）作为神经元近期活动的指标，结合 iDISCO 组织清亮技术和光片显微镜成像，利用 ClearMap 软件进行自动化区域量化。
    *   **分子鉴定：** 结合已发表的视前区（POA）空间转录组图谱（MERFISH 数据），通过差异表达分析锁定 ADP 区的 *Crh*（促肾上腺皮质激素释放激素）神经元。
    *   **闭环光遗传系统：** 开发了一套基于红外热成像实时监测体温的闭环系统，当小鼠体温降至 33°C 以下时自动触发光刺激，以精确模拟自然复温过程。
    *   **神经环路解析：** 利用顺行示踪（synaptophysin-EGFP）、全脑投影映射以及离体脑片电生理记录（Patch-clamp）探究 ADP-Crh 神经元的下游投射及突触性质。

### 3. 实验设计
*   **实验场景：** 主要使用禁食诱导的小鼠每日蛰伏模型（环境温度 16°C）。
*   **对比方法与 Benchmark：**
    *   **细胞类型对比：** 对比了 ADP 区的 *Crh* 神经元与 *Nos1* 神经元，发现仅前者与复温显著相关。
    *   **功能特异性对比：** 将复温环路与急性冷防御（4°C 暴露）、应激性高热（换笼应激）、LPS 诱导的发烧反应进行对比，验证该环路的特异性。
    *   **跨物种验证：** 在叙利亚仓鼠（真正的冬眠物种）中重复实验，观察其在深冬眠复温时 ADP-Crh 神经元的激活情况。

### 4. 资源与算力
*   **算力说明：** 论文未明确提及具体的 GPU 型号或大规模模型训练时长。其计算工作主要集中在：
    *   光片显微镜产生的大规模 3D 图像处理（ClearMap 管道）。
    *   基于 Python 的实时红外图像处理与闭环控制算法。
    *   空间转录组数据的统计分析。
    *   这些任务通常在高性能工作站上完成，而非依赖超算集群。

### 5. 实验数量与充分性
*   **实验规模：** 论文包含了从全脑筛选、分子鉴定、功能抑制（化学遗传学/细胞消融）、功能激活（光遗传学）、自然活动监测（钙成像）到环路解析（示踪/电生理）的完整证据链。
*   **充分性与客观性：**
    *   **消融实验：** 既使用了化学遗传学瞬时抑制，也使用了 taCasp3 进行永久性消融，结果一致。
    *   **对照严谨：** 设置了 hrGFP/mCherry 病毒对照、CNO 药物对照、以及同时间点的喂食对照组（排除昼夜节律影响）。
    *   **因果验证：** 实验不仅证明了 ADP-Crh 神经元是复温“必需”的（抑制后蛰伏变深变长），也证明了它是“充分”的（激活后迅速复温）。

### 6. 论文的主要结论与发现
*   **关键群体：** 视前区前背侧（ADP）的 *Crh* 神经元是触发小鼠从蛰伏中复温的关键细胞群。
*   **作用机制：** ADP-Crh 神经元主要是 GABA 能（抑制性）神经元，通过单突触投射抑制侧视前区（LPO）的活动。
*   **生理效应：** 激活该环路会优先诱导棕色脂肪组织（BAT）产热，且产热反应早于行为觉醒（运动增加）。
*   **特异性：** 该环路专门用于从深度低温状态恢复，而不参与常规的体温维持或发烧反应。
*   **进化保守性：** 在冬眠仓鼠中也观察到了该脑区的激活，暗示这可能是哺乳动物退出深低温状态的通用逻辑。

### 7. 优点（亮点）
*   **技术集成度高：** 完美结合了全脑成像、空间转录组和闭环光遗传技术，研究思路清晰。
*   **功能区分细致：** 成功将“复温”这一特定生理过程从广义的“体温调节”中剥离出来，发现了专用的神经环路。
*   **生理意义重大：** 为理解极端环境下生物的生存策略提供了新视角，对人工诱导低代谢状态后的安全复温具有潜在应用价值。

### 8. 不足与局限
*   **下游效应器路径：** 虽然确定了 LPO 是关键下游，但 LPO 之后如何连接到经典的产热中枢（如 DMH 或 RPa）仍需进一步阐明。
*   **触发信号未知：** 论文尚未确定是什么信号（是内部代谢产物还是外部环境感知）在自然状态下激活了 ADP-Crh 神经元。
*   **物种差异：** 虽然在仓鼠中观察到了激活，但由于缺乏对仓鼠的遗传操纵工具，尚未在冬眠物种中进行因果性验证。

（完）
