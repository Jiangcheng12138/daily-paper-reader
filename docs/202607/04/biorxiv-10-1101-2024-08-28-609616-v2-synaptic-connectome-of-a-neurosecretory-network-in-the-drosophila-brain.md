---
title: Synaptic connectome of a neurosecretory network in the Drosophila brain
title_zh: 果蝇脑中神经分泌网络的突触连接组
authors: "McKim, T. H., Gera, J., Gayban, A. J., Christie, K., Shin, J., Reinhard, N., Manoli, G., Hilpert, S., Callaerts, P., van Breugel, F., Helfrich-Forster, C., Zandawala, M."
date: 2026-06-29
pdf: "https://www.biorxiv.org/content/10.1101/2024.08.28.609616v2.full.pdf"
tags: ["query:slp-ns"]
score: 8.0
evidence: 神经分泌网络的突触连接组，涉及睡眠和行为调控
tldr: 激素调控动物行为与生理，但神经分泌网络如何被调控尚不清楚。本研究构建了果蝇大脑中神经分泌细胞的突触连接组，发现利尿激素44表达细胞是主要协调枢纽，味觉输入间接，而嗅觉通路被解析。线性动力学模型显示肠神经元影响最强，下行神经元同步内分泌与运动。输出主要由corazonin细胞介导并影响产卵，结合单细胞数据揭示旁分泌互连。
source: biorxiv
selection_source: fresh_fetch
motivation: 理解神经分泌网络如何整合感觉信息调控激素释放，进而驱动行为与生理。
method: 利用成年果蝇大脑电子显微数据构建神经分泌细胞的突触连接组，结合单细胞转录组分析。
result: 发现利尿激素44细胞为协调中心，味觉输入间接，肠神经元为最强影响者，corazonin细胞输出调控产卵。
conclusion: 该连接组为解析复杂激素网络及其对动物行为的调控提供了系统框架。
---

## 摘要
激素介导器官间信号传导，对于协调多种行为和生理过程至关重要，包括睡眠与活动、摄食、生长、代谢和繁殖。昆虫的脑间部和侧部是主要枢纽，包含产生多种肽类激素的神经分泌细胞（NSC）。为了深入了解激素信号如何被调控，我们描述了成年果蝇脑中NSC的突触连接组。对提供输入给多个NSC类别的神经元的鉴定表明，表达利尿激素44的NSC是生理和行为的主要协调者。令人惊讶的是，尽管大多数NSC在食管下区（初级味觉处理中心）有树突，但外周味觉神经元向NSC的输入主要是间接的。我们还解析了不同嗅觉输入传递到NSC的通路。通过连接组信号传播的线性动力学模型，发现与其他感觉模态相比，肠道神经元是NSC活动的最强影响者。此外，我们的分析揭示了大脑下行神经元向NSC的大量输入，表明下行神经元调节内分泌和运动输出，以同步生理变化与适当行为。与NSC输入相比，NSC的突触输出稀疏且主要由corazonin NSC介导。我们证明，表达corazonin的NSC及其下游突触伙伴DNg27影响产卵。我们还通过分析单细胞转录组数据集，探索了NSC类别之间以及从NSC到外周组织的肽类激素通路的假定旁分泌互联性。我们对果蝇神经分泌网络连接组的全面表征，为理解复杂的激素网络以及它们如何协调动物行为和生理提供了一个平台。

