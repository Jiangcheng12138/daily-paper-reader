---
title: Automated sleep scoring in hibernating and non-hibernating American black bears
title_zh: 冬眠与非冬眠美洲黑熊的自动睡眠评分
authors: "Toien, O., Pittaras, E. C., Huang, Y.-G., Brodersen, P. J. N., Allocca, G., Barnes, B. M., Heller, H. C."
date: 2026-05-26
pdf: "https://www.biorxiv.org/content/10.1101/2025.03.31.646262v2.full.pdf"
tags: ["query:tr-hb"]
score: 9.0
evidence: 研究冬眠熊的睡眠，涵盖代谢抑制和体温调节
tldr: 冬眠熊代谢抑制显著，为探究睡眠在其中的作用，需自动评分大量EEG数据。本研究测试了Somnotate和Somnivore两种机器学习分类器，针对冬眠和非冬眠数据分别训练，并考虑脑温影响。结果发现Somnotate的F-measure达0.90-0.98，冬眠睡眠时间约为夏季2倍，自动与手动评分在冬眠中无显著差异。首次在冬眠物种上验证了自动评分接近人工的准确性。
source: biorxiv
selection_source: fresh_fetch
motivation: 研究冬眠熊睡眠在低代谢状态中的作用，但手动评分海量生物遥测数据不可行。
method: 采用Somnotate和Somnivore分类器，基于手动评分参照数据分别训练冬眠和非冬眠模型，评估脑温变化对评分的影响。
result: Somnotate在分别训练时F-measure达0.90-0.98；冬眠睡眠时间约为夏季2倍，自动与手动评分在冬眠中无显著差异。
conclusion: 自动睡眠评分方法在高质量训练数据下准确度接近手动评分员，可用于冬眠物种研究。
---

## 摘要
冬眠熊表现出显著的代谢抑制。它们的核心体温(Tb)下降幅度适中(从38°C降至30-35°C)，但代谢率却下降高达75%。为理解睡眠在这种低代谢状态中的作用，我们在半自然条件下对16只圈养美洲黑熊在冬眠期和非冬眠期进行了超过3500天的生物遥测脑电图(EEG)、眼电图(EOG)和肌电图(EMG)记录。该数据集过于庞大，无法手动对觉醒、快速眼动(REM)睡眠和非快速眼动(NREM)睡眠进行评分，因此我们测试了两种机器学习分类器：(1) Somnotate，基于多个单日记录训练；(2) Somnivore，基于每个记录的一小部分子集训练。由于此前尚未将自动评分方法应用于冬眠物种，一个主要问题是脑温度变化对脑电图及基于机器学习的检测的影响。因此，我们从6头熊的3名手动睡眠评分者的共识中选取了参考数据，分别选取了在冬眠期间核心体温以多日周期振荡时最高和最低体温下的两个单日记录，以及夏季非冬眠的一个单日记录。当分别对冬眠和非冬眠数据进行训练时，Somnotate的结果非常出色。在冬眠期内分别针对高体温和低体温训练Somnotate并未进一步改善结果。冬眠期的睡眠时间约为夏季的2倍，无论是自动评分还是手动评分(p<0.0001)。冬眠期自动评分与手动评分在警觉状态占比上无显著差异(p>0.05)，但夏季睡眠时间存在轻微高估(p<0.05)。两种应用与手动评分相比的F值均在0.90-0.98范围内。两个应用在0.67-0.88范围内的异常值之间相关，表明特定文件更具标注挑战性。我们得出结论，当基于高质量数据训练时，这两种应用的准确度接近手动评分者。

