---
title: Video-based eye movements are linked to cortical and pupil-based arousal in human sleep
title_zh: 基于视频的眼动与人类睡眠中的皮层和瞳孔唤起相关
authors: "Carro-Dominguez, M., Oberlin, S., Oesch, T. L., Wenderoth, N., Meissner, S. N., Lustenberger, C."
date: 2026-06-12
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.10.731319v1.full.pdf"
tags: ["query:slp-ns"]
score: 9.0
evidence: 视频眼动与REM睡眠和觉醒标记物相关
tldr: 睡眠中的眼动与 arousal 波动密切相关。本研究利用红外视频眼动追踪记录17名健康成人，通过计算机视觉提取眼动参数，发现眼动速度在非快速眼动睡眠期与瞳孔大小正相关，在清醒和 REM 期与 EEG 频谱斜率相关，且不同睡眠阶段眼动差异显著。结果表明视频眼动可高保真反映皮层和皮层下 arousal，为睡眠表型与临床评估提供新工具。
source: biorxiv
selection_source: fresh_fetch
motivation: 探索视频眼动与睡眠中皮层和瞳孔 arousal 指标的耦合关系。
method: 结合多导睡眠图和红外视频眼动追踪，用计算机视觉提取眼动参数，分析其与瞳孔大小和 EEG 频谱斜率的关联。
result: 眼动参数随睡眠阶段显著变化；眼动速度在 NREM 期与瞳孔大小正相关 (R≥0.21)，在清醒和 REM 期与 EEG 斜率相关 (R≥0.11)。
conclusion: 视频眼动定量反映脑 arousal 波动，为睡眠表型提供高保真、非侵入性的评估工具。
---

## 摘要
研究目标：量化整个睡眠宏观和微观结构中的高分辨率基于视频的眼动学，并确定它们与基于瞳孔和皮层的唤醒标记的耦合。方法：我们记录了17名健康成年人的多导睡眠图，并利用基于红外视频的眼动追踪。采用计算机视觉提取眼球位置和速度，这些与瞳孔大小（皮层下唤醒标记）和EEG频谱斜率（皮层唤醒标记）相关，涉及睡眠阶段、快速眼动（REM）亚状态和K-复合波。结果：眼动学在睡眠阶段之间显著变化（p<0.001），但水平瞳孔位置除外（p=0.192）。基于视频的眼睛位置和速度足以以高于偶然水平的准确度（47%）对阶段进行分类。在非REM睡眠期间，眼动速度与瞳孔大小呈正相关（R≥0.21，p<0.001），在清醒和REM睡眠期间与频谱斜率呈正相关（R≥0.11，p<0.018）。这些相关性的强度因眼动方向而异。与紧张性REM相比，相性REM表现出更快的眼动、更大的瞳孔大小（p<0.001）和更平坦的频谱斜率（p=0.014），表明皮层下和皮层唤醒升高。K-复合波伴随着眼动速度增加（p<0.05）和更陡的频谱斜率（p≤0.010），表明尽管同时有动眼神经激活，但向睡眠保护的皮层状态短暂转变。结论：基于视频的眼动追踪显示，眼动以状态依赖的方式与全脑唤醒波动定量耦合。该方法为解决睡眠期间精细眼动动态提供了一个真实框架，为睡眠表型和临床评估提供了高保真工具。

## Abstract
Study Objectives To quantify high-resolution video-based eye kinematics across sleep macro- and microstructure and determine their coupling with pupil-based and cortical arousal markers. Methods We recorded polysomnography and utilized infrared video-based eye-tracking in 17 healthy adults. Computer vision was employed to extract eye position and speed, which were related to pupil size (subcortical arousal marker) and EEG spectral slope (cortical arousal marker) across sleep stages, rapid eye movement (REM) substates, and K-complexes. Results Eye kinematics varied significantly across sleep stages (p<0.001), except for horizontal pupil position (p=0.192). Video-based eye position and speed are sufficient to classify stages with above chance level accuracy (47%). Eye movement speed positively correlated with pupil size during non-REM sleep (R[&ge;]0.21, p<0.001) and with spectral slope during wakefulness and REM sleep (R[&ge;]0.11, p<0.018). These strengths of the correlations differ depending on the direction of the eye movement. Phasic REM exhibited faster eye movements, larger pupil size (p<0.001), and a flatter spectral slope (p=0.014) compared to tonic REM, indicating elevated subcortical and cortical arousal. K-complexes were accompanied by increased eye movement speed (p<0.05) and a steeper spectral slope (p[&le;]0.010), suggesting a transient shift toward a sleep-protective cortical state despite concurrent oculomotor activation. Conclusions Video-based eye-tracking reveals that eye movements are quantitatively coupled to brain-wide arousal fluctuations in a state-dependent manner. This methodology provides a ground-truth framework for resolving fine-grained eye dynamics during sleep, offering a high-fidelity tool for sleep phenotyping and clinical assessment.

---

## 论文详细总结（自动生成）

好的，作为一名资深学术论文分析助手，我将根据您提供的论文内容，生成一份结构化、深入且客观的中文总结。

---

