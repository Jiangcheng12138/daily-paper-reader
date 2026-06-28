---
title: A probabilistic atlas of the human thalamic reticular nucleus derived from 7T MRI
title_zh: 基于7T MRI的人类丘脑网状核概率图谱
authors: "Kotwicka, Z., Gulban, O. F., Dowdle, L., Auksztulewicz, R., Moerel, M."
date: 2026-06-26
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.22.733673v1.full.pdf"
tags: ["query:slp-ns"]
score: 9.0
evidence: 丘脑网状核图谱支持睡眠-觉醒周期研究
tldr: 丘脑网状核（TRN）是调控丘脑皮层信息流的关键结构，但因体积小、位置深，传统成像难以观测。本研究利用7T超高场MRI获取0.35mm各向同性高分图像，手动分割TRN并与高质量死后数据对比验证。结果显示活体分割的TRN体积和厚度与死后参考高度一致，形态位置个体间一致性高且捕获有意义变异。最终构建了公开的人TRN概率图谱，证明7T可稳健绘制活体TRN，为功能、结构和临床研究提供新资源。
source: biorxiv
selection_source: fresh_fetch
motivation: TRN在注意、任务切换和睡眠中起核心作用，但常规MRI难以可靠成像，需开发活体可视化方法。
method: "采用7T超高场MRI获取0.35mm各向同性T2*和T1像，手动分割TRN，并与两个高质量死后数据集进行定量比较。"
result: 活体TRN体积和厚度与死后参考高度吻合，形状位置个体间一致性高且捕获显著变异，构建了公开概率图谱。
conclusion: 7T MRI可稳健映射人TRN，概率图谱为研究其结构与功能奠定基础。
---

## 摘要
丘脑网状核（TRN）是围绕丘脑的一层薄薄的抑制性外壳。它调节丘脑皮层信息流，因此在注意力、任务切换和睡眠-觉醒周期中起核心作用。尽管其重要性，TRN在人类大脑中的研究仍然很少。这主要是因为其体积小和深层的解剖位置限制了传统非侵入性神经影像技术的可视性。在此，我们评估了能否使用7特斯拉的超高场（UHF）磁共振成像（MRI）在体内可靠地可视化并分割人类TRN。从健康个体获取高分辨率（0.35 mm各向同性）局部脑T2*和T1扫描，随后手动勾画TRN。将这些体内分割与从两个作为解剖参考的高质量死后数据集获得的TRN估计值进行比较。TRN体积和厚度的体内分割与死后参考数据集测量结果紧密匹配，定量比较显示个体间TRN形状和位置高度一致，同时也捕获了有意义的个体间变异。利用这些分割，我们构建了一个公开可用的人类TRN概率图谱。该图谱为将TRN解剖学整合到功能、结构和临床神经影像研究中提供了新资源。我们的研究结果表明，人类TRN可以在7T下稳健地进行体内映射，并为未来研究其结构和功能奠定了基础。

## Abstract
The thalamic reticular nucleus (TRN) is a thin, inhibitory shell surrounding the thalamus. It regulates the thalamocortical information flow, and thereby plays a central role in attention, task switching, and the sleep-wake cycle. Despite its importance, the TRN remains poorly studied in the human brain. This is largely because its small size and deep anatomical location limit its visibility with conventional non-invasive neuroimaging techniques. Here, we assessed whether the human TRN can be reliably visualised and segmented in vivo using ultra-high field (UHF) magnetic resonance imaging (MRI) at 7 Tesla. High resolution (0.35 mm isotropic) partial-brain T2* and T1 scans were acquired from healthy individuals, followed by manual delineation of the TRN. These in vivo segmentations were compared with TRN estimates obtained from two high-quality postmortem datasets serving as an anatomical reference. In vivo segmentations of TRN volume and thickness closely matched measurements derived from the postmortem reference datasets, and quantitative comparisons showed high consistency in TRN shape and location across individuals while also capturing meaningful inter-individual variability. Using these segmentations, we constructed a publicly available probabilistic atlas of the human TRN. This atlas provides a new resource for incorporating TRN anatomy into functional, structural, and clinical neuroimaging studies. Our findings demonstrate that the human TRN can be robustly mapped in vivo at 7T and establish a foundation for future investigations into its structure and function.

---

## 论文详细总结（自动生成）

# 基于7T MRI的人类丘脑网状核概率图谱：详细总结

