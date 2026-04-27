---
title: Sharp and Fast Dynamic Extraction and Tracking of Emitted Cellular Transients
title_zh: 细胞发射瞬变信号的精确快速动态提取与追踪
authors: "Niu, W., Chen, Y., Li, X., Garnero, M., Mach, S., Verbe, A., Le, M., Jousseaume, R., David, F., Cancela, J.-M., Graupner, M., Eschbach, C., Rouach, N., Jacquir, S., Galante, M., Lerasle, M., Dallerac, G."
date: 2026-04-20
pdf: "https://www.biorxiv.org/content/10.64898/2026.04.16.718018v1.full.pdf"
tags: ["query:slp-ns"]
score: 7.0
evidence: 追踪细胞瞬态以理解大脑功能的神经相关性
tldr: 针对神经科学中荧光成像数据（如钙信号和神经递质释放）处理复杂、维度高的难题，研究团队开发了 DETECT 管道。该工具集成了背景去噪、目标分割和多目标跟踪技术，并提供基于 Python 的低资源消耗 GUI。DETECT 能够高效、精准地从多种成像模态中提取动态信号，为复杂神经活动分析提供了稳健的自动化解决方案。
source: biorxiv
selection_source: fresh_fetch
motivation: 神经科学研究中荧光传感器产生的海量高维时空复杂数据给信号检测与分析带来了巨大挑战。
method: 开发了名为 DETECT 的 Python 管道，集成了背景去噪、目标分割和多目标跟踪功能，并提供易用的图形界面。
result: 该工具在多种成像模式和生物模型中得到了验证，能够高效处理钙信号及神经递质释放等复杂数据集。
conclusion: DETECT 为神经科学研究提供了一个稳健、全面且低资源消耗的动态细胞瞬态信号分析解决方案。
---

## 摘要
在神经科学中，理解脑功能的神经相关性目前在很大程度上涉及对荧光传感器瞬变信号的检测和分析。共聚焦和双光子显微镜等成像技术，以及车载微型显微镜（miniscopes），能够实现神经活动的视觉化，并捕获离体和在体的动态信号。这包括通过在特定脑细胞中表达 GCaMP 等基因编码传感器来监测 Ca2+ 瞬变。此外，基于 GPCR 的神经递质传感器的出现，使得对包括谷氨酸和 GABA 在内的神经递质，以及多巴胺或去甲肾上腺素等神经调节剂的释放进行成像成为可能。然而，这些方法会产生大规模、高维度且时空复杂的动态数据集，给信号检测和分析带来了重大挑战。为了克服这些挑战，我们开发了一套名为 DETECT（细胞发射瞬变信号动态提取与追踪）的多功能流水线，它结合了背景去噪、目标分割和多目标追踪。我们基于 Python 开发的图形用户界面（GUI）易于使用，为高效的数据分析提供了一个低资源消耗的平台。经多种成像模式和生物模型验证，DETECT 为神经科学研究中复杂成像数据集的分析提供了一个稳健且全面的解决方案。

## Abstract
Understanding neural correlates of brain function in neuroscience now largely involves detecting and analyzing transient signals from fluorescent sensors. Imaging technologies such as confocal and two-photon microscopy, along with onboard miniscopes, enable the visualization of neural activities and capture dynamic signals both ex vivo and in vivo. This includes monitoring Ca2+ transients via the expression of genetically encoded sensors such as GCaMP in specific brain cells. Additionally, the advent of GPCR-based neurotransmitter sensors allows for imaging the release of neurotransmitters including glutamate and GABA, as well as neuromodulators such as dopamine or noradrenaline. These approaches however generate large, high-dimensional, spatiotemporally complex datasets, presenting significant challenges for signal detection and analysis. To overcome these challenges, we developed a versatile pipeline of Dynamic Extraction and Tracking of Emitted Cellular Transients (DETECT), which combines background denoising, object segmentation, and multi-object tracking. Our user-friendly, Python-based GUI offers a low-resource platform for efficient data analysis. Validated across various imaging modalities and biological models, DETECT provides a robust and comprehensive solution for analyzing complex imaging datasets in neuroscience research.