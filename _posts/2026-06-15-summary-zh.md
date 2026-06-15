---
layout: default
title: "Horizon Summary: 2026-06-15 (ZH)"
date: 2026-06-15
lang: zh
---

> From 23 items, 3 important content pieces were selected

---

1. [2014 年演讲《JavaScript 的诞生与死亡》准确预测了 WebAssembly 与 JavaScript 的演变](#item-1) ⭐️ 8.0/10
2. [华为发布开源盘古 2.0 大模型，拥有 5050 亿参数和 512K 上下文长度。](#item-2) ⭐️ 8.0/10
3. [美国政府以出口管制指令迫使 Anthropic 全面封锁其 Fable 5 和 Mythos 5 AI 模型的访问权限。](#item-3) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [2014 年演讲《JavaScript 的诞生与死亡》准确预测了 WebAssembly 与 JavaScript 的演变](https://www.destroyallsoftware.com/talks/the-birth-and-death-of-javascript) ⭐️ 8.0/10

在 2014 年的一次会议演讲中，Gary Bernhardt 预测 JavaScript 将演变为 Web 的通用编译目标，并最终被取代。随着后来 WebAssembly（Wasm）的发展和采用，他的预见被证明是相当准确的。 这次演讲作为一项有先见之明的技术评论具有重要意义，它正确预见了 Web 开发的一次重大架构转变。它强调了前瞻性思想如何塑造行业讨论，并验证了将 WebAssembly 作为与 JavaScript 并行的、可移植的高性能编译目标这一发展趋势。 演讲中特别提到了 asm.js，这是一个早期用作编译目标的 JavaScript 低级子集，是 WebAssembly 的前身。一个值得注意的局限是，虽然 WebAssembly 作为编译目标已经成功，但其在全栈 Web 开发（例如直接操作 DOM）中的应用速度比一些预测要慢，JavaScript 作为“粘合”代码仍然必不可少。

hackernews · subset · Jun 14, 12:38 · [社区讨论](https://news.ycombinator.com/item?id=48526661)

**背景**: JavaScript 是由 Brendan Eich 于 1995 年创建的一种编程语言，最初用于在 Netscape 浏览器中为网页添加交互性。WebAssembly（Wasm）是一种低级的二进制指令格式，被设计为 C/C++和 Rust 等语言的便携式编译目标，使它们能够以接近原生的性能在 Web 上运行。“通用编译目标”的概念指的是一种通用的中间格式，许多不同的高级编程语言都可以被编译成这种格式，从而允许它们在像 Web 浏览器这样的共享运行时环境中执行。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://webassembly.org/">WebAssembly</a></li>
<li><a href="https://developer.mozilla.org/en-US/docs/WebAssembly">WebAssembly - MDN</a></li>
<li><a href="https://en.wikipedia.org/wiki/JavaScript">JavaScript - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 社区讨论反映了对该演讲准确性的钦佩，用户们指出其成功预测了 JavaScript 成为编译目标以及随后 WebAssembly 的兴起。一些评论强调了 Wasm 的发展速度比预期要慢，特别是缺乏直接访问 DOM 的能力，这导致仍需继续使用 JavaScript。另一些人则幽默地指出，该演讲预测了 2020-2025 年左右会发生全球性灾难，尽管性质不同。

**标签**: `#JavaScript`, `#WebAssembly`, `#Programming Languages`, `#Web Development`, `#History of Computing`

---

<a id="item-2"></a>
## [华为发布开源盘古 2.0 大模型，拥有 5050 亿参数和 512K 上下文长度。](https://t.me/zaihuapd/41948) ⭐️ 8.0/10

在华为开发者大会 2026 上，华为发布了开源盘古 openPangu 2.0 模型，包含 5050 亿参数的 Pro 版和 920 亿参数的 Flash 版，均支持 512K 上下文长度。华为计划从 2026 年 6 月 30 日起，陆续开源预训练代码等七大组件。 此次发布是领先的中国科技公司的一次重大开源贡献，可能挑战现有的全球主流大模型，并促进更丰富的 AI 生态系统。该模型针对华为昇腾硬件和鸿蒙系统的优化，也强化了华为的集成化 AI 技术栈，为开发者提供了英伟达 CUDA 生态之外的替代选择。 该模型专门针对华为的昇腾 AI 处理器进行了优化，并适配鸿蒙系统。华为高管余承东表示，虽然华为为支持国内其他企业提供了大量算力，但其自身用于模型开发的算力储备其实非常有限。

telegram · zaihuapd · Jun 14, 08:05

**背景**: 华为的盘古（亦称 openPangu）是一个多模态大语言模型系列，最初于 2021 年 7 月发布。昇腾 AI 处理器是华为自研的 AI 加速芯片，采用专为高效 AI 计算设计的达芬奇架构。上下文长度是指模型单次输入能处理的最大令牌数（大致相当于单词或词片段），512K 的上下文长度使得模型能够分析非常长的文档或对话。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Huawei_PanGu">Huawei PanGu - Wikipedia</a></li>
<li><a href="https://www.sciencedirect.com/book/9780128234884/ascend-ai-processor-architecture-and-programming">Ascend AI Processor Architecture and Programming | ScienceDirect</a></li>
<li><a href="https://medium.com/@anand_sahu/what-is-context-length-in-ai-models-8bb32bbd7719">What is Context Length in AI Models? Large Models... | Medium</a></li>

</ul>
</details>

**标签**: `#AI`, `#Large Language Models`, `#Open Source`, `#Huawei`, `#Machine Learning`

---

<a id="item-3"></a>
## [美国政府以出口管制指令迫使 Anthropic 全面封锁其 Fable 5 和 Mythos 5 AI 模型的访问权限。](https://t.me/zaihuapd/41949) ⭐️ 8.0/10

美国商务部向 Anthropic 公司发出出口管制指令，要求其暂停所有客户（包括美国境内外的外国公民）对 Fable 5 和 Mythos 5 AI 模型的访问。Anthropic 表示，为确保合规，已关闭这两款模型对所有客户的访问权限，但其其他 Claude 模型不受影响。 此举是美国政府基于国家安全考虑，直接干预并限制对特定强大 AI 模型访问的重要先例，标志着出口管制可能从硬件扩展到 AI 软件和模型权重。这可能影响全球 AI 研究合作、前沿模型的商业部署，并为各国政府监管被认为有风险的高级 AI 能力树立范本。 涉事模型 Fable 5 和 Mythos 5 共享相同的底层模型权重和原始能力，其中 Mythos 5 被描述为 Anthropic 能力最强的 AI 模型，尤其以其发现软件安全漏洞的能力而著称。据报道，此次指令与担忧这些模型可能被“越狱”有关，这可能导致未经授权的数据访问或生成有害内容。

telegram · zaihuapd · Jun 14, 09:06

**背景**: 出口管制是美国政府出于国家安全原因，限制敏感技术、商品和信息向外国实体出口的法规。最近，这些管制范围已从高级 AI 芯片扩展到包括使用大量算力训练的非公开 AI 模型权重。AI“越狱”指的是绕过 AI 模型内置安全和伦理防护的技术，可能释放出危险能力，例如生成犯罪活动指令。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://techcrunch.com/2026/06/12/anthropics-safety-warnings-may-have-just-backfired-the-government-has-pulled-the-plug-on-its-most-powerful-ai/">Anthropic 's safety warnings may have just backfired... | TechCrunch</a></li>
<li><a href="https://www.microsoft.com/en-us/security/blog/2024/06/04/ai-jailbreaks-what-they-are-and-how-they-can-be-mitigated/">AI jailbreaks : What they are and how they... | Microsoft Security Blog</a></li>
<li><a href="https://www.sidley.com/en/insights/newsupdates/2025/01/new-us-export-controls-on-advanced-computing-items-and-artificial-intelligence-model-weights">New U.S. Export Controls on Advanced Computing Items and Artificial Intelligence Model Weights: Seven Key Takeaways | Insights | Sidley Austin LLP</a></li>

</ul>
</details>

**标签**: `#AI Regulation`, `#Export Controls`, `#Anthropic`, `#National Security`, `#AI Safety`

---