## 1. 论文的核心问题与整体含义（研究动机和背景）
- **核心问题**：丘脑网状核（TRN）是围绕丘脑的薄层抑制性结构，调控丘脑皮层信息流，在注意力、任务切换和睡眠-觉醒周期中发挥核心作用。然而，由于TRN体积小、解剖位置深，传统常规MRI难以在活体中可靠可视化，导致人类TRN研究严重不足。
- **研究动机**：评估能否利用7特斯拉（7T）超高场MRI在活体中可靠地可视化并分割人类TRN，从而为后续功能、结构和临床神经影像研究提供解剖基础。
- **整体含义**：成功构建首个基于活体7T MRI的人TRN概率图谱，为研究该区域的结构和功能奠定资源基础，有望促进对注意、睡眠等认知过程的理解。

## 2. 论文提出的方法论
- **核心思想**：利用7T MRI的高空间分辨率（0.35 mm各向同性）和超高场强提供的信噪比优势，获取局部脑部的T2*和T1加权像，通过手动分割的方式描绘TRN边界，并与高质量的死后解剖参考数据集进行定量比较，验证活体分割的准确性。
- **关键技术细节**：
  - 扫描序列：高分辨率部分脑T2*和T1扫描（0.35 mm各向同性）。
  - 分割方法：手动勾画TRN（由专家依据解剖标准进行）。
  - 验证参考：使用两个独立的高质量死后数据集（获取的TRN估计值作为金标准）。
  - 比较指标：TRN体积、厚度、形状和位置的个体间一致性及个体间变异。
- **公式或算法流程**：文中未涉及公式或自动算法流程，主要依赖手动分割和定量比较。

## 3. 实验设计
- **数据集/场景**：
  - 活体数据集：来自健康个体的7T MRI扫描（具体样本量文中未明确说明）。
  - 死后参考数据集：两个高质量死后人脑数据集，提供TRN的解剖估计。
- **基准（Benchmark）**：以死后数据集的TRN分割结果作为解剖参考金标准。
- **对比方法**：将活体手动分割与死后参考的TRN体积、厚度进行直接定量比较，同时分析个体间形状和位置的一致性。未与其他自动分割方法或不同场强MRI结果对比。

## 4. 资源与算力
- **硬件资源**：论文明确使用了7特斯拉（7T）超高场MRI扫描仪获取影像数据，但未提及GPU型号、数量、训练时长等计算资源。
- **说明**：由于分割为手动操作，无需深度学习训练，因此未涉及算力投入的详细描述。文中未对计算资源做任何说明。

## 5. 实验数量与充分性
- **实验组数**：摘要中仅提及进行了活体分割与两个死后数据集的比较，未报告具体活体样本量（如多少名受试者）或重复实验次数。
- **充分性与客观性**：
  - **优点**：采用双死后数据集作为参考，提高了验证的可靠性；定量比较体积、厚度、位置一致性，指标全面。
  - **不足**：实验数量有限（单中心、小样本估计），缺乏跨扫描仪、跨场强或跨人群（如患者）的验证；手动分割依赖专家，可能存在主观偏差；未进行消融实验或方法对比（如不同分辨率、不同序列的影响）。整体而言，实验初步证明了方法的可行性，但充分性有限。

## 6. 论文的主要结论与发现
- **主要结论**：人类TRN可以在7T MRI下稳健地进行活体映射。
- **关键发现**：
  - 活体分割的TRN体积和厚度与死后参考数据集测量结果高度吻合。
  - 个体间TRN形状和位置具有高度一致性，同时捕获了有意义的个体间变异。
  - 构建了一个公开可用的人类TRN概率图谱，为后续研究提供新资源。

## 7. 优点
- **方法亮点**：
  - 首次基于7T超高场MRI实现活体人类TRN的稳健可视化，突破了传统MRI的成像限制。
  - 通过与高质量死后数据定量比较，验证了活体分割的准确性，增强了结果可信度。
  - 构建的概率图谱公开可用，可直接应用于其他功能/结构研究，具有实用价值。
  - 手动分割结合超高分辨率和对比度，提供了精细的解剖细节。

## 8. 不足与局限
- **实验覆盖**：样本量未明确，可能较小，且仅包含健康个体，缺乏对患者人群（如失眠、注意力缺陷等）的应用验证。
- **偏差风险**：手动分割存在主观性和专家依赖，可重复性未知；未与自动或半自动分割方法比较，难以评估其相对优势。
- **应用限制**：依赖7T MRI设备，普适性有限（多数研究机构仅有3T或更低场强）；扫描时间、序列参数等未充分优化，可能影响临床转化。
- **资源方面**：未提及分割的一致性检验（如组内相关系数）或跨专家分割的变异，限制了方法的客观性。
- **其他**：未讨论TRN与周围结构（如丘脑、内囊）分界的困难；未提供概率图谱的统计参数（如模板空间、配准方法等细节）。

（完）