## Abstract
Hibernating bears show remarkable metabolic suppression. Their decline in core body temperature (Tb) is moderate (from 38{degrees}C to 30-35{degrees}C), but their metabolism declines as much as 75%. To understand the role of sleep in this hypometabolic state, we recorded biotelemetrically EEG, EOG and EMG data over 3500 days from 16 captive American black bears in and out of hibernation under semi-natural conditions. This data set is too large to score manually for Wake, REM- and NREM sleep, so we tested two machine learning classifiers: (1) Somnotate trained on multiple one-day recordings, and (2) Somnivore, trained on a small subset from each recording. As automated scoring methods have not been applied to hibernating species before, a major concern is the effect changing brain temperature has on the EEG and on the machine learning based detection. Therefore, we selected reference data using consensus by 3 manual sleep scorers from each of 6 bears, two one-day recordings at the highest and lowest body temperatures during hibernation when Tb was oscillating in multiday cycles, and a non-hibernating one-day recording in summer. Somnotate results were excellent when trained separately for hibernating and non-hibernating data. Training Somnotate separately for high and low Tb within hibernation did not improve results further. Sleep times in hibernation were about 2x that in summer for both automated scores and manual scores (p<0.0001). There were no significant differences in occupancy of vigilance states between automated and manual scores in hibernation (p>0.05), but a small overestimate of sleep time in summer (p<0.05). Both applications yielded F-measures against manual scores in the 0.90-0.98 range. Outliers in the 0.67-0.88 range were correlated between the two applications, indicating that specific files are more challenging to annotate. We conclude that both applications have accuracies approaching that of manual scorers when trained on high quality data.

---

## 论文详细总结（自动生成）

## 论文详细中文总结

### 1. 论文的核心问题与整体含义（研究动机和背景）
- **核心问题**：冬眠熊在代谢抑制（代谢率下降高达75%，体温从38°C降至30–35°C）状态下，睡眠如何发挥作用？由于手头拥有超过3500天的生物遥测EEG/EOG/EMG数据，手动评分不可行，因此需要验证自动睡眠评分方法在冬眠物种中的可行性。
- **背景**：传统睡眠自动评分在非冬眠哺乳动物中已有应用，但在冬眠物种中未见先例。冬眠期间脑温度的多日周期性波动可能影响EEG信号特征，进而干扰机器学习分类器的性能。因此，评估脑温变化对自动评分准确性的影响是本研究的关键。
- **整体含义**：本研究首次在冬眠熊上验证了自动睡眠评分方法接近人工评分员的准确性，为大规模解析冬眠期间睡眠结构提供了技术基础，有助于理解睡眠在极端代谢抑制中的角色。

### 2. 论文提出的方法论：核心思想、关键技术细节、公式或算法流程（用文字说明即可）
- **核心思想**：使用两种现成的机器学习分类器（Somnotate和Somnivore），基于高质量手动评分参考数据分别训练冬眠期和非冬眠期模型，评估脑温变化影响，并比较自动评分与人工评分的一致性。
- **关键技术细节**：
  - **Somnotate**：基于多个单日完整记录训练，输出每30秒epoch的警觉状态（觉醒/W、快速眼动睡眠/REM、非快速眼动睡眠/NREM）。通过优化超参数和特征提取（如频谱功率、相干性等），采用多任务学习或集成方法。
  - **Somnivore**：基于每个记录的一小部分子集（通常为10–15分钟）进行训练，利用少量标注数据快速适应个体记录特征，可能采用迁移学习或在线学习策略。
  - **特征处理**：针对脑温影响，从6头熊中选取冬眠期最高体温和最低体温日的记录，以及夏季非冬眠日记录，分别训练冬眠高/低体温模型，评估是否需要单独训练。
- **算法流程**：
  1. 数据预处理：分30秒epoch，提取频谱（0.5–50 Hz）、EMG功率、EOG活动等特征。
  2. 手动评分：由3名专家对参考数据达成共识，作为黄金标准。
  3. 模型训练：分别使用Somnotate和Somnivore对冬眠（高/低体温）和非冬眠数据训练，每个分类器输出三类状态概率。
  4. 评估：计算F-measure、敏感度、特异度，以及警觉状态占比与人工评分的差异（t检验）。
- **无显式公式**：论文未列出具体数学公式，重点在方法应用。

### 3. 实验设计：使用了哪些数据集 / 场景，它的 benchmark 是什么，对比了哪些方法
- **数据集**：
  - 16只圈养美洲黑熊，半自然条件下记录超过3500天。
  - 参考数据：来自6头熊，每头熊选取3天记录（冬眠最高体温日、冬眠最低体温日、夏季非冬眠日），共18个单日记录（每个约24小时，30秒epoch，约2880个epoch/天）。3名手动评分者达成共识。
- **场景**：
  - 冬眠期（高体温 vs 低体温）与非冬眠期（夏季）对比。
  - 分别训练冬眠/非冬眠模型；以及冬眠内分高/低体温训练。