### 论文分析总结

#### 1. 论文的核心问题与整体含义（研究动机和背景）

*   **核心问题**：传统用于睡眠监测的电生理信号（如眼电图，EOG）空间分辨率低，且易与脑电或肌肉活动信号混淆，无法精确区分真实的眼动。因此，睡眠中眼动与大脑内部唤醒水平（arousal）之间的精确关系尚不明确。本研究旨在探究基于视频的高精度眼动追踪能否揭示这种潜在的耦合关系。
*   **研究动机**：动物研究表明，控制唤醒水平的脑干核团与控制眼球运动的动眼神经核之间在解剖和功能上紧密相连。这暗示眼动可能是大脑内部状态变化（尤其是唤醒水平波动）的直接反映。然而，由于EOG的技术局限性，这一假设在人类研究中一直未能得到有效验证。
*   **整体含义**：本研究旨在建立一种“地面真值”方法，将眼动模式精确关联到皮层（以EEG频谱斜率为标志）和皮层下（以瞳孔大小为标志）的唤醒水平，从而为理解睡眠微结构、区分睡眠亚状态（如紧张性和相性REM睡眠）提供一个更清晰、更可靠的神经生理学框架，并为睡眠表型分析和临床评估（如帕金森病）提供新的高保真生物标记物。

#### 2. 论文提出的方法论：核心思想、关键技术细节、算法流程

*   **核心思想**：利用高分辨率红外视频眼动追踪技术，获取眼动的位置和速度等精确运动学参数，并与同时记录的皮层唤醒标记（EEG频谱斜率）和皮层下唤醒标记（瞳孔大小）进行量化关联，以揭示眼动在不同睡眠阶段和微结构事件中的神经生理学意义。
*   **关键技术细节**：
    *   **眼动追踪**：使用`Pupil Core`红外眼动追踪眼镜，以50Hz采样率获取右眼视频。
    *   **计算机视觉分析**：采用`DeepLabCut`深度学习框架，在每帧视频中标注36个标记点（12个眼睑、12个虹膜、12个瞳孔），以精确提取瞳孔位置和边界。通过几何计算确定眼动坐标系（以内外眦连线为水平轴，中点为原点）。
    *   **唤醒标记**：
        *   **皮层唤醒**：使用`FOOOF`算法从EEG信号（电极Fpz）中提取30-45Hz频段的非周期性成分（频谱斜率）。斜率越负（越陡），表示皮层唤醒水平越低。
        *   **皮层下唤醒**：计算瞳孔与虹膜的半径比作为瞳孔大小，该指标与蓝斑-去甲肾上腺素系统等皮层下唤醒系统密切相关。
*   **算法流程（文字说明）**：
    1.  **数据采集**：同步记录PSG（EEG, EOG, EMG等）和红外视频眼动数据。
    2.  **预处理**：对PSG数据进行滤波、降采样、人工判读睡眠分期；对眼动视频进行降采样、标记提取、插值对齐。
    3.  **眼动参数提取**：计算30秒时间窗内的平均水平和垂直瞳孔位置、水平和垂直眼动速度以及矢量速度（速率）。
    4.  **唤醒标记提取**：计算同时间窗内的瞳孔大小和EEG频谱斜率。
    5.  **统计分析**：
        *   利用线性混合效应模型比较不同睡眠阶段/微结构事件（如REM亚状态）的眼动参数差异。
        *   利用重复测量相关分析计算眼动速度与瞳孔大小/频谱斜率之间的相关性。
        *   使用随机森林分类器评估眼动参数单独或结合瞳孔大小进行睡眠分期的能力，并用SHAP分析评估各特征的重要性。
        *   基于速度阈值（>0.4 a.u./s为相性，<0.2 a.u./s为紧张性）和EOG幅度阈值（<25μV）自动划分REM睡眠的紧张性和相性亚状态。
        *   通过视觉检测，识别出同步出现在额叶（Fpz）和中央（Cz）电极的K-复合波。

#### 3. 实验设计：数据集、基准、对比方法

*   **数据集**：17名健康成年人（最终16名纳入分析）的夜间睡眠数据，包括多导睡眠图（PSG）和同步的红外视频眼动追踪记录。
*   **基准（任务）**：本研究并非旨在与现有方法进行性能竞赛，而是提供一套全新的、高保真的“地面真值”数据。但作为验证，他们执行了以下任务：
    *   **睡眠分期任务**：利用眼动参数（水平/垂直位置和速度）作为特征，训练随机森林分类器对W, N1, N2, N3, REM这5个睡眠阶段进行分类。使用总体准确率（47%）和F1分数（0.46）评估，并与随机水平（20%）进行对比。
    *   **对比与验证**：分类结果验证了眼动参数在不同睡眠阶段具有区分性。同时，结合瞳孔大小后准确率提升至66%，证明了睡眠阶段分类可以融合多模态耦合的生理信号。
*   **方法对比**：本研究未直接与其他眼动分析方法（如纯EOG分析）进行定量对比或benchmark测试。其核心价值在于提出并验证了一种比EOG更精确、更可靠的新方法学框架。

#### 4. 资源与算力

