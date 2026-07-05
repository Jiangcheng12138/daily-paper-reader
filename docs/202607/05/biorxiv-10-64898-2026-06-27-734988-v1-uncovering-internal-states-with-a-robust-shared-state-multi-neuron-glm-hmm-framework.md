---
title: Uncovering internal states with a robust shared-state multi-neuron GLM-HMM framework
title_zh: 利用鲁棒的共享状态多神经元GLM-HMM框架揭示内部状态
authors: "Lawrence, A., Yezerets, E., Janak, P. H., Charles, A."
date: 2026-07-02
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.27.734988v1.full.pdf"
tags: ["query:slp-ns"]
score: 6.0
evidence: 从多神经元活动推断内在状态的方法，可应用于睡眠-觉醒状态研究
tldr: 神经群体活动的稀疏性和共线性使得拟合多神经元状态模型困难。本文构建了稳健的多神经元GLM-HMM框架，通过引入神经元自适应惩罚和信任区域算法改进EM过程，克服了协变量共线性和病态Hessian问题。在三个决策任务电生理数据集上，模型稳定收敛并推断出具有行为相关性的内部状态。该框架为从稀疏群体活动中揭示内部状态提供了可靠工具。
source: biorxiv
selection_source: fresh_fetch
motivation: 现有方法难以同时建模神经活动和行为状态，且在稀疏、共线性数据上拟合不稳定。
method: 提出改进EM算法，在M步中采用神经元自适应L1惩罚和信任区域优化，稳定估计泊松GLM系数并保证收敛。
result: 在三个灵长类和啮齿类决策任务电生理数据集上实现稳定收敛，推断的状态与行为选择显著相关。
conclusion: 该框架能够可靠地从稀疏神经群体活动中提取内部状态，为理解脑状态-行为关系提供稳健方法。
---

## 摘要
神经系统表现出多种放电状态，这些状态反映了生物体的内部状态，并调节外部环境刺激与行为之间的关系。多项研究通过将非泊松行为观测的广义线性模型（GLM）补充到传统隐马尔可夫模型（HMM）中，推断出这些潜在状态。然而，理解大脑内部状态与行为之间的关系还需要对神经活动进行建模。尽管如此，由于神经元数据集的高稀疏性、共线性和低试验次数，拟合多神经元GLM-HMM并非易事。因此，我们构建了一个鲁棒的多神经元GLM-HMM框架，该框架从群体活动中揭示潜在状态，同时纳入时间戳任务变量和脉冲历史的影响。为了获得可靠的模型参数，我们采用了一种改进的期望最大化过程。具体而言，我们表明在最大化步骤中引入神经元自适应惩罚能够克服时间戳事件和稀疏放电典型的协变量共线性问题，从而得到泊松GLM系数的稳定估计。此外，我们融入了一个信赖域算法，以确保在存在病态Hessian矩阵（可能导致不稳定的Newton-Raphson更新）的情况下实现稳定的M步收敛。我们进一步展示了留一法交叉验证分析在低试验次数且不破坏时间结构的数据集上评估模型性能的实用性。我们在三个来自灵长类和啮齿类动物在执行决策任务时的电生理数据集上评估了我们的框架，展示了稳定的模型收敛性，并讨论了推断状态的行为相关性。

## Abstract
Neural systems exhibit multiple firing states that reflect an organism's internal state and modulate the relationship between external environmental stimuli and behavior. Several studies have inferred these latent states by supplementing the traditional hidden Markov Model (HMM) with generalized linear models (GLMs) with non-Poisson behavioral observations. However, understanding the relationship between internal brain states and behavior also requires modeling the neural activity. Nonetheless, fitting multi-neuron GLM-HMMs is non-trivial due to high sparsity, collinearity, and low trial counts in neuronal datasets. Therefore, we built a robust multi-neuron GLM-HMM framework that uncovers latent states from population activity while incorporating the influence of time-stamped task variables and spike histories. To obtain reliable model parameters, we employ a modified expectation-maximization procedure. Specifically, we show that incorporating neuron-adaptive penalization in the maximization step overcomes the covariate co-linearity issues typical of time-stamped events and sparse spiking, yielding stable estimates of Poisson GLM coefficients. Furthermore, we incorporate a trust-region algorithm to ensure stable M-step convergence in the presence of ill-conditioned Hessians that can lead to unstable Newton-Raphson updates. We further demonstrate the utility of leave-one-out cross-validation analysis for evaluating model performance on datasets with low trial counts and without breaking their temporal structure. We evaluate our framework on three electrophysiological datasets from primates and rodents as they perform a decision-making task, demonstrate stable model convergence, and discuss the behavioral relevance of the inferred states.