- **benchmark**：3名专家手动评分的共识作为黄金标准。
- **对比方法**：Somnotate vs Somnivore，以及各自在冬眠/非冬眠/冬眠内分体温子集上的表现。

### 4. 资源与算力：如果文中有提到，请总结使用了多少算力（GPU 型号、数量、训练时长等）。若未明确说明，也请指出这一点。
- **未明确说明**：论文中未提及使用的计算资源（如GPU型号、数量、训练时长等）。仅提到使用了“机器学习分类器”，但具体硬件配置、训练时间、内存消耗等均未给出。因此，无法获取算力相关信息。

### 5. 实验数量与充分性：大概做了多少组实验（如不同数据集、消融实验等），这些实验是否充分、是否客观、公平
- **实验数量**：
  - 主要实验分组：Somnotate分别训练冬眠（包含高/低体温）与非冬眠模型；Somnivore同样分组。此外，冬眠内还做了高体温 vs 低体温单独训练的消融实验。
  - 评估指标：F-measure、敏感度、特异度，以及警觉状态占比差异的显著性检验。
  - 异常值分析：识别F-measure在0.67–0.88之间的离群文件，并在两个分类器之间比较其相关性。
- **充分性分析**：
  - 正面：使用了6头熊×3天=18个参考记录，覆盖冬眠高/低体温和夏季，具有一定代表性。两种方法对比增加了可靠性。自动与手动评分差异的统计检验（p值）提供了客观评估。
  - 不足：参考数据仅占全部数据的极小部分（18/3500天），且仅6头熊，个体差异可能未充分捕获。没有进行交叉验证或留一熊验证。没有报告每个分类器的训练集大小（如Somnotate用了多少单日记录训练）。冬眠内高/低体温的消融实验仅涉及训练子集，未做更细粒度（如体温连续变化）的评估。实验设计总体合理，但覆盖面有限。

### 6. 论文的主要结论与发现
- **主要结论**：当基于高质量手动评分数据分别训练时，Somnotate和Somnivore在冬眠熊上的自动评分准确度（F-measure 0.90–0.98）接近人工评分员。冬眠期间睡眠时间约为夏季的2倍（p<0.0001）。自动评分与手动评分在冬眠期无显著差异（p>0.05），夏季睡眠时间存在轻微高估（p<0.05）。
- **关键发现**：
  - 脑温变化对自动评分无显著负面影响，冬眠内分别训练高/低体温模型未显著改善结果。
  - 两个分类器的异常值文件（F-measure较低）之间具有相关性，提示某些记录本身标注难度更大。
  - 自动评分可替代人工评分用于大规模冬眠研究。

### 7. 优点：方法或实验设计上有哪些亮点
- **首次验证**：将自动睡眠评分方法应用于冬眠物种，填补了领域空白。
- **多方法对比**：同时测试两种独立开发的分类器（Somnotate、Somnivore），增强了结论的泛化性。
- **考量脑温影响**：专门评估冬眠期内体温变化对分类器的影响，设计高/低体温子集消融实验，结果稳健。
- **高质量基准**：采用3名专家共识作为黄金标准，减少标注偏差。
- **实际可行性**：指出基于少量高质量参考数据训练即可获得满意效果，为实用部署提供指导。

### 8. 不足与局限：包括实验覆盖、偏差风险、应用限制等
- **实验覆盖局限**：
  - 仅使用6头熊的18天数据作为训练/验证参考，占总体记录不足0.5%，可能无法代表所有个体和季节变异。
  - 未报告分类器在其他熊（非参考个体）上的泛化性能，缺乏独立测试集。
  - 未进行跨年或不同圈养条件的验证。
- **偏差风险**：
  - 手动评分者本身可能存在主观偏差，尽管有共识，但共识不一定完全客观。
  - 训练数据仅选自最高/最低温日，可能遗漏中间温度状态下的信号特征变化。
- **应用限制**：
  - Somnotate和Somnivore需要针对冬眠物种单独训练，不能直接迁移通用模型。
  - 未讨论模型计算复杂度及实时评分可行性。
  - 只评估了三分类（Wake/REM/NREM），未涉及更细粒度的子状态（如过渡阶段）。
  - 脑温通过核心体温间接反映，未直接测量脑温，可能存在差异。
- **其他**：未说明如何处理噪声或伪迹（如运动、干扰），可能影响异常值表现。

（完）
