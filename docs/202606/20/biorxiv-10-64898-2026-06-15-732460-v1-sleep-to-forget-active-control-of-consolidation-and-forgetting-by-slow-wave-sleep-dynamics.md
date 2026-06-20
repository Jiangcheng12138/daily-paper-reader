---
title: "Sleep to forget: active control of consolidation and forgetting by slow-wave sleep dynamics"
title_zh: 睡眠以遗忘：慢波睡眠动力学对巩固与遗忘的主动控制
authors: "Golden, R., Wei, M., Coury, S., Mizrahi-Kliger, A., Ganguly, K., Bazhenov, M."
date: 2026-06-19
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.15.732460v1.full.pdf"
tags: ["query:slp-ns"]
score: 9.0
evidence: 聚焦慢波睡眠动态控制记忆巩固与遗忘
tldr: 慢波睡眠中两种Up状态对记忆有相反作用：慢波巩固记忆，delta波促进遗忘。本文构建丘脑皮层网络模型，通过操纵Ca2+动力学产生两种Up状态，并引入STDP规则。序列学习任务复现了光遗传分离：慢波期间抑制可塑性破坏记忆，delta波期间抑制则增强记忆。机制上，慢波Up状态更长，在干扰输入后提供自发再激活阶段保护记忆，而delta波无法支持。模型预测慢波与delta波的比率可灵活调控记忆巩固与遗忘的平衡。
source: biorxiv
selection_source: fresh_fetch
motivation: 探究慢波睡眠中两种Up状态如何分别控制记忆巩固与遗忘的突触机制。
method: 构建生物物理丘脑皮层网络模型，结合STDP和Ca2+动力学模拟不同Up状态，并用序列学习任务验证。
result: 慢波Up状态通过自发再激活阶段保护记忆，delta波Up状态削弱记忆且使突触更稀疏。
conclusion: 慢波与delta波的比率可灵活调控记忆巩固与遗忘的平衡。
---

## 摘要
睡眠既支持新记忆的巩固，也支持其他记忆的遗忘，但大脑皮层如何灵活控制这些结果仍知之甚少。近期研究表明，在慢波睡眠（SWS）期间，两种类型的Up状态可能扮演着不同且相互竞争的角色：慢波主动巩固记忆痕迹，而delta波则促进其弱化。本文利用一个配备有尖峰时序依赖可塑性的生物物理丘脑皮层网络模型，研究这种分离背后的突触机制。通过操控皮层锥体细胞的内在钙离子动力学，我们在单个网络中同时生成了慢波和delta波的Up状态。采用序列学习任务范式，我们复现了光遗传学分离：在慢波期间移除可塑性会削弱记忆，而在delta波期间移除则会增强巩固。机制上，模型揭示了较长的慢波Up状态提供了一个自发性再激活阶段，发生在干扰输入之后，在此阶段训练过的记忆被选择性再激活并受到保护，而截短的delta波Up状态则无法支持这一阶段。我们进一步发现，与慢波相比，delta波能使突触表征更加稀疏，并预测睡眠期间慢波与delta波的比例可灵活调节巩固与遗忘之间的平衡。

## Abstract
Sleep supports both the consolidation of new memories and the forgetting of others, but how the cortex flexibly controls these outcomes remains poorly understood. Recent work has shown that two types of Up states may play distinct, competing roles during slow-wave sleep (SWS): slow waves actively consolidate memory traces, whereas delta waves promote their weakening. Here we use a biophysical thalamocortical network model equipped with spike-timing-dependent plasticity to investigate the synaptic mechanisms underlying this dissociation. By manipulating the intrinsic Ca2+ dynamics of cortical pyramidal cells, we generate both slow and delta wave Up states within a single network. Using a sequence-learning task paradigm we recapitulate the optogenetic dissociation: removing plasticity during slow waves degrades the memory, while removing it during delta waves enhances consolidation. Mechanistically, the model reveals the longer slow wave Up state affords a spontaneous reactivation phase, occurring after the interfering input, during which the trained memory is selectively reactivated and protected, a phase the truncated delta Up state cannot support. We further find that delta waves sparsen the synaptic representation more than slow waves and predict that the balance between consolidation and forgetting can be flexibly tuned by the ratio of slow to delta waves during SWS.

---

## 论文详细总结（自动生成）

# 论文详细中文总结

## 1. 论文的核心问题与整体含义（研究动机和背景）
- **核心问题**：睡眠既支持新记忆的巩固，也支持其他记忆的遗忘，但大脑皮层如何灵活控制这两种相反的过程仍不清楚。近期研究发现，慢波睡眠（SWS）中存在两种不同类型的Up状态，它们可能扮演竞争角色：**慢波（slow waves）主动巩固记忆痕迹**，而**delta波（delta waves）则促进记忆的弱化**。本文旨在揭示这种分离背后的突触机制。
- **研究意义**：理解睡眠中巩固与遗忘的灵活调控机制，对于揭示记忆的形成与更新、以及睡眠障碍相关疾病的治疗具有重要意义。

