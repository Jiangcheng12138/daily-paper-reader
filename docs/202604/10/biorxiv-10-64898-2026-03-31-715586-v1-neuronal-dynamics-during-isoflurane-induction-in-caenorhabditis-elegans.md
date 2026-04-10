---
title: Neuronal Dynamics During Isoflurane Induction in Caenorhabditis elegans
title_zh: 秀丽隐杆线虫异氟烷诱导过程中的神经动力学
authors: "White, H., Bosinski, C., Gabel, C. V., Connor, C."
date: 2026-04-02
pdf: "https://www.biorxiv.org/content/10.64898/2026.03.31.715586v1.full.pdf"
tags: ["query:slp-ns"]
score: 8.0
evidence: 从清醒到麻醉过渡期间的神经元动态
tldr: 本研究探讨了秀丽隐杆线虫在异氟醚诱导麻醉过程中神经元动态的变化。研究人员利用光片显微镜对表达GCaMP6s的线虫进行了全脑单细胞成像，并分析了神经元集群活动及信息流指标。结果表明，麻醉诱导导致神经活动逐渐减少，且伴随着神经元间的断连与失序。该过程在动力学上是苏醒过程的逆过程，但速度更快且个体差异显著，为理解麻醉诱导的系统级机制提供了新见解。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-03-31-715586-v1/fig-001.webp\", \"caption\": \"Figure 1: Tracking of Caenorhabditis elegans neuronal activity and computing functional information flow metrics. Diagrams in F and G correspond with definitions in Chang et al (2023).\", \"page\": 24, \"index\": 1, \"width\": 928, \"height\": 656}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-03-31-715586-v1/fig-002.webp\", \"caption\": \"Figure 5: Time-course evolution of entropy parameters for individual animals and a summary metric of system disconnection. Where applicable, the dotted line indicates t = 30 minutes, a major transition point in activity state.\", \"page\": 25, \"index\": 2, \"width\": 920, \"height\": 221}]"
motivation: 旨在探究动物从清醒状态进入全身麻醉状态时，单细胞水平的神经元动态和系统连接性如何演变。
method: 采用光片显微镜对秀丽隐杆线虫进行全脑神经元成像，并利用频谱分析和信息流指标评估异氟醚诱导过程中的神经活动。
result: 异氟醚诱导导致神经活动在40分钟内逐渐减弱，表现为全频段信号功率下降以及神经元间信息流的断连，且诱导动力学呈现出苏醒过程的逆向特征。
conclusion: 麻醉诱导本质上是神经系统逐渐失序和断连的过程，其动力学特征与苏醒过程互为镜像，但在速度和个体反应上具有显著差异。
---

## 摘要
背景：当动物从清醒状态过渡到全身麻醉状态时，神经活动是如何变化的？以往的研究利用秀丽隐杆线虫探讨了清醒和麻醉状态、麻醉苏醒过程，并建立了表征这些条件下全系统神经动力学差异的指标。本研究采用一种新技术，在异氟烷诱导麻醉期间连续成像秀丽隐杆线虫的全神经元活动。

方法：通过光片显微镜对表达全神经元核定位 RFP 和胞质 GCaMP6s 的秀丽隐杆线虫进行成像，以测量异氟烷暴露诱导期间动物头部大部分神经元的单细胞活动。通过将测量流量的异氟烷蒸气通入与成像系统兼容的特制气体密封腔室，在整个实验过程中保持稳定的异氟烷浓度。在以往研究麻醉苏醒工作的基础上，我们分析了集群神经活动、频率随时间变化的光谱图以及神经元间信息流的指标。

结果：异氟烷麻醉诱导导致神经活动在 40 分钟内逐渐减少。光谱图显示所有频率的整体信号功率均有所下降，尤其是在低频段。状态解耦（State Decoupling）和内部可预测性（Internal Predictability）是区分麻醉状态最有效的指标，证明了诱导动力学是苏醒过程的逆过程。然而，每只动物进入麻醉状态的时间并不相同；反应时间具有高度的个体差异性。

结论：神经动力学活动的信息指标表明，异氟烷诱导导致神经元连接断开和无序化程度逐渐增加。因此，在单个神经元连接和系统动力学层面，秀丽隐杆线虫的麻醉诱导本质上是苏醒的逆过程。然而，诱导发生得更快，并表现出显著的个体间差异。未来的遗传学研究将揭示哪些分子靶点决定了对异氟烷等挥发性麻醉剂的敏感性。

总结陈述：异氟烷诱导的意识丧失是跨物种的普遍现象。当在单个神经元层面测量活动时，麻醉诱导是通过明显的决策状态转换产生的，还是通过系统动力学的逐渐变化产生的？

## Abstract
BackgroundHow does neuronal activity change as an animal transitions from being awake to a state of general anesthesia? Previous studies used C. elegans to investigate awake and anesthetized states, emergence from anesthesia, and to establish metrics characterizing how system-wide neuronal dynamics differ under these conditions. This study employs a new technique to image pan-neuronal activity in C. elegans continuously during induction of anesthesia with isoflurane.

MethodsC. elegans worms expressing pan-neuronal nuclear RFP and cytosolic GCaMP6s were imaged with light sheet microscopy to measure single cell activity in the majority of neurons in the animals head during induction via isoflurane exposure. Stable concentrations of isoflurane were maintained throughout the experiment by measured flow vaporization of isoflurane into a specially designed gas enclosure compatible with the imaging system. Building on our previous work investigating emergence from anesthesia, we analyzed ensemble neuronal activity, spectrograms of frequency over time, and metrics of information flow between neurons.

ResultsInduction of isoflurane anesthesia caused a progressive reduction in neuronal activity over the course of 40 minutes. Spectrograms indicated a loss of bulk signal power across all frequencies, notably in low frequencies too. State Decoupling and Internal Predictability were among the most useful metrics for discriminating the anesthetized state, demonstrating induction kinetics that are the inverse of emergence. However, each animal does not arrive at the anesthetized state at the same time; response times are highly individualized.

ConclusionsInformation metrics of neurodynamic activity demonstrate that isoflurane induction results in a gradual increase in neuronal disconnection and disorganization. Thus, at the level of individual neuron connectivity and system dynamics, the induction of anesthesia in C. elegans nematodes is in essence the reverse of emergence. Induction however occurs more rapidly and shows marked variability between individuals. Future genetic studies will show which molecular targets define sensitivity to volatile anesthetics like isoflurane.

Summary StatementIsoflurane-induced unconsciousness is a common phenomenon across species. Does the induction of anesthesia arise by distinct state transitions, or through gradual changes in system dynamics when activity is measured at the level of individual neurons?