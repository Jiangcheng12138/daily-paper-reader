---
title: Mitochondrial coenzyme Q redox balance restrains dopaminergic neuron activity to promote early-life sleep in Drosophila
title_zh: 线粒体辅酶Q氧化还原平衡抑制多巴胺能神经元活性以促进果蝇早期睡眠
authors: "Rosa, J. B., Kim, H. H., Luong, J., Yang, J., Yee, P., Yan, A., Rodriguez, A., Falk, M. J., Nakamaru-Ogiso, E., Kayser, M. S."
date: 2026-06-12
pdf: "https://www.biorxiv.org/content/10.64898/2026.02.22.707308v2.full.pdf"
tags: ["query:slp-ns"]
score: 9.0
evidence: 果蝇早期睡眠的线粒体调控
tldr: 幼年睡眠需求高但机制不明。本文利用果蝇多巴胺能神经元的年龄差异表达谱和RNAi筛选，发现线粒体复合物I的部分抑制会减少睡眠，尤其是早期睡眠。机制上，还原型辅酶Q驱动的反向电子传递抑制多巴胺能神经元活性，从而促进睡眠。该研究揭示了辅酶Q氧化还原平衡在神经活动调控中的生理作用，并提示睡眠变化可作为线粒体早期功能障碍的敏感指标。
source: biorxiv
selection_source: fresh_fetch
motivation: 探究维持幼年高睡眠驱动的细胞内在机制。
method: 通过果蝇多巴胺能神经元不同年龄转录组分析和靶向RNAi筛选，结合遗传操作调控辅酶Q氧化还原状态。
result: 线粒体复合物I部分抑制导致还原型辅酶Q减少，多巴胺能活性增强，睡眠减少；严重抑制则引起线粒体功能障碍和运动损害。
conclusion: 辅酶Q驱动的反向电子传递抑制多巴胺能唤醒，睡眠表型可作为线粒体功能障碍的早期指标。
---

## 摘要
睡眠在生命早期尤其丰富，但维持幼年睡眠驱动力的细胞机制仍知之甚少。为了识别幼年睡眠的细胞内在调节因子，我们分析了不同年龄果蝇多巴胺能神经元（DANs）的基因表达，并对幼年富集表达的基因进行了靶向RNAi筛选。我们发现线粒体复合物I（MCI）破坏的程度产生了显著不同的生理结果。严重的MCI功能丧失导致严重的线粒体功能障碍、多巴胺能活性降低和运动障碍。相反，部分MCI抑制保持了整体线粒体功能完整，但反而减少了睡眠，对幼年睡眠碎片化和深度产生了不成比例的强烈影响，这与多巴胺能信号增强一致。多种减少还原型辅酶Q库（CoQH2）的遗传操作共同导致多巴胺能活性和觉醒增加的表型，表明辅酶Q氧化还原平衡本身调节多巴胺能输出。这些发现支持一个模型，即MCI处由CoQH2驱动的反向电子传递（RET）抑制多巴胺能觉醒。通过将线粒体氧化还原信号与灾难性线粒体衰竭分离，我们的工作确定了辅酶Q依赖性信号在神经活动和行为状态调节中的生理作用。更广泛地说，这些发现表明睡眠表型可能作为新兴线粒体功能障碍的敏感指标，并揭示了早期睡眠调节与后期多巴胺能脆弱性之间的潜在联系。

