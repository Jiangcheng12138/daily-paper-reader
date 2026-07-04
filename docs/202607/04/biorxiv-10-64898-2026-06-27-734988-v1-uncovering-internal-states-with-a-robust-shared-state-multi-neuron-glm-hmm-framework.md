---
title: Uncovering internal states with a robust shared-state multi-neuron GLM-HMM framework
title_zh: 利用鲁棒的共享状态多神经元GLM-HMM框架揭示内部状态
authors: "Lawrence, A., Yezerets, E., Janak, P. H., Charles, A."
date: 2026-07-02
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.27.734988v1.full.pdf"
tags: ["query:slp-ns"]
score: 6.0
evidence: 多神经元GLM-HMM方法推断脑内隐状态，可应用于睡眠神经科学
tldr: 传统隐马尔可夫模型仅建模行为观测，无法同时利用神经活动揭示内部状态。本文提出多神经元GLM-HMM框架，在广义线性模型中融入时间戳任务变量和尖峰历史，通过神经元自适应惩罚和信赖域算法改进EM收敛。在三个灵长类和啮齿类决策任务电生理数据集上验证，模型稳定收敛，推断的状态与行为显著相关。该框架为理解内部脑状态与行为的关系提供了鲁棒工具。
source: biorxiv
selection_source: fresh_fetch
motivation: 传统HMM仅建模行为，无法整合神经活动揭示内部状态；高稀疏性和共线性使多神经元GLM-HMM拟合困难。
method: 构建多神经元GLM-HMM，采用神经元自适应惩罚处理共线性，结合信赖域算法稳定M步，并使用留一交叉验证评估低试验数数据集。
result: 在灵长类和啮齿类决策任务电生理数据上，模型稳定收敛，推断的状态具有行为相关性。
conclusion: 该框架鲁棒地从群体神经元活动推断潜在状态，促进理解内部状态与行为的关系。
---

## 摘要
神经系统中存在多种放电状态，这些状态反映了生物体的内部状态，并调节外部环境刺激与行为之间的关系。多项研究通过将传统隐马尔可夫模型与广义线性模型结合非泊松行为观测来推断这些潜在状态。然而，理解大脑内部状态与行为之间的关系还需要对神经活动进行建模。尽管如此，由于神经元数据集的高稀疏性、共线性和低试验次数，拟合多神经元GLM-HMM模型并非易事。因此，我们构建了一个鲁棒的多神经元GLM-HMM框架，该框架能够从群体活动中揭示潜在状态，同时纳入时间戳任务变量和脉冲历史的影响。为了获得可靠的模型参数，我们采用了改进的期望最大化程序。具体而言，我们展示了在最大化步骤中融入神经元自适应惩罚如何克服时间戳事件和稀疏尖峰活动典型存在的协变量共线性问题，从而得到泊松GLM系数的稳定估计。此外，我们引入了信赖域算法，以确保在病态Hessian矩阵（可能导致不稳定的Newton-Raphson更新）存在下M步的稳定收敛。我们进一步展示了留一法交叉验证分析在评估低试验次数数据集模型性能且不破坏其时序结构方面的实用性。我们基于灵长类和啮齿类动物在执行决策任务时的三个电生理数据集评估了我们的框架，展示了稳定的模型收敛性，并讨论了推断状态的行为相关性。

## Abstract
Neural systems exhibit multiple firing states that reflect an organism's internal state and modulate the relationship between external environmental stimuli and behavior. Several studies have inferred these latent states by supplementing the traditional hidden Markov Model (HMM) with generalized linear models (GLMs) with non-Poisson behavioral observations. However, understanding the relationship between internal brain states and behavior also requires modeling the neural activity. Nonetheless, fitting multi-neuron GLM-HMMs is non-trivial due to high sparsity, collinearity, and low trial counts in neuronal datasets. Therefore, we built a robust multi-neuron GLM-HMM framework that uncovers latent states from population activity while incorporating the influence of time-stamped task variables and spike histories. To obtain reliable model parameters, we employ a modified expectation-maximization procedure. Specifically, we show that incorporating neuron-adaptive penalization in the maximization step overcomes the covariate co-linearity issues typical of time-stamped events and sparse spiking, yielding stable estimates of Poisson GLM coefficients. Furthermore, we incorporate a trust-region algorithm to ensure stable M-step convergence in the presence of ill-conditioned Hessians that can lead to unstable Newton-Raphson updates. We further demonstrate the utility of leave-one-out cross-validation analysis for evaluating model performance on datasets with low trial counts and without breaking their temporal structure. We evaluate our framework on three electrophysiological datasets from primates and rodents as they perform a decision-making task, demonstrate stable model convergence, and discuss the behavioral relevance of the inferred states.