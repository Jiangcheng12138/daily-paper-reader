---
title: Sharp and Fast Dynamic Extraction and Tracking of Emitted Cellular Transients
title_zh: 细胞发射瞬态信号的精确快速动态提取与追踪
authors: "Niu, W., Chen, Y., Li, X., Garnero, M., Mach, S., Verbe, A., Le, M., Jousseaume, R., David, F., Cancela, J.-M., Graupner, M., Eschbach, C., Rouach, N., Jacquir, S., Galante, M., Lerasle, M., Dallerac, G."
date: 2026-04-20
pdf: "https://www.biorxiv.org/content/10.64898/2026.04.16.718018v1.full.pdf"
tags: ["query:slp-ns"]
score: 7.0
evidence: 神经科学中瞬态信号的检测与分析
tldr: 针对神经科学中荧光传感器产生的大规模、高维度复杂成像数据，研究团队开发了名为 DETECT 的通用分析流程。该工具集成了背景去噪、目标分割和多目标追踪功能，并提供易用的 Python 图形界面。经多种成像模式和生物模型验证，DETECT 为钙信号及神经递质释放的高效分析提供了低资源消耗的稳健解决方案。
source: biorxiv
selection_source: fresh_fetch
motivation: 现代神经成像技术产生的数据量巨大且时空复杂度高，传统方法难以高效准确地检测和分析微弱的细胞瞬时信号。
method: 开发了名为 DETECT 的分析流程，结合了背景去噪、目标分割和多目标追踪技术，并配备了基于 Python 的用户友好型 GUI。
result: 该工具在多种成像模式和生物模型中得到了验证，能够高效处理钙瞬变及多种神经递质的动态信号。
conclusion: DETECT 为神经科学研究提供了一个通用、高效且低资源占用的复杂成像数据分析平台。
---

## 摘要
在神经科学中，理解脑功能的神经相关性目前在很大程度上涉及对荧光传感器产生的瞬态信号进行检测和分析。诸如共聚焦显微镜、双光子显微镜以及微型显微镜（miniscopes）等成像技术，使得可视化神经活动并捕获离体和在体的动态信号成为可能。这包括通过在特定脑细胞中表达如 GCaMP 等基因编码传感器来监测钙离子（Ca2+）瞬态。此外，基于 GPCR 的神经递质传感器的出现，使得对包括谷氨酸和 GABA 在内的神经递质，以及多巴胺或去甲肾上腺素等神经调节剂的释放进行成像成为可能。然而，这些方法会产生大规模、高维度且时空复杂的动态数据集，为信号检测和分析带来了重大挑战。为了克服这些挑战，我们开发了一个名为 DETECT（细胞发射瞬态动态提取与追踪）的多功能流程，它结合了背景去噪、目标分割和多目标追踪。我们基于 Python 开发的用户友好型图形用户界面（GUI）提供了一个低资源消耗的平台，用于高效的数据分析。经多种成像模式和生物模型验证，DETECT 为神经科学研究中复杂成像数据集的分析提供了一个稳健且全面的解决方案。

## Abstract
Understanding neural correlates of brain function in neuroscience now largely involves detecting and analyzing transient signals from fluorescent sensors. Imaging technologies such as confocal and two-photon microscopy, along with onboard miniscopes, enable the visualization of neural activities and capture dynamic signals both ex vivo and in vivo. This includes monitoring Ca2+ transients via the expression of genetically encoded sensors such as GCaMP in specific brain cells. Additionally, the advent of GPCR-based neurotransmitter sensors allows for imaging the release of neurotransmitters including glutamate and GABA, as well as neuromodulators such as dopamine or noradrenaline. These approaches however generate large, high-dimensional, spatiotemporally complex datasets, presenting significant challenges for signal detection and analysis. To overcome these challenges, we developed a versatile pipeline of Dynamic Extraction and Tracking of Emitted Cellular Transients (DETECT), which combines background denoising, object segmentation, and multi-object tracking. Our user-friendly, Python-based GUI offers a low-resource platform for efficient data analysis. Validated across various imaging modalities and biological models, DETECT provides a robust and comprehensive solution for analyzing complex imaging datasets in neuroscience research.