## Abstract
Hormones mediate inter-organ signaling which is crucial in orchestrating diverse behaviors and physiological processes including sleep and activity, feeding, growth, metabolism and reproduction. The pars intercerebralis and pars lateralis in insects represent major hubs which contain neurosecretory cells (NSC) that produce various peptide hormones. To obtain insight into how hormonal signaling is regulated, we have characterized the synaptic connectome of NSC in the adult Drosophila brain. Identification of neurons providing inputs to multiple NSC classes implicate diuretic hormone 44-expressing NSC as a major coordinator of physiology and behavior. Surprisingly, despite most NSC having dendrites in the subesophageal zone (primary taste processing center), inputs from peripheral gustatory neurons to NSC are largely indirect. We also deciphered pathways via which diverse olfactory inputs are relayed to NSC. Linear dynamical modeling of signal propagation through the connectome identifies enteric neurons as the strongest influencers of NSC activity compared to other sensory modalities. Further, our analyses revealed substantial inputs from brain descending neurons to NSC, suggesting that descending neurons regulate both endocrine and motor output to synchronize physiological changes with appropriate behaviors. In contrast to NSC inputs, synaptic output from NSC is sparse and mostly mediated by corazonin NSC. We show that both corazonin-expressing NSC and their downstream synaptic partner DNg27 influence egg-laying. We additionally explore putative paracrine interconnectivity between NSC classes and peptide hormone pathways from NSC to peripheral tissues by analyzing single-cell transcriptomic datasets. Our comprehensive characterization of the Drosophila neurosecretory network connectome provides a platform to understand complex hormonal networks and how they orchestrate animal behaviors and physiology.

---

## 论文详细总结（自动生成）

# 论文详细中文总结

## 1. 核心问题与整体含义（研究动机和背景）
- **研究动机**：激素协调多种行为和生理过程（如睡眠、摄食、生长、代谢、繁殖）。昆虫的脑间部和侧部是神经分泌细胞（NSC）聚集的主要枢纽，但神经分泌网络如何被调控尚不清楚。
- **核心问题**：揭示果蝇大脑中神经分泌细胞（NSC）的突触连接组，以理解激素信号如何通过突触输入/输出网络被整合和调控。
- **整体含义**：为解析复杂激素网络及其对动物行为和生理的系统性调控提供结构性框架，有助于揭示感觉信息如何转化为内分泌信号进而驱动行为。

## 2. 方法论：核心思想、关键技术细节
- **核心思想**：利用成年果蝇大脑的高分辨率电子显微镜（EM）数据，手动和自动重建NSC及其突触伙伴的完整连接图谱，并结合单细胞转录组数据探索旁分泌互连。
- **关键技术细节**：
  - 使用成年果蝇“半脑”电子显微数据集（来自FlyEM项目）进行神经突触连接组重建。
  - 对多个NSC类别（如表达利尿激素44、corazonin、胰岛素样肽等的细胞）进行鉴定和突触伙伴追踪。
  - 构建有向加权图（突触数量作为权重），并用**线性动力学模型**模拟信号在连接组中的传播，评估不同感觉模态（味觉、嗅觉、肠道神经元等）对NSC活动的相对影响强度。
  - 结合**单细胞转录组**数据（scRNA-seq），分析NSC类别间及各NSC与外围组织的肽类激素通路，推测旁分泌互连。
  - 行为学验证：通过遗传操作（如表达corazonin的NSC及其下游伙伴DNg27）进行产卵实验。

## 3. 实验设计：数据集、基准、对比方法
- **数据集**：
  - **EM连接组数据**：成年果蝇“半脑”电子显微图像及已发布的突触连接组（FlyWire/FAFB数据集）。论文未指明具体版本号，但强调基于官方重建。
  - **单细胞转录组数据**：来自公开的果蝇脑单细胞RNA测序数据集（如Fly Cell Atlas或相关数据库），用于分析肽类受体和配体表达。
- **基准与对比**：论文中没有直接与其他方法进行定量对比，而是以构建完整的连接图谱为主要目标。对比主要体现在：将NSC输入与输出进行对比（输入丰富、输出稀疏），以及不同感觉通路的影响权重对比（线性动力学模型模拟结果）。
- **所采用的方法**：自身对比（不同NSC类别之间的输入/输出差异，不同感觉模态的影响力差异）。

## 4. 资源与算力
- **文中未明确说明**使用的GPU型号、数量、训练时长等具体算力资源。论文主要基于已有的EM数据集重建和分析，未详述计算资源。仅提及使用了连接组学工具和线性动力学模型，但未量化硬件需求。

