---
title: Quantum machine learning for detection of sleep deprivation from EEG signals
title_zh: 基于EEG信号的睡眠剥夺检测的量子机器学习
authors: "Sarma-Sarkar, P., Saini, R., Roy, P. P."
date: 2026-06-18
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.14.732153v1.full.pdf"
tags: ["query:slp-ns"]
score: 7.0
evidence: 利用量子机器学习从脑电图信号检测睡眠剥夺
tldr: "睡眠剥夺影响半数印度人口，基于EEG的自动检测具有临床价值。本研究采用量子支持向量机（QSVM）和混合量子神经网络（HQNN）对静息态EEG信号进行分类，提取频谱功率、Hjorth参数及功能连接特征并编码为量子态。HQNN在epoch级和subject级评估中分别达到96.88%和81.25%的准确率，超越以往方法。结果证实量子机器学习在生物医学应用中具有竞争力。"
source: biorxiv
selection_source: fresh_fetch
motivation: 睡眠剥夺严重损害认知与健康，EEG可客观反映神经变化，但传统机器学习方法性能有限，亟需更高效的检测模型。
method: 从EEG提取频谱带功率、带比、Hjorth参数及功能连接特征，编码为量子态构建量子核；采用QSVM和HQNN进行分类，评估epoch级与subject级性能。
result: "HQNN在epoch级取得96.88%准确率，subject级81.25%；QSVM分别达到93.75%和75.00%，均优于此前报道的最佳结果。"
conclusion: 量子机器学习能有效提升EEG睡眠剥夺检测的准确性，为实际应用提供新途径。
---

## 摘要
据估计，印度约有50%的人口存在睡眠相关障碍。睡眠剥夺是一种普遍存在的状况，会对认知能力、神经功能和整体健康产生不利影响。脑电图（EEG）提供了一种客观捕捉与睡眠缺失相关神经变化的方法，因此非常适合用于自动化检测框架。在本研究中，我们探索了应用量子支持向量机和混合量子神经网络，利用静息态EEG信号对睡眠剥夺状态和休息良好状态进行分类。

我们采用了一个综合性的特征提取流程，包括谱带功率、波段比、Hjorth参数以及功能连接性度量。这些特征随后被编码为量子态以构建量子核，进而用于分类。模型性能在epoch级和subject级数据划分方案下进行评估。

混合量子神经网络（HQNN）在两种评估设置下均达到最高性能，在epoch级准确率为96.88%，在subject级准确率为81.25%。QSVM模型在epoch级和subject级评估中分别达到93.75%和75.00%的准确率。在subject级和epoch级评估中，HQNN优于先前报道的结果（68.23%和95.72%）。总体而言，这些发现凸显了量子机器学习作为基于EEG的睡眠剥夺检测的一种有竞争力方法的潜力，对实际生物医学应用具有前景。

## Abstract
Approximately 50% of the population in India is estimated to experience sleep-related disorders. Sleep deprivation is a prevalent condition that adversely impacts cognitive performance, neural functioning, and overall health. Electroencephalography (EEG) offers an objective means of capturing neural alterations associated with sleep loss, making it well-suited for automated detection frameworks. In this study, we explore the application of a Quantum Support Vector Machine and Hybrid Quantum Neural Networks to classify sleep-deprived and well-rested states using resting-state EEG signals.

A comprehensive feature extraction pipeline is employed, incorporating spectral band power, band ratios, Hjorth parameters, and functional connectivity measures. These features are subsequently encoded into quantum states to construct a quantum kernel, which is then utilized for classification. Model performance is evaluated under both epoch-level and subject-level data partitioning schemes.

The Hybrid Quantum Neural Network (HQNN) achieves the highest performance across both evaluation settings, attaining an accuracy of 96.88% at the epoch level and 81.25% at the subject level. The QSVM model achieves accuracies of 93.75% and 75.00% for epoch-level and subject-level evaluations, respectively. At subject-level and epoch -level evaluation, HQNN outperforms previously reported results (68.23% and 95.72%). Overall, these findings highlight the potential of quantum machine learning as a competitive approach for EEG-based sleep deprivation detection, with promising implications for real-world biomedical applications.