## 2. 论文提出的方法论
- **核心思想**：构建一个生物物理丘脑皮层网络模型，通过操控皮层锥体细胞的内在Ca²⁺动力学，在同一网络中同时生成慢波和delta波的Up状态，并在该模型上模拟序列学习任务，观察突触可塑性的变化。
- **关键技术细节**：
  - 网络模型包含丘脑和皮层模块，配备**尖峰时序依赖可塑性（STDP）** 规则。
  - 通过改变锥体细胞的Ca²⁺动态特性（如钙泵速率、钙缓冲区等），使网络产生不同持续时间和频率的Up状态：慢波Up状态持续时间较长，delta波Up状态较短。
  - 在序列学习任务中，训练网络形成顺序记忆模式，并在睡眠阶段分别**光遗传学模拟**：在慢波期间移除可塑性（即抑制STDP），或在delta波期间移除可塑性，观察记忆保留情况。
- **算法流程（文字说明）**：
  1. 初始化网络权重（随机或基于某种预置模式）。
  2. 进行序列学习任务：向网络输入一系列有序脉冲，利用STDP更新突触权重，形成记忆痕迹。
  3. 睡眠阶段：网络自发产生慢波或delta波Up状态；分别在不同Up状态期间施加扰动（如抑制STDP）。
  4. 测试阶段：再次向网络输入相同或干扰序列，评估记忆保留程度（通过读出神经元的响应模式）。
  5. 分析各条件下突触权重分布和再激活特性。

## 3. 实验设计
- **使用数据集/场景**：无传统基准数据集，主要使用**序列学习任务范式**，即让网络学习一系列有序的输入脉冲序列。
- **基准（benchmark）**：参考近期光遗传学实验（如对小鼠SWS中慢波或delta波进行可塑性抑制）的观察结果，将模型行为与这些实验发现进行对比。
- **对比方法**：
  - 慢波期间抑制STDP vs. 不抑制。
  - delta波期间抑制STDP vs. 不抑制。
  - 不同波类型对突触稀疏化影响的比较。

## 4. 资源与算力
- **文中未明确说明**使用了何种GPU型号、数量或训练时长。本工作基于生物物理模型仿真，可能使用CPU集群或少量GPU，但未提供具体信息。

## 5. 实验数量与充分性
- **实验数量**：围绕核心序列学习任务，进行了**至少两组主要对比实验**（慢波和delta波各自的可塑性移除），并分析了突触权重分布、再激活阶段的神经元活动。
- **充分性评估**：
  - 实验设计再现了光遗传学分离现象，机制解释较为清晰。
  - 但该研究为纯模拟工作，缺乏多尺度验证（如不同复杂度的学习任务、不同网络规模）。
  - 未进行多组随机初始化或参数敏感性分析以评估鲁棒性（但文中可能隐含了重复运行，未明确说明）。
  - **客观性**较好，但需更多跨条件验证（如不同刺激强度、不同Up状态时长）。

## 6. 论文的主要结论与发现
- **慢波Up状态（长持续）** 在干扰输入后提供一个**自发性再激活阶段**，训练过的记忆被选择性再激活并受到保护，因此记忆得以巩固。
- **delta波Up状态（短持续）** 无法支持该再激活阶段，且使突触表征更加**稀疏**，促进遗忘。
- **慢波与delta波的相对比例**可灵活调节巩固与遗忘的平衡：慢波比例高时巩固占优，delta波比例高时遗忘占优。
- **机制上**：长Up状态提供了足够时间让干扰后内部动力学会重新激活学习过的序列，而短Up状态则使干扰信号占据主导，造成突触权重重排和记忆弱化。

## 7. 优点
- **方法亮点**：通过操控单一的Ca²⁺动力学参数在同一网络中生成两种不同Up状态，简化了模型复杂性，同时保持生物学合理性。
- **实验设计亮点**：巧妙地结合了光遗传学实验中的干扰逻辑，在模型中进行对照，能够解释已有实验现象并做出预测。
- **解释性**：提出了再激活阶段作为记忆保护的关键时间窗口，提供了清晰的机制假说。

## 8. 不足与局限
- **实验覆盖**：仅使用了序列学习这一种任务，未测试其他类型记忆（如空间、条件反射等），是否具有普适性未知。
- **偏差风险**：模型参数可能经过精细调校以匹配预期结果，缺乏对网络规模、STDP规则细节等参数的充分敏感性分析。
- **应用限制**：完全基于模拟，缺乏真实神经数据的直接验证（如同一网络中的电生理记录）。实际大脑中两种Up状态可能通过不同的丘脑-皮层环路实现，模型过于简化。
- **资源与计算细节缺失**，可复现性受到影响。

（完）
