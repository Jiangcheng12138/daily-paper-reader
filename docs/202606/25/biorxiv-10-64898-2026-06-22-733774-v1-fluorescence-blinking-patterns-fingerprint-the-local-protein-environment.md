---
title: Fluorescence Blinking Patterns Fingerprint the Local Protein Environment
title_zh: 荧光闪烁模式指纹识别局部蛋白质环境
authors: "Püntener, S., Kossmann, D., Bielec, K., Rivera-Fuentes, P."
date: 2026-06-23
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.22.733774v1.full.pdf"
tags: ["query:qll"]
score: 6.0
evidence: 提供荧光指纹识别方法检测局部蛋白环境，对翻译后修饰敏感，可用于老化中蛋白修饰研究
tldr: 蛋白质功能受构象和修饰影响，现有单分子识别方法常牺牲构象信息。本文利用自发闪烁荧光团标记完整蛋白，其闪烁动力学受局部化学环境影响，结合深度学习提取指纹，实现不同蛋白、同一蛋白不同区域及单个翻译后修饰的高精度区分。该技术将荧光闪烁用于蛋白指纹识别和表面化学探测。
source: biorxiv
selection_source: fresh_fetch
motivation: 现有单分子蛋白识别方法需变性或酶解，丢失折叠构象信息，无法区分功能不同的蛋白变构体。
method: 在蛋白上共价连接自发闪烁荧光团，记录其荧光-暗态转换的热力学与动力学，利用深度学习分析闪烁模式。
result: 成功区分不同蛋白、同一蛋白不同结合口袋及单翻译后修饰，分类准确率极高。
conclusion: 单分子荧光闪烁可作为非变性蛋白指纹识别方法，同时原位探测蛋白表面局部化学环境。
---

## 摘要
蛋白质的功能不仅取决于其序列，还取决于翻译后修饰和折叠，这些修饰和折叠产生功能不同的蛋白形式。用于蛋白质鉴定的单分子方法，如纳米孔测序，通常需要变性或蛋白水解，从而牺牲了构成蛋白形式多样性的构象信息。在这里，我们通过使用单一共价标记记录其局部表面化学的光学指纹来识别完整的折叠蛋白质。该信号是通过已建立的生物偶联反应连接到蛋白质上的自发闪烁荧光团产生的。其荧光态和暗态之间转换的热力学和动力学受直接蛋白质环境的影响，且这种影响在化学上可解释。通过深度学习可以提取更多区分信息，实现出色的识别准确性。使用这种方法，我们区分了不同的蛋白质、同一蛋白质的不同口袋以及单一翻译后修饰的存在，在每种情况下都将分类追溯到不同的物理化学机制。这些结果确立了单分子荧光闪烁既是一种蛋白质指纹识别方法，也是折叠蛋白质表面局部化学的探针。

## Abstract
The function of a protein depends not only on its sequence but on post-translational modifications and folding that produce functionally distinct proteoforms. Single-molecule methods for protein identification, such as nanopore sequencing, typically require denaturation or proteolysis, sacrificing conformational information that contributes to proteoform diversity. Here, we identify intact, folded proteins by recording an optical fingerprint of their local surface chemistry using a single covalent label. The signal is produced by a spontaneously blinking fluorophore attached to the protein through established bioconjugation reactions. The thermodynamics and kinetics of its switching between a fluorescent and a dark state are influenced by the immediate protein environment in a chemically interpretable manner. Further discriminative information can be extracted using deep learning to achieve excellent identification accuracy. Using this approach, we distinguish different proteins, different pockets of the same protein, and the presence of a single post-translational modification, in each case tracing the classification back to a distinct physicochemical mechanism. These results establish single-molecule fluorescence blinking as both a protein fingerprinting method and a probe of local chemistry on the surface of folded proteins.