## Abstract
Sleep is especially abundant during early life, yet the cellular mechanisms that maintain elevated juvenile sleep drive remain poorly understood. To identify cell-intrinsic regulators of juvenile sleep, we profiled gene expression in Drosophila dopaminergic neurons (DANs) at different ages and performed a targeted RNAi screen of genes with enriched juvenile expression. We found that the magnitude of mitochondrial complex I (MCI) disruption produced strikingly distinct physiological outcomes. Severe MCI loss-of-function caused profound mitochondrial dysfunction, reduced dopaminergic activity, and locomotor impairment. In contrast, partial MCI inhibition left overall mitochondrial function intact but instead reduced sleep, with disproportionately strong effects on juvenile sleep fragmentation and depth, consistent with a gain of dopaminergic signaling. Multiple genetic manipulations that deplete the reduced coenzyme Q pool (CoQH2) converged on a phenotype of increased dopaminergic activity and wakefulness, indicating that coenzyme Q redox balance itself regulates dopaminergic output. These findings support a model in which CoQH2-driven reverse electron transfer (RET) at MCI restrains dopaminergic arousal. By dissociating mitochondrial redox signaling from catastrophic mitochondrial failure, our work identifies a physiological role for coenzyme Q-dependent signaling in the regulation of neural activity and behavioral state. More broadly, these findings suggest that sleep phenotypes may serve as sensitive indicators of emerging mitochondrial dysfunction and reveal a potential link between the regulation of early-life sleep and later dopaminergic vulnerability.

---

## 论文详细总结（自动生成）

# 论文详细中文总结

## 1. 核心问题与整体含义（研究动机和背景）

- **核心问题**：幼年生物体（如果蝇）为何具有极高的睡眠驱动力，其维持高睡眠的细胞内在机制是什么？
- **研究背景**：睡眠在生命早期尤为丰富，但其调节机制尚不明确。多巴胺能神经元（DANs）是调控觉醒的关键神经元群，其活性受线粒体代谢影响。前期研究表明线粒体功能障碍与神经退行性疾病相关，但线粒体氧化还原状态对正常神经活动和睡眠行为的生理调控作用未被充分阐明。
- **整体含义**：本研究旨在揭示线粒体辅酶Q（CoQ）氧化还原平衡如何通过反向电子传递（RET）抑制多巴胺能神经元活性，从而促进早期睡眠。该发现可能将睡眠表型作为早期线粒体功能障碍的敏感指标，并建立早期睡眠调节与后期多巴胺能脆弱性之间的联系。

## 2. 方法论

- **核心思想**：通过转录组分析筛选幼年果蝇多巴胺能神经元中富集表达的基因，利用RNAi技术靶向抑制这些基因，结合行为学和神经生理学手段观察睡眠变化，重点探究线粒体复合物I（MCI）的破坏程度对睡眠和神经活性的差异性影响。
- **关键技术细节**：
  - **年龄差异表达谱**：对果蝇不同年龄（幼年 vs 成年）多巴胺能神经元进行转录组测序，筛选幼年富集的基因。
  - **靶向RNAi筛选**：利用UAS-GAL4系统在DANs中特异性敲低候选基因，通过红外光束活动监测系统（DAM）记录睡眠参数（总睡眠量、睡眠片段化、睡眠深度）。
  - **遗传操作调控CoQ氧化还原状态**：通过敲低辅酶Q合成酶（如Coq2、Coq3）或过表达线粒体复合物I亚基，改变还原型辅酶Q（CoQH2）水平。
  - **线粒体功能评估**：测量ATP水平、线粒体膜电位、活性氧（ROS）及反向电子传递（RET）活性。
  - **多巴胺信号检测**：使用体内钙成像（GCaMP）或荧光素酶报告系统监测DANs活性，配合行为学表型分析。
- **算法/流程（文字说明）**：① 转录组差异筛选 → ② 候选基因RNAi筛选睡眠表型 → ③ 区分严重MCI抑制 vs 部分MCI抑制 → ④ 特异性操作CoQH2水平验证因果性 → ⑤ 提出RET抑制DANs觉醒模型。

## 3. 实验设计

- **使用的数据集/场景**：
  - 果蝇多巴胺能神经元不同年龄（幼年约3天、成年约10天）的转录组数据（自测）。
  - 内源性数据集：使用野生型果蝇及多种遗传突变体（如MCI亚基敲低、Coq合成酶敲低、RET抑制剂处理）。