## 5. 实验数量与充分性
- **实验数量**：
  - **连接组重建**：对多个主要NSC类别（至少包括diuretic hormone 44、corazonin、insulin-like peptide、CCAP等）进行了突触伙伴全脑追踪。
  - **线性动力学模型**：模拟了不同感觉输入（味觉、嗅觉、肠道神经元、下行神经元等）到NSC的信号传播影响，计算了相对影响力排序。
  - **行为学验证**：对corazonin NSC及其下游伙伴DNg27进行产卵实验（至少两组：遗传激活/抑制 vs 对照），并统计产卵数量。
  - **单细胞转录组分析**：分析了多个NSC类别的配体-受体表达，推测旁分泌连接。
- **实验充分性评价**：
  - **优势**：覆盖了多种NSC类别，输入/输出分析完整；行为验证支持了输出通路的功能；转录组补充了非突触通信。
  - **局限**：缺乏对其他NSC类别输出功能的直接行为验证（仅验证了corazonin通路）；线性动力学模型有简化假设（未考虑非线性、突触可塑性等）；单细胞转录组数据可能无法区分NSC亚型细微差异。总体而言，实验在结构层面较为充分，功能验证尚不完全。

## 6. 主要结论与发现
- **利尿激素44表达细胞是主要协调枢纽**：其接受最多样化的输入（与多个感觉模态相连），被视为生理和行为的中央协调者。
- **味觉输入间接**：尽管NSC树突位于食管下区（味觉初级中枢），外周味觉神经元通常通过中间神经元间接连接，而非直接突触。
- **嗅觉通路被解析**：阐明了不同嗅觉输入（触角叶、蘑菇体等）如何通过多层中继传递到NSC。
- **肠道神经元影响最强**：线性动力学模型显示，与其他感觉模态相比，肠道感觉神经元对NSC活动的影响权重最大。
- **下行神经元同步内分泌与运动**：大量来自大脑下行神经元（descending neurons）的输入投射到NSC，提示下行通路同时调控内分泌和运动输出。
- **NSC突触输出稀疏且主要由corazonin细胞介导**：多数NSC突触输出集中于corazonin NSC；验证了corazonin NSC及其下游伙伴DNg27影响产卵行为。
- **旁分泌互连**：单细胞转录组推断出NSC类别之间以及NSC与外围组织之间存在肽类旁分泌通路。

## 7. 优点
- **方法系统性**：首次在成年果蝇脑中构建完整的突触连接组，覆盖多个NSC类别，弥补了精细连接组学的空白。
- **多模态整合**：将电子显微镜连接组数据与单细胞转录组、行为学验证相结合，从结构到功能形成证据链。
- **创新模型**：线性动力学模型提供了一种可量化的方法比较不同感觉输入对内分泌网络的相对影响力，为连接组学从静态结构到动态功能推断提供了新视角。
- **开源数据**：基于公开数据集，可重复性强；结果可被其他研究者验证和扩展。

## 8. 不足与局限
- **实验覆盖不足**：仅对corazonin输出通路进行了行为验证，其他NSC（如利尿激素44、胰岛素样肽等）的功能预测未直接验证。
- **线性模型简化**：忽略突触可塑性、神经调节、非线性动态等，可能夸大某些输入的重要性或掩盖真实调控模式。
- **单细胞转录组数据分辨率和注释限制**：可能无法完全区分所有NSC亚型及其投射特异性，旁分泌预测有一定推测性。
- **EM数据的半脑限制**：仅分析半脑，可能遗漏对侧半球连接；双侧信息不对称或协调机制未被考虑。
- **未讨论昼夜节律或状态依赖性**：连接组是静态快照，而NSC活动可能随光照、内部状态变化，但文中未分析这种动态调控如何体现在连接层面上。
- **应用限制**：结论基于果蝇模型，推广到其他昆虫或脊椎动物时需谨慎。

（完）
