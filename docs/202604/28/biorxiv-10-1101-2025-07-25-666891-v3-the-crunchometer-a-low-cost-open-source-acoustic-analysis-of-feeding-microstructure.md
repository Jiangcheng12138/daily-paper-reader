---
title: "The Crunchometer: A Low-Cost, Open-Source Acoustic Analysis of Feeding Microstructure"
title_zh: Crunchometer：一种低成本、开源的摄食微观结构声学分析系统
authors: "Gil-Lievana, E., Arroyo, B., Perez-Ortega, J. E., Lopez, A., Rodriguez-Blanco, L. A., Diaz, X., Hernandez, G., Coss, A., Alway, E., Reicher, N., Hernandez-Lemus, E., Kaelberer, M., Bohorquez, D. V., Gutierrez, R."
date: 2026-04-24
pdf: "https://www.biorxiv.org/content/10.1101/2025.07.25.666891v3.full.pdf"
tags: ["query:slp-ns"]
score: 6.0
evidence: 控制食欲和进食微结构的神经回路
tldr: 本研究开发了Crunchometer，这是一种低成本、开源的声学分析系统，旨在解决现有工具在监测固体食物摄入微观结构时成本高或时间分辨率不足的问题。该系统通过计算算法分析进食声音，生成高分辨率行为图谱。实验证明其能精确检测药物干预及饮食偏好变化，并成功结合电生理与钙成像技术，揭示了外侧下丘脑神经元对固体与液体食物摄入的不同编码机制，为食欲研究提供了强有力的工具。
source: biorxiv
selection_source: fresh_fetch
motivation: 现有的固体食物摄入监测工具成本高昂且缺乏足够的时间分辨率，难以与神经活动精确对齐。
method: 开发了一种名为Crunchometer的开源声学系统，利用计算算法从进食声音中提取高分辨率的进食行为图谱。
result: 该系统成功识别了受药物影响的进食抑制及饮食偏好，并揭示了外侧下丘脑神经元对固体食物和液体蔗糖摄入的差异化编码。
conclusion: Crunchometer为研究食欲相关的神经环路提供了一个稳健、易得且具有单次咬合分辨率的分析平台。
---

## 摘要
阐明控制食欲的神经回路需要对固体食物摄入的微观结构进行精确、高分辨率的监测，而现有工具要么成本高昂，要么缺乏将摄食事件与神经活动对齐的时间分辨率，无法满足这一需求。为了克服这一难题，我们开发了 Crunchometer，这是一种低成本、开源的声学系统，利用计算算法根据固体食物摄入过程中产生的声音生成高分辨率的摄食行为谱。在不同能量状态（饥饿/饱腹）下的验证确认了其对摄食微观结构变化的敏感性，且该系统可靠地检测到了司美格鲁肽（semaglutide）诱导的摄入抑制以及对高脂饮食偏好的降低。利用其与自由活动小鼠体内记录的无缝集成，我们将 Crunchometer 与外侧下丘脑（LH）电生理学相结合，识别出了追踪整个进餐过程而非单个摄食片段的“进餐相关”神经元。钙成像进一步揭示了 LH GABA 能和谷氨酸能神经元的不同子集分别对仅摄食、仅舔舐或两种行为都有反应。因此，LH 神经元集群对固体食物与液体蔗糖的摄入进行了差异化编码。这些发现表明，Crunchometer 是一个稳健且易于获取的平台，能够在单次咀嚼的分辨率下剖析摄食行为的神经相关性。

意义声明：Crunchometer 是一种低成本、开源的技术，它使摄食分析普及化，能够精确剖析涉及食欲的神经回路，从而推动肥胖和饮食失调治疗方法的发展。

## Abstract
Elucidating the neuronal circuits that govern appetite requires precise, high-resolution monitoring of the microstructure of solid food consumption, a need unmet by existing tools, which are either costly or lack the temporal resolution to align feeding events with neuronal activity. To overcome this, we developed the Crunchometer, a low-cost, open-source acoustic system that uses computational algorithms to generate high-resolution feeding ethograms from the sounds produced during solid food consumption. Validation across energy states (hunger/satiety) confirmed its sensitivity to changes in feeding microstructure, and the system reliably detected semaglutide-induced suppression of intake and reduced preference for a high-fat diet. Leveraging its seamless integration with in vivo recordings in freely behaving mice, we paired the Crunchometer with lateral hypothalamus (LH) electrophysiology to identify "meal-related" neurons that track entire meals rather than individual bouts. Calcium imaging further revealed that distinct subsets of LH GABAergic and glutamatergic neurons were tuned to feeding only, to licking only, or to both behaviors. Thus, LH neuronal ensembles differentially encode the consumption of solid food versus liquid sucrose. These findings demonstrate that the Crunchometer is a robust, accessible platform for dissecting the neural correlates of feeding behavior at the resolution of a single bite.

Significance statementThe Crunchometer is a low-cost, open-source technology that democratizes feeding analysis, enabling the precise dissection of neuronal circuits involved in appetite to advance therapies for obesity and eating disorders.