---
title: Hippocampo-neocortical interaction as compressive retrieval-augmented generation
title_zh: 海马体-新皮层相互作用作为压缩式检索增强生成
authors: "Spens, E., Burgess, N."
date: 2026-04-08
pdf: "https://www.biorxiv.org/content/10.1101/2024.11.04.621950v4.full.pdf"
tags: ["query:slp-ns"]
score: 7.0
evidence: 海马-新皮层相互作用与记忆神经机制
tldr: 该研究提出了一个将海马体与新皮层交互建模为“压缩检索增强生成（RAG）”的计算模型。研究指出，海马体以压缩形式存储序列经验，并通过回放训练新皮层生成网络，从而提取统计规律并实现泛化。该模型模拟了记忆编码、巩固及提取过程，解释了记忆随时间产生的图式扭曲现象，并揭示了情景记忆与语义记忆在问题解决中的协同作用。
source: biorxiv
selection_source: fresh_fetch
motivation: 旨在阐明海马体（情景记忆）与新皮层（语义记忆）在学习、记忆和问题解决中相互作用的神经机制。
method: 提出一种计算模型，将海马体编码的压缩经验回放给新皮层生成网络，并利用检索增强生成（RAG）框架模拟两者的交互。
result: 模型成功模拟了记忆随时间演变的过程（如基于图式的扭曲），并展示了如何通过结合特定情景信息与通用知识来预测未来和解决问题。
conclusion: 海马体-新皮层交互可被视为一种压缩检索增强生成过程，有效整合了具体经验与抽象规律。
---

## 摘要
学习、记忆和问题解决的许多方面都涉及情景（海马体）系统和语义（新皮层）系统之间的相互作用，但支持这一过程的神经机制尚不清楚。我们提出了一个计算模型，在该模型中，序列经验以压缩形式编码在海马体中，并通过回放来训练新皮层生成网络。该网络捕捉特定情景的要点，并提取可泛化到新情境的统计模式，从而实现对过去的有效重构和对未来的预测。这两个系统在编码、召回和问题解决过程中相互作用，海马体将相关的情景信息检索到工作记忆中，作为利用新皮层网络“通用知识”进行生成的基础。我们将这种相互作用模拟为“检索增强生成”，并增加了将情景记忆压缩进海马体以及将其巩固到新皮层的机制。该模型解释了记忆随时间的变化，包括基于图式的扭曲，并展示了情景记忆和语义记忆如何助力问题解决。

## Abstract
Many aspects of learning, memory, and problem solving involve interplay between episodic (hippocampal) and semantic (neocortical) systems, but the neural mechanisms supporting this are unclear. We present a computational model in which sequential experiences are encoded in hippocampus in compressed form and replayed to train a neocortical generative network. This network captures the gist of specific episodes and extracts statistical patterns that generalise to new situations, enabling efficient reconstruction of the past and prediction of the future. The two systems interact during encoding, recall and problem solving, with the hippocampus retrieving relevant episodic information into working memory as a basis for generation using the 'general knowledge' of the neocortical network. We simulate this interaction as 'retrieval-augmented generation', with the addition of mechanisms to compress episodic memories into hippocampus and to consolidate them into neocortex. The model explains changes to memories over time, including schema-based distortions, and shows how episodic and semantic memory contribute to problem solving.