---
layout: default
title: "Horizon Summary: 2026-07-30 (ZH)"
date: 2026-07-30
lang: zh
---

> From 31 items, 3 important content pieces were selected

---

1. [开源引擎通过 SSD 流式加载，在 M 系列 Mac 上仅用 2GB RAM 运行 Gemma 4 26B 模型。](#item-1) ⭐️ 8.0/10
2. [自复制 AI 蠕虫通过 Microsoft Word 文档中的隐藏指令利用 Copilot 传播](#item-2) ⭐️ 8.0/10
3. [OpenAI 宣布向 10 万名学术研究人员免费开放前沿 AI 模型](#item-3) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [开源引擎通过 SSD 流式加载，在 M 系列 Mac 上仅用 2GB RAM 运行 Gemma 4 26B 模型。](https://github.com/drumih/turbo-fieldfare) ⭐️ 8.0/10

开发者 'drumih' 发布了 TurboFieldfare，这是一个用 Swift 和 Metal 编写的开源推理引擎，能够在任何 M 系列 Mac 上仅使用约 2GB RAM 运行 4 位量化的 Gemma 4 26B-A4B-IT 模型。其核心技巧是在推理过程中，将共享模型部分和 KV 缓存保留在 RAM 中，同时从 SSD 流式加载每个 token 所需的路由专家权重。 这项创新极大地推动了设备端 AI 的实用边界，使得大型、能力强的语言模型能够在内存受限的消费级硬件（如 8GB 内存的 MacBook Air）上运行。它展示了一条可行的路径，让用户无需依赖昂贵的高内存硬件或云端服务，就能使用强大的 AI 模型。 该引擎在 8GB 内存的 M2 MacBook Air 上能达到每秒 5-6 个 token，在 M5 MacBook Pro 上能达到每秒 31-35 个 token。它包含一个实验性的、兼容 OpenAI 的本地服务器，支持流式输出和工具调用。一个关键的技术细节是使用了有界的并行 `pread` 调用，将 SSD 读取与共享层的 GPU 计算重叠进行，以缓解 SSD 的延迟。

hackernews · gitpusher42 · Jul 29, 15:05 · [社区讨论](https://news.ycombinator.com/item?id=49098510)

**背景**: Gemma 4 26B 是谷歌推出的大型语言模型，其 4 位量化版本通过仅用 4 比特表示权重（而非标准的 16 或 32 比特）来减少内存占用。该模型采用了混合专家（Mixture of Experts, MoE）架构，每个输入只激活一部分'专家'神经网络，这使得选择性权重流式加载成为可能。Metal 是苹果的低层级 GPU API，而 Swift 是苹果平台的主要编程语言，这使得该解决方案成为原生 macOS/iOS 方案。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/blog/moe">Mixture of Experts Explained</a></li>
<li><a href="https://www.emergentmind.com/topics/4-bit-model-quantization">4-Bit Model Quantization</a></li>
<li><a href="https://huggingface.co/docs/diffusers/en/optimization/mps">Metal Performance Shaders (MPS) · Hugging Face</a></li>

</ul>
</details>

**社区讨论**: 社区表现出浓厚兴趣，讨论内容涵盖技术对比、针对旧版 macOS 的变通方案以及潜在的合作可能。一位用户将该方法与 llama.cpp 中使用`mmap`的方式进行了比较，询问同步 SSD 读取的具体优势。另一位用户分享了在 macOS 15 上编译的变通方案，还有一位从事相关项目（DiffusionGemma）的开发者表达了共享优化成果的兴趣。

**标签**: `#on-device-ai`, `#inference-optimization`, `#llm`, `#memory-efficiency`, `#apple-silicon`

---

<a id="item-2"></a>
## [自复制 AI 蠕虫通过 Microsoft Word 文档中的隐藏指令利用 Copilot 传播](https://simonwillison.net/2026/Jul/29/ai-worming-through-word/#atom-everything) ⭐️ 8.0/10

安全研究员 Håkon Måløy 发现了一种新型提示词注入攻击，能使自复制 AI 蠕虫通过 Microsoft Word 传播。该蠕虫通过在文档中嵌入隐藏指令实现；当该文档被用作 Word 中 Copilot 的源材料时，AI 可能会执行这些指令并将其复制到新文档中，从而使蠕虫能够自主传播。 这标志着 AI 安全威胁的重大升级，将常见的提示词注入漏洞转变为一种能够在文档和工作流中自主传播的蠕虫，且无需原始攻击文件。它凸显了任何使用 AI 辅助生产力工具的组织所面临的关键供应链风险，因为受信任的工作流程可能被利用来传播恶意软件或虚假信息。 该漏洞已向微软进行了负责任的披露，微软有 144 天的时间来解决它，但截至报告发布时，尚无针对此类攻击的全面缓解措施。该攻击利用了文档中的隐藏文本（如白底白字），这是一种在其他场景中出现过的技术，但这是首次已知的通过 AI 代理实现自我复制的实例。

rss · Simon Willison · Jul 29, 18:43

**背景**: 提示词注入是一种安全漏洞，攻击者隐藏在输入数据中的对抗性指令会操纵 AI 模型的行为，可能导致其执行非预期的操作。自复制 AI 蠕虫，如早期的'Morris II'研究，利用对抗性提示词通过检索增强生成在 AI 应用间传播。Microsoft Copilot 是集成在 Microsoft 365 应用程序（包括 Word）中的 AI 助手，旨在帮助用户起草和编辑内容。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Prompt_injection">Prompt injection - Wikipedia</a></li>
<li><a href="https://thehackernews.com/2026/06/researchers-build-self-replicating-ai.html">Researchers Build Self - Replicating AI Worm That Operates Entirely...</a></li>
<li><a href="https://enklypesalt.com/posts/context-collapse-part3-ai-worming-through-word/">Context Collapse, Part 3 - AI Worming through Word | En Klype Salt</a></li>

</ul>
</details>

**标签**: `#ai-security`, `#prompt-injection`, `#microsoft-copilot`, `#vulnerability`

---

<a id="item-3"></a>
## [OpenAI 宣布向 10 万名学术研究人员免费开放前沿 AI 模型](https://openai.com/index/chatgpt-for-academic-researchers/) ⭐️ 8.0/10

OpenAI 于 2026 年 7 月 29 日宣布启动“ChatGPT for Academic Researchers”项目，计划在 2027 年前向全球 10 万名科学、数学和工程领域的研究人员免费提供其前沿 AI 模型。该项目将于今年夏天首批开放 1 万个名额，参与者可使用 GPT-5.6 系列模型，且工作区数据默认不会用于模型训练。 这一举措是 OpenAI 对全球科研界的一项重大战略投资，有望加速基因组学、蛋白质建模和材料科学等领域的发现。通过降低使用尖端 AI 工具的门槛，该项目可以普及先进的研究能力，并促进学术界的创新。 项目提供的访问权限包括 GPT-5.6 模型系列（Luna, Terra, Sol 等变体），并附带针对研究任务的培训和技术支持。申请资格仅限于具有高水平研究活动的学位授予机构的研究人员，申请人需验证其机构身份并提交研究计划。每位参与者最多可邀请四位机构合作者。

telegram · zaihuapd · Jul 30, 00:17

**背景**: 前沿 AI 模型是指市场上能够部署的能力最强、处于技术前沿的系统，通常具备先进的推理和工具集成能力。GPT-5.6 是 OpenAI 于 2026 年 7 月发布的最新大型语言模型系列，包含不同能力等级的变体，在生物学和编程等科学领域具有增强的性能。AI 辅助蛋白质建模是一个关键应用，它利用 AI 来预测和设计蛋白质结构，这对于药物发现和理解生物过程至关重要。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/GPT-5.6">GPT-5.6 - Wikipedia</a></li>
<li><a href="https://openai.com/index/gpt-5-6/">GPT-5.6: Frontier intelligence that scales with your ambition | OpenAI</a></li>
<li><a href="https://nhimg.org/glossary/frontier-ai-model/">What Is Frontier AI model ? Definition & Examples</a></li>

</ul>
</details>

**标签**: `#AI Research`, `#OpenAI`, `#Academic Collaboration`, `#GPT-5`, `#Science`

---