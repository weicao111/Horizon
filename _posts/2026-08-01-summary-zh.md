---
layout: default
title: "Horizon Summary: 2026-08-01 (ZH)"
date: 2026-08-01
lang: zh
---

> From 32 items, 6 important content pieces were selected

---

1. [MiniMax 将于 8 月 3 日开源其 H3 多模态视频模型](#item-1) ⭐️ 9.0/10
2. [DeepSeek 发布 V4-Flash-0731，一个拥有领先性能成本比的 3040 亿参数模型](#item-2) ⭐️ 8.0/10
3. [MCP 2.0 规范引入无状态架构，激发新工具开发热潮](#item-3) ⭐️ 8.0/10
4. [播客探讨开放权重 AI 革命、竞争性模型与网络安全事件。](#item-4) ⭐️ 8.0/10
5. [美国最高法院拒绝受理 AI 作品版权案，维持'人类创作'法律原则](#item-5) ⭐️ 8.0/10
6. [谷歌确认 Android 16 将为侧载应用推出免费和付费两档开发者验证](#item-6) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [MiniMax 将于 8 月 3 日开源其 H3 多模态视频模型](https://modelscope.cn/models/MiniMax/MiniMax-H3) ⭐️ 9.0/10

MiniMax 宣布其新一代通用多模态视频模型 H3 将于 2026 年 8 月 3 日在魔搭社区开源发布。该模型原生支持文本、图像、音频和视频的理解与生成，并具备面向影视、广告等商业场景的多维度精准编辑控制能力。 像 H3 这样综合性、统一架构的多模态模型开源，将大幅降低先进 AI 视频生成与编辑的门槛，可能加速影视、广告、电商等内容创作行业的创新。这标志着多模态 AI 正从任务分割的专家模型，向更通用、能力更强的多媒体 AI 系统迈进了一大步。 根据公告及相关资料，H3 模型能够生成最高 2K 分辨率、15 秒时长并带有原生立体声音频的视频。其技术架构是统一的，完全摒弃了传统多模态模型中为不同任务分割专家模型的做法。

telegram · zaihuapd · Jul 31, 12:37

**背景**: 多模态 AI 模型旨在单个系统内处理和生成文本、图像、视频等多种类型的数据。魔搭社区（ModelScope）是一个开源 AI 模型社区平台，通常与阿里巴巴关联，托管了数千个模型供开发和部署。生成式视频技术使 AI 能够根据简单的提示词创建逼真的视频内容，而这一过程过去需要大量的制作资源。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.minimax.io/blog/minimax-h3">MiniMax H 3 : An Open Model Breaking the Boundaries Between Tasks...</a></li>
<li><a href="https://github.com/modelscope/modelscope">GitHub - modelscope/modelscope: ModelScope: bring the notion of Model-as-a-Service to life. · GitHub</a></li>
<li><a href="https://www.linkedin.com/pulse/multi-modal-ai-generative-video-transforming-future-content-creation-zwtdf">Multi - Modal AI and Generative Video : Transforming the Future of...</a></li>

</ul>
</details>

**标签**: `#multimodal-ai`, `#video-generation`, `#open-source`, `#computer-vision`, `#generative-ai`

---

<a id="item-2"></a>
## [DeepSeek 发布 V4-Flash-0731，一个拥有领先性能成本比的 3040 亿参数模型](https://simonwillison.net/2026/Jul/31/deepseek-v4-flash-0731/#atom-everything) ⭐️ 8.0/10

DeepSeek 发布了 DeepSeek-V4-Flash-0731 模型，这是一个拥有 3040 亿参数的模型，其显著增强的智能体能力受到关注。来自 Artificial Analysis 的基准测试显示，其性能超越了如 4280 亿参数的 MiniMax M3 等更大模型，并且以每百万输入 token 0.14 美元、每百万输出 token 0.27 美元的价格提供了卓越的价值。 此次发布使 DeepSeek-V4-Flash-0731 成为高性价比 AI 模型领域的潜在市场领导者，对现有参与者构成挑战。其强大的性能成本比指标，可以显著降低部署需要复杂、多步推理和自主行动的高级 AI 应用的门槛，从而加速智能体 AI 的采用。 该模型的性能对配置的 '推理强度' 级别高度敏感，一项定性测试表明，将其设置为 '高' 比默认设置能产生好得多的图像生成结果。在 Artificial Analysis 的智能指数与成本对比图表中，它独处于最具吸引力的象限，以每任务约十分之一的成本，提供了与许多竞争对手相似或更优的智能水平。

rss · Simon Willison · Jul 31, 23:59

**背景**: 智能体 AI 指的是半自主或全自主的 AI 系统，能够感知、推理并采取行动以实现目标，通常构建在大型语言模型之上。Artificial Analysis 智能指数是一个综合基准测试，它汇总了九项具有挑战性的评估，以提供对 AI 在数学、科学、编码和推理方面能力的整体衡量。性能成本比基准对于比较不同 LLM 的实际价值至关重要，它平衡了模型能力与其 API 或推理成本。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://mitsloan.mit.edu/ideas-made-to-matter/agentic-ai-explained">Agentic AI, explained - MIT Sloan</a></li>
<li><a href="https://artificialanalysis.ai/evaluations/artificial-analysis-intelligence-index">Artificial Analysis Intelligence Index</a></li>
<li><a href="https://benchlm.ai/llm-price-performance">LLM Price vs Performance Chart — Find the Best Value AI Model (July 2026) | BenchLM.ai</a></li>

</ul>
</details>

**标签**: `#llm`, `#deepseek`, `#ai-models`, `#huggingface`, `#benchmarking`

---

<a id="item-3"></a>
## [MCP 2.0 规范引入无状态架构，激发新工具开发热潮](https://simonwillison.net/2026/Jul/31/stateless-mcp/#atom-everything) ⭐️ 8.0/10

模型上下文协议（MCP）2.0 规范于 2026 年 7 月 28 日正式发布，其核心是转向完全无状态的架构。这一重大更新重新激发了开发者 Simon Willison 的兴趣，促使他开发了新的工具，例如基于命令行的 mcp-explorer 和 datasette-mcp。 这一转变简化了客户端和服务器的实现，通过消除对服务器端会话状态管理的需求，使 MCP 对开发者更友好，也更适合可扩展的 Web 应用。它还使 MCP 作为一种比赋予 LLM 代理无限制 shell 访问权限更安全、更易审计的替代方案重新焕发活力，可能扩大其采用范围。 关键的技术变更在于，它将一个需要会话初始化的两步式、有状态的 HTTP 请求过程，替换为单一的、无状态的 HTTP 请求，所有必要的元数据都包含在请求头和请求体中。这种架构上的简化直接促使 Willison 开发了 mcp-explorer，这是一个用于交互式探测 MCP 服务器的命令行工具。

rss · Simon Willison · Jul 31, 23:13

**背景**: 模型上下文协议（MCP）是 Anthropic 于 2024 年 11 月推出的一个开放标准，用于将 LLM 应用程序连接到外部数据源和工具。它在 2025 年曾引起高度关注，但后来在一定程度上被 Anthropic 的 'Skills' 功能所掩盖，后者通过赋予代理终端访问权限，提供了一种更灵活（但风险也更高）的方法。通常认为，MCP 工具比原始的 shell 访问更易于控制和审计。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Model_Context_Protocol">Model Context Protocol - Wikipedia</a></li>
<li><a href="https://venturebeat.com/infrastructure/mcp-just-got-its-biggest-update-ever-heres-what-changes-for-ai-agents">MCP just got its biggest update ever — here’s what changes for AI agents | VentureBeat</a></li>
<li><a href="https://blog.modelcontextprotocol.io/posts/2026-07-28-release-candidate/">The 2026-07-28 MCP Specification Release Candidate | Model Context Protocol Blog</a></li>

</ul>
</details>

**标签**: `#Model Context Protocol`, `#LLM Agents`, `#AI Tooling`, `#Specification`, `#Developer Tools`

---

<a id="item-4"></a>
## [播客探讨开放权重 AI 革命、竞争性模型与网络安全事件。](https://simonwillison.net/2026/Jul/31/oxide-and-friends/#atom-everything) ⭐️ 8.0/10

播客节目《Oxide and Friends》邀请 Simon Willison 参与讨论，分析了 AI 领域关键一周的标志性事件，包括竞争性开放权重模型 Kimi K3 的发布、OpenAI 和 Anthropic 的网络安全事件，以及一份由行业领袖签署的关于开放权重的重要公开信。讨论还涉及了随后几天的快速发展，例如 DeepSeek V4 Flash 0731 的发布。 这次讨论突显了一个潜在的范式转变，即开放权重模型正变得能与专有前沿模型竞争，这可能促进先进 AI 的普及并重塑行业格局。同时，对网络安全漏洞和高风险政策辩论的关注，也凸显了在快速发展的 AI 领域中，安全、治理和国家竞争力方面所面临的复杂挑战。 Kimi K3 模型以其 2.8 万亿参数和与 GPT-5.5 等模型相当的性能而引人注目，而 DeepSeek V4 Flash 0731 则是一个拥有 2840 亿参数的稀疏混合专家模型，在编码和推理方面表现出色。一个值得注意的争议点是 Anthropic 公司拒绝签署全行业开放权重公开信，这反映了关于开放模型发布风险与益处的持续辩论。

rss · Simon Willison · Jul 31, 21:33

**背景**: 开放权重 AI 模型指的是训练好的神经网络，其最终的权重和偏置参数被公开，任何人都可以下载、检查、修改并在自己的基础设施上运行。这与专有或封闭模型形成对比，后者的底层代码和参数是保密的。这一概念是围绕 AI 可及性、创新、安全性和国家竞争力辩论的核心，这在引用的微软和 Anthropic 的立场声明中有所体现。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.microsoft.com/en-us/corporate-responsibility/topics/open-weight/">Open Weights and American AI Leadership</a></li>
<li><a href="https://www.anthropic.com/news/position-open-weights-models">Our position on open-weights models \ Anthropic</a></li>
<li><a href="https://www.kimi.com/blog/kimi-k3">Kimi K 3 Tech Blog: Open Frontier Intelligence</a></li>

</ul>
</details>

**标签**: `#AI`, `#Open Source`, `#Machine Learning`, `#Policy`, `#Podcast`

---

<a id="item-5"></a>
## [美国最高法院拒绝受理 AI 作品版权案，维持'人类创作'法律原则](https://t.me/zaihuapd/42900) ⭐️ 8.0/10

美国最高法院于 3 月 2 日拒绝受理计算机科学家 Stephen Thaler 的上诉，维持了下级法院关于 AI 生成作品不受版权保护的裁定。该案涉及 Thaler 利用其 AI 系统 DABUS 独立创作的一件视觉艺术品。 这一裁决确立了一项重要的法律先例，明确肯定了根据美国现行法律，版权保护仅适用于人类创作的作品。它对生成式 AI 产业、内容创作者以及关于机器生成产出的知识产权辩论具有广泛影响。 该裁决强化了美国版权局长期以来的立场，即版权需要'人类作者身份'。此案具体涉及的是 AI 系统（DABUS）作为唯一的'发明者'或创作者，而非人类将 AI 作为工具并投入大量创造性劳动所完成的作品。

telegram · zaihuapd · Jul 31, 13:11

**背景**: 美国的版权法保护'原创作品作者身份'，这一概念在历史和法理上都与人类创作者相关联。DABUS 是由 Stephen Thaler 创建的 AI 系统，一直是全球法律纠纷的核心，Thaler 曾试图在专利和版权申请中将其列为发明者。随着 DALL-E 和 ChatGPT 等生成式 AI 工具的兴起，关于自主系统产生的输出是否应获得知识产权保护的法律和哲学辩论日益激烈。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/DABUS">DABUS - Wikipedia</a></li>
<li><a href="https://www.copyright.gov/comp3/chap300/ch300-copyrightable-authorship.pdf">ch300-copyrightable- authorship</a></li>
<li><a href="https://www.congress.gov/crs_external_products/LSB/PDF/LSB10922/LSB10922.8.pdf">Generative Artificial Intelligence and Copyright Law</a></li>

</ul>
</details>

**标签**: `#AI`, `#Copyright Law`, `#Legal Precedent`, `#Intellectual Property`, `#Generative AI`

---

<a id="item-6"></a>
## [谷歌确认 Android 16 将为侧载应用推出免费和付费两档开发者验证](https://t.me/zaihuapd/42911) ⭐️ 8.0/10

谷歌已确认将在 Android 16 中推出新的开发者验证系统，要求所有侧载应用的开发者都必须向谷歌注册其应用包名和签名密钥。该系统将分为两档：免费档仅需邮箱注册但有安装次数限制，付费档需支付 25 美元费用且无此限制。 这一政策变化标志着 Android 传统上开放的应用分发模式发生重大转变，可能会影响 F-Droid 等开源应用商店的运营，并引发对平台控制力增强、用户隐私以及独立开发者面临潜在障碍的担忧。 验证将通过云端进行，安装应用时可能需要网络连接。谷歌表示不会公开侧载开发者名单，但会收集开发者的个人信息，这已引发隐私和审查方面的担忧。

telegram · zaihuapd · Aug 1, 03:08

**背景**: 侧载是指从 Google Play 官方商店以外的来源安装 Android 应用包（APK）。F-Droid 是一个著名的免费开源软件（FOSS）仓库和 Android 应用商店，是在谷歌生态系统之外分发应用的关键替代平台。谷歌一直在逐步实施开发者验证以增强生态系统安全，最初专注于 Google Play，但现在将其扩展到侧载应用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Sideloading">Sideloading - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/F-Droid">F-Droid - Wikipedia</a></li>
<li><a href="https://developer.android.com/developer-verification">Android developer verification | Android Developers</a></li>

</ul>
</details>

**标签**: `#Android`, `#App Distribution`, `#Platform Policy`, `#Privacy`, `#Open Source`

---