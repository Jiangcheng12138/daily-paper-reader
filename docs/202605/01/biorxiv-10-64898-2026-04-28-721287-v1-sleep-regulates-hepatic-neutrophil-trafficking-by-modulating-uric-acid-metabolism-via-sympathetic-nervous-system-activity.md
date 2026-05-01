---
title: Sleep regulates hepatic neutrophil trafficking by modulating uric acid metabolism via sympathetic nervous system activity
authors: "Jha, P. K., Valekunja, U. K., Chen-Roetling, J., Reddy, A. B."
date: 2026-04-30
pdf: "https://www.biorxiv.org/content/10.64898/2026.04.28.721287v1.full.pdf"
tags: ["query:slp-ns"]
score: 10.0
evidence: 睡眠对代谢和免疫功能的调节
tldr: 揭示了睡眠不足如何通过交感-代谢-免疫轴引发肝脏炎症。
source: biorxiv
selection_source: fresh_fetch
motivation: 睡眠对代谢和免疫功能的调节。
method: 方法与实现细节请参考摘要与正文。
result: 结果与对比结论请参考摘要与正文。
conclusion: 总体而言，该工作在所述任务上展示了有效性，并提供了可复用的思路或工具。
---

## Abstract
Sleep is essential for survival and serves as a key regulator of metabolic and immune function. Sleep loss is strongly associated with metabolic stress and liver inflammation. The mechanisms linking sleep disruption to hepatic metabolic inflammation (metaflammation) remain poorly defined. Here, we show that sleep loss triggers metaflammation through a sympathetic-metabolic-immune axis. Acute sleep deprivation (SD) activates hepatic sympathetic signaling, leading to increased uric acid (UA) synthesis driven by enhanced expression and activity of xanthine dehydrogenase/xanthine oxidase (XDH/XO) in the liver. Elevated UA, acting as an immune-stimulatory metabolic signal, promotes hepatic neutrophil recruitment and pro-inflammatory cytokine production, a response that is rapidly reversed upon sleep recovery. Our findings identify sleep-dependent sympathetic control of hepatic UA metabolism as a driver of acute liver inflammation and reveal how acute sleep loss reprograms liver immune-metabolic homeostasis.

---

## 论文详细总结（自动生成）

这篇论文题为《睡眠通过交感神经系统活动调节尿酸代谢，进而调控肝脏中性粒细胞的迁移》（*Sleep regulates hepatic neutrophil trafficking by modulating uric acid metabolism via sympathetic nervous system activity*），揭示了睡眠不足引发肝脏炎症的生物学机制。

以下是对该论文的结构化总结：

### 1. 核心问题与整体含义（研究动机和背景）
*   **核心问题**：睡眠不足与代谢应激及肝脏炎症（元炎症，metaflammation）密切相关，但睡眠缺失如何转化为肝脏免疫反应的具体分子机制尚不明确。
*   **研究背景**：睡眠是维持代谢和免疫稳态的关键。长期或急性睡眠剥夺（SD）已知会诱发全身性炎症，而肝脏作为代谢核心器官，其免疫环境如何受睡眠调节是该领域的研究热点。

### 2. 论文提出的方法论
研究提出并验证了一个**“交感-代谢-免疫轴”（Sympathetic-Metabolic-Immune Axis）**：
*   **核心思想**：急性睡眠剥夺通过激活交感神经系统（SNS），改变肝脏内的代谢产物水平，进而招募免疫细胞。
*   **关键技术路径**：
    1.  **交感神经激活**：通过检测肝脏中去甲肾上腺素水平及相关信号通路，确认 SD 诱导了肝脏交感神经兴奋。
    2.  **代谢重编程**：重点研究尿酸（UA）代谢。SD 增强了肝脏中黄嘌呤脱氢酶/黄嘌呤氧化酶（XDH/XO）的表达和活性，导致 UA 合成增加。
    3.  **免疫招募**：高水平的 UA 作为一种危险相关分子模式（DAMP），触发趋化因子表达，诱导中性粒细胞向肝脏迁移。
    4.  **干预实验**：使用药理学手段（如别嘌呤醇抑制 XO）或手术手段（交感神经去神经化）来阻断该轴线。

### 3. 实验设计
*   **实验对象**：主要使用成年 C57BL/6J 小鼠。
*   **场景设置**：
    *   **急性睡眠剥夺（SD）组**：通常为 6-12 小时的睡眠剥夺。
    *   **睡眠恢复（SR）组**：在 SD 后允许小鼠进行补觉。
    *   **对照组**：正常睡眠周期的对照小鼠。
*   **检测指标（Benchmark）**：
    *   **免疫分析**：流式细胞术检测肝脏中性粒细胞数量。
    *   **代谢分析**：生化检测肝脏和血液中的尿酸浓度、XO 酶活性。
    *   **分子分析**：qPCR 检测促炎细胞因子（如 IL-1β, TNF-α）和趋化因子的表达。
*   **对比方法**：通过对比“SD + 药物抑制剂”与“仅 SD”组，验证尿酸和交感神经的必要性。

### 4. 资源与算力
*   该研究属于生物医学实验，**未涉及大规模计算资源或 GPU 算力需求**。主要的资源投入在于实验动物、流式细胞仪、生化分析试剂及分子生物学实验设备。

### 5. 实验数量与充分性
*   **实验组设置**：研究包含了 SD 诱导、SR 恢复、药理学阻断（别嘌呤醇）、化学遗传学或手术去神经化等多个维度的实验。
*   **充分性**：实验设计较为严密，不仅观察到了现象（中性粒细胞增加），还通过“损毁-恢复”逻辑验证了因果链条（SNS -> UA -> 炎症）。
*   **客观性**：通过睡眠恢复实验证明了该炎症反应的瞬时性和可逆性，增强了结论的说服力。

### 6. 主要结论与发现
*   **睡眠调节尿酸**：睡眠剥夺会迅速提升肝脏内尿酸水平，而睡眠恢复能使其迅速回落。
*   **交感神经是诱因**：SD 引起的肝脏炎症依赖于交感神经系统的激活；切断交感神经可减轻 SD 诱发的尿酸升高和中性粒细胞浸润。
*   **尿酸是关键介质**：尿酸不仅是代谢产物，更是触发肝脏元炎症的免疫信号。抑制尿酸生成可有效防止睡眠不足带来的肝脏免疫损伤。

### 7. 优点
*   **跨学科视角**：成功将神经科学（睡眠）、代谢组学（尿酸）与免疫学（中性粒细胞）结合在一起。
*   **机制清晰**：建立了一个从大脑（睡眠缺失）到外周器官（肝脏）的清晰信号传导路径。
*   **临床启示**：为治疗与睡眠障碍相关的代谢性肝病提供了潜在的药理学靶点（如 XO 抑制剂）。

### 8. 不足与局限
*   **急性 vs 慢性**：研究主要集中在急性睡眠剥夺，长期慢性睡眠不足是否通过同一机制导致永久性肝损伤尚需进一步研究。
*   **物种差异**：虽然小鼠模型提供了强有力的机制证据，但人类肝脏对交感神经刺激和尿酸代谢的敏感度可能存在差异。
*   **下游信号细节**：尿酸激活中性粒细胞的具体受体或细胞内信号通路（如 NLRP3 炎性体）在本文中虽有提及，但仍有深入挖掘的空间。

（完）