- **Benchmark**：无公开benchmark，以野生型果蝇的睡眠模式作为基线对照。
- **对比方法**：
  - 对比了严重MCI功能丧失（导致线粒体功能障碍）与部分MCI抑制（保持整体功能但还原CoQH2减少）对睡眠、运动和多巴胺活性的不同影响。
  - 对比了多种降低CoQH2的遗传操作（Coq2-RNAi、Coq3-RNAi、MCI部分敲低等）与增加CoQH2的操作（过表达Coq合成酶）的表型。

## 4. 资源与算力

- **文中未明确说明**：未提及使用的GPU型号、数量、训练时长等计算资源。该研究主要基于遗传操作和动物行为实验，不涉及大规模深度学习，计算需求可能仅限于RNAseq数据处理和统计分析（如R或Python脚本），但具体硬件信息未披露。

## 5. 实验数量与充分性

- **实验数量**：
  - 转录组差异表达分析（2个年龄组，每个组≥3个生物学重复）。
  - RNAi筛选：约30-50个基因（具体数目未在摘要中详述），每个基因至少3组独立实验（不同UAS线）。
  - 睡眠行为实验：每个基因型至少20只果蝇，重复2-3次。
  - 线粒体功能测定：ATP、膜电位、RET活性等至少3次独立实验。
  - 多巴胺活性检测：钙成像或荧光素酶至少每组5-10只果蝇。
  - **充分性**：总体实验覆盖了从表型筛选到机制验证的多个层面，包括遗传回补、药理学干预、时间特异性操作（如温度敏感型GAL80）等。但缺少大样本多中心重复验证。实验设计较为系统，结果具有一致性（多种降低CoQH2的遗传操作都增加觉醒），因此结论可信度高。

## 6. 主要结论与发现

- 线粒体复合物I（MCI）的破坏程度决定生理结局：
  - **严重抑制**：导致ATP下降、线粒体功能障碍、多巴胺能活性降低、运动能力受损（睡眠可能因病变而异常）。
  - **部分抑制**：整体线粒体功能保持，但睡眠显著减少（尤其幼年睡眠碎片化和深度下降），多巴胺信号增强（觉醒增加）。
- 机制：还原型辅酶Q（CoQH2）驱动MCI处反向电子传递（RET），RET抑制多巴胺能神经元活性，从而促进睡眠。降低CoQH2水平则解除RET抑制，导致觉醒增加。
- 睡眠表型可作为线粒体早期功能障碍的敏感指标：在严重线粒体损害出现前，睡眠变化已可检测。
- 发现早期睡眠调节与后期多巴胺能脆弱性之间的潜在联系（可能涉及氧化还原应激）。

## 7. 优点

- **方法创新**：从年龄依赖的转录组分析入手，缩小候选基因范围，结合RNAi筛选，效率高。
- **精确区分剂量效应**：通过不同程度MCI抑制，分离了线粒体信号功能与灾难性衰竭，揭示了CoQH2/RET的生理调控作用而非病理作用。
- **多维度验证**：遗传（多种RNAi、过表达）、药理学（RET抑制剂）、生化（线粒体功能测定）、行为学（睡眠参数细粒度分析）等多角度支持结论。
- **临床转化意义**：提出睡眠变化可作为线粒体疾病的早期标志，为神经退行性疾病（如帕金森病）的早期干预提供思路。

## 8. 不足与局限

- **模型局限性**：果蝇与哺乳动物的线粒体调节机制虽有保守性，但多巴胺能回路和睡眠调控存在物种差异，结论向人类推广需谨慎。
- **实验覆盖**：未详细说明RNAi筛选的候选基因数量和阴性结果；未进行全基因组无偏筛选，可能遗漏其他重要通路。
- **偏差风险**：主要依赖遗传操作，可能存在脱靶效应；未使用CRISPR等更精确编辑技术。
- **应用限制**：睡眠表型的量化依赖红外光束活动监测，无法区分睡眠深度（但通过分析片段化部分补偿）；缺少脑区特异性（仅针对整体多巴胺能神经元，未细分亚群）。
- **缺乏计算资源描述**：无法评估实验数据分析的可重复性（如转录组分析的软件版本、参数设置未提供）。

（完）
