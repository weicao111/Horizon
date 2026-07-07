---
layout: default
title: "Horizon Summary: 2026-07-07 (ZH)"
date: 2026-07-07
lang: zh
---

> From 28 items, 3 important content pieces were selected

---

1. [Anthropic 研究论文提出语言模型中的'全局工作空间'机制](#item-1) ⭐️ 8.0/10
2. [腾讯发布开源 MoE 大模型 Hy3，参数量达 2950 亿，上下文长度 256K。](#item-2) ⭐️ 8.0/10
3. [马斯克宣布解散 xAI，将其并入 SpaceX 并更名为 SpaceXAI。](#item-3) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Anthropic 研究论文提出语言模型中的'全局工作空间'机制](https://www.anthropic.com/research/global-workspace) ⭐️ 8.0/10

Anthropic 发表了一篇研究论文，识别并研究了大型语言模型内部的一种'全局工作空间'机制，具体定义了一个'J 空间'，用于整合来自不同专用电路的信息。这项工作将该机制与认知科学中的意识'全局工作空间理论'进行了类比。 这项研究意义重大，因为它为理解大型语言模型如何整合和协调不同内部组件的信息提供了一个新颖的、机制性的框架，这是复杂推理的一个关键方面。它通过将模型架构与人类认知和意识理论联系起来，为 AI 可解释性开辟了新途径，并引发了跨学科的讨论。 所提出的'J 空间'在数学上被定义为由特定层的微小扰动引起的最终输出 logits 的预期变化，这是一个与信息几何相关的概念。社区中的一些研究者提醒，虽然与意识的类比很有趣，但这些发现可能更直接地证明了跨不同上下文存在一个共享的抽象推理子空间。

hackernews · in-silico · Jul 6, 17:44 · [社区讨论](https://news.ycombinator.com/item?id=48808002)

**背景**: 全局工作空间理论是认知科学中的一个重要理论，它提出意识产生于一个全脑范围的'工作空间'，信息在此变得对多个认知系统全局可用，以便进行整合和访问。在 AI 领域，可解释性研究旨在理解像大型语言模型这样复杂模型的内部工作原理，这些模型通过跨越多层的数十亿参数来处理信息。Anthropic 此前已发表过关于绘制和追踪语言模型内部'思维'的基础性工作。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Global_Workspace_Theory">Global workspace theory - Wikipedia</a></li>
<li><a href="https://www.anthropic.com/research/mapping-mind-language-model">Mapping the Mind of a Large Language Model - Anthropic</a></li>
<li><a href="https://www.anthropic.com/research/tracing-thoughts-language-model">Tracing the thoughts of a large language model \ Anthropic</a></li>

</ul>
</details>

**社区讨论**: 社区讨论显示出对技术细节的兴趣，有用户引用了通过复制活跃层来提升模型性能等相关实验。关于将'J 空间'与意识觉知进行类比的有效性存在争论，一些人认为将其描述为一个共享的抽象推理子空间更为贴切。另一些用户则认为论文链接的由 Neel Nanda 等研究者撰写的独立评论是更易理解的见解来源。

**标签**: `#artificial-intelligence`, `#machine-learning`, `#neuroscience`, `#research`, `#llm`

---

<a id="item-2"></a>
## [腾讯发布开源 MoE 大模型 Hy3，参数量达 2950 亿，上下文长度 256K。](https://simonwillison.net/2026/Jul/6/hy3/#atom-everything) ⭐️ 8.0/10

腾讯 Hy 团队发布了新的开源大模型 Hy3，这是一个基于 Apache 2.0 许可证的混合专家模型，总参数量达 2950 亿，其中激活参数量为 210 亿，MTP 层参数量为 38 亿，上下文长度达 256K。该模型在 OpenRouter 上提供免费测试，截止日期为 7 月 21 日。 此次发布是开源大模型领域的一次重大进展，Hy3 凭借其巨大规模和 MoE 架构，性能可媲美参数量是其 2-5 倍的旗舰模型。作为一个免费提供的高容量模型，它降低了开发者和研究人员接触前沿 AI 技术的门槛，有望加速相关领域的创新和应用开发。 完整版模型大小为 598GB，而 FP8 量化版本可将其大小缩减至 300GB。该模型在 4 月底发布预览版后，收集了来自 50 多个产品的反馈，并在此基础上使用更高质量的数据进行了扩展的后训练。

rss · Simon Willison · Jul 6, 23:57

**背景**: 混合专家模型是一种神经网络架构，它将计算任务分配给多个专门的子网络（即“专家”），系统会根据不同的输入选择性地激活相应的专家。这种设计使得模型可以拥有巨大的总参数量（如 2950 亿），同时通过每次推理只使用一部分激活参数（如 210 亿）来保持可控的计算成本。FP8 量化是一种通过以 8 位浮点格式存储模型权重来减小模型大小、加速推理的技术，在许多情况下，它在效率和精度之间的平衡优于基于整数的 INT8 量化。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mixture_of_experts">Mixture of experts - Wikipedia</a></li>
<li><a href="https://developer.nvidia.com/blog/applying-mixture-of-experts-in-llm-architectures/">Applying Mixture of Experts in LLM Architectures | NVIDIA Technical Blog</a></li>
<li><a href="https://www.spheron.network/blog/fp8-quantization-inference-performance-hardware-explained/">What is FP8 Quantization? AI Inference Performance, Accuracy, and Hardware Support Explained (2026) | Spheron Blog</a></li>

</ul>
</details>

**标签**: `#llm`, `#open-source`, `#mixture-of-experts`, `#tencent`, `#huggingface`

---

<a id="item-3"></a>
## [马斯克宣布解散 xAI，将其并入 SpaceX 并更名为 SpaceXAI。](https://x.com/i/status/2074214064746832060) ⭐️ 8.0/10

埃隆·马斯克宣布解散其人工智能公司 xAI，该公司将被更名为 SpaceXAI 并完全整合到 SpaceX 旗下。这一更名首次出现在与 Anthropic 达成的一项计算合作公告中，该公司在公告中首次以 SpaceXAI 自称。 此举将马斯克的人工智能、航天和社交媒体业务整合到一个统一的公司架构下，可能简化运营，并使 AI 开发与 SpaceX 的轨道计算等宏伟目标保持一致。这标志着一个重大的战略转变，通过创建一个专注于天基 AI 基础设施的综合性科技巨头，可能重塑行业竞争格局。 这一变化发生在 SpaceX 今年早些时候收购 xAI 之后，该收购案也包括了社交平台 X。美国专利商标局的备案文件表明，新的 SpaceXAI 品牌与建设天基数据中心和轨道计算的计划相关，这符合 SpaceX 潜在 IPO 的更大叙事背景。

telegram · zaihuapd · Jul 7, 02:30

**背景**: xAI 由埃隆·马斯克于 2023 年创立，目标是理解宇宙，并开发了 AI 聊天机器人 Grok。2025 年初，xAI 与 X（前身为 Twitter）合并，随后于 2026 年 2 月被 SpaceX 收购。与 xAI 合作的 Anthropic 是一家专注于 AI 安全的主要公司，以其 Claude 大语言模型而闻名。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://x.ai/">xAI</a></li>
<li><a href="https://www.businessinsider.com/xai-rebrand-spacexai-new-logo-x-handle-spacex-2026-7">XAI Rebrands to SpaceXAI With New Logo... - Business Insider</a></li>
<li><a href="https://en.wikipedia.org/wiki/Anthropic">Anthropic - Wikipedia</a></li>

</ul>
</details>

**标签**: `#Artificial Intelligence`, `#Corporate Strategy`, `#SpaceX`, `#xAI`, `#Industry News`

---