*   **未明确说明**：文中没有提及训练深度学习模型（DeepLabCut或随机森林分类器）所使用的具体GPU型号、数量或训练时长。仅指出使用Python 3.8、DeepLabCut 2.2、MATLAB R2019a等软件环境。

#### 5. 实验数量与充分性

*   **实验数量**：论文进行了一系列分析实验，覆盖了睡眠宏结构（5个睡眠阶段）、微结构（REM亚状态、K-复合波）以及眼动与两个唤醒标记（瞳孔大小、频谱斜率）之间的相关性。关键分析包括：
    *   各睡眠阶段眼动参数的组间比较（图2）。
    *   跨睡眠阶段和同睡眠阶段内眼动速度与唤醒标记的相关性（图3）。
    *   紧张性与相性REM亚状态的唤醒水平比较（图4）。
    *   K-复合波前后眼动和频谱斜率的变化（图5）。
    *   睡眠分期分类与特征重要性分析（图2C，补充图1）。
*   **充分性与公平性**：
    *   **优点**：研究设计层次分明，从宏观到微观，系统性地探讨了眼动与唤醒的耦合关系，实验内容丰富。使用线性混合效应模型和重复测量相关分析处理重复测量数据，统计学方法恰当。
    *   **不足**：
        *   **样本量较小**：最终纳入分析的仅16人，限制了统计效力和结果的普适性，尤其对于N1和N3等数据量较少的睡眠阶段，分析结果可能不稳定。
        *   **分析窗口不均**：不同睡眠阶段的数据量差异很大（例如N2睡眠通常远多于N1和N3），这可能导致分类模型存在“多数类偏差”。
        *   **自变量复杂性**：实验操作（如用胶带撑开眼睑、注射维生素A药膏）可能对正常的眼动和瞳孔动力学产生未知影响，这是实验设计中一个潜在的人为因素混淆。

#### 6. 论文的主要结论与发现

*   **眼动参数随睡眠阶段动态变化**：基于视频的眼动速度和垂直位置在睡眠阶段之间表现出显著差异，足以以47%的准确率（远高于随机水平）进行睡眠分期，且垂直眼位对识别REM睡眠最关键，而眼动速度对识别NREM和清醒最重要。
*   **眼动与唤醒水平的耦合状态依赖**：
    *   在NREM睡眠期间，眼动速度与**瞳孔大小**（皮层下唤醒）正相关最强。
    *   在清醒和REM睡眠期间，眼动速度与**EEG频谱斜率**（皮层唤醒）正相关最强。相关性强度还取决于眼动的方向（水平vs.垂直）。
*   **精确描绘REM亚状态**：利用视频眼动的高时间分辨率，证实了**相性REM睡眠**相较于**紧张性REM睡眠**，表现出更快的眼动速度、更大的瞳孔大小和更平坦的EEG频谱斜率，提示其皮层下和皮层唤醒水平均更高。
*   **K-复合波伴随矛盾现象**：K-复合波的发生伴随着眼动速度的增加（提示动眼激活），但同时伴随着更陡的EEG频谱斜率，即皮层唤醒下降。这表明K-复合波可能是一个**向“睡眠保护性”皮层状态的短暂转变**，尽管同时存在眼动激活。

#### 7. 优点（方法论与实验设计）

*   **方法论创新性高**：首次将高分辨率视频眼动追踪技术用于量化睡眠全过程的眼动力学，相比于传统EOG，提供了无混叠、高时空分辨率的“地面真值”数据。
*   **多模态表征**：巧妙地整合了眼动、瞳孔和EEG三个互补指标，分别从动眼、皮层下和皮层三个层面全面表征脑的唤醒状态，提供了更丰富的神经生理学视角。
*   **跨宏微观分析**：研究不仅分析了宏观的睡眠阶段，还深入到微观结构事件（REM亚状态、K-复合波），展示了对睡眠神经生理学的精细理解能力。
*   **机器学习增强解释**：通过随机森林分类和SHAP分析，量化了不同眼动特征在睡眠分类中的具体贡献，增强了结果的解释性和可操作性。

#### 8. 不足与局限

*   **样本量和普适性**：样本量小（n=16），且为健康年轻成人，限制了结果向老年人、病人或特殊人群的推广。
*   **技术局限**：50Hz的眼动采样率较低，无法捕捉精细的眼跳动力学特征（如微眼跳）。人工撑开眼睑和涂抹药膏的操作本身可能影响睡眠质量和眼球正常生理，引入未知偏差。
*   **分析偏差**：睡眠分期模型对N2阶段存在分类偏差，容易将其他阶段误判为N2。相关性分析中，N1和N3阶段的数据点可能相对较少。
*   **因果性不明**：研究发现了眼动与唤醒之间的相关性，但无法确定其因果关系。是唤醒水平的波动驱动了眼动，还是眼动导致了下游的唤醒变化，尚需因果推断实验。
*   **研究情境限制**：睡眠环境是非自然状态的（固定头部、佩戴眼罩和耳机），且有声音刺激（未被分析的时间窗口），结论在自然睡眠情境下的可推广性有限。

（完）
