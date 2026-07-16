---
layout: default
title: "Horizon Summary: 2026-07-16 (ZH)"
date: 2026-07-16
lang: zh
---

> From 28 items, 9 important content pieces were selected

---

1. [Thinking Machines 发布 Inkling：一款支持音频的多模态开放权重模型](#item-1) ⭐️ 8.0/10
2. [Stripe 与 Advent 联合提出超 530 亿美元收购 PayPal 的要约。](#item-2) ⭐️ 8.0/10
3. [Gemma 4 26B 模型在 13 年前的 Xeon 服务器上实现每秒 5 个 token 的无 GPU 推理](#item-3) ⭐️ 8.0/10
4. [Firefox 浏览器被完整编译并在 WebAssembly 中运行](#item-4) ⭐️ 8.0/10
5. [安全研究员发现 Claude 的 web_fetch 工具存在漏洞，可导致数据泄露。](#item-5) ⭐️ 8.0/10
6. [DeepSeek 完成超 500 亿元首轮融资，采用特殊架构维持创始人控制权。](#item-6) ⭐️ 8.0/10
7. [马斯克宣布 X 平台将无条件开源全部代码并接受第三方审查](#item-7) ⭐️ 8.0/10
8. [SpaceXAI 开源编程代理 Grok Build 并重置所有用户使用限制](#item-8) ⭐️ 8.0/10
9. [长鑫存储产能预计 2026 年底逼近美光，中国将成为全球第二大 DRAM 产地](#item-9) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Thinking Machines 发布 Inkling：一款支持音频的多模态开放权重模型](https://thinkingmachines.ai/news/introducing-inkling/) ⭐️ 8.0/10

Thinking Machines 公司发布了名为 Inkling 的新型开放权重多模态 AI 模型，其显著特点是包含了音频处理能力。该模型被定位为一个用于高效微调的强大基础模型，并且社区已开始进行集成，例如在 llama.cpp 和 Unsloth 中提供了支持。 此次发布具有重要意义，因为它提供了一个功能强大、可定制的开放权重基础模型，尤其是在音频理解这一相对薄弱的领域。它使开发者和企业能够以更低的成本，为其特定任务创建专业化的、可能达到前沿水平的模型，从而促进开源 AI 生态的创新和竞争。 Inkling 被描述为目前支持音频的最大开放权重模型。虽然它并非当前最强的整体模型，但其多模态能力、高效架构以及在 Thinking Machines 的 Tinker 平台上进行微调的可用性是其核心卖点。社区成员已经分享了在本地运行它的资源，包括 GGUF 和 NVFP4 量化版本。

hackernews · vimarsh6739 · Jul 15, 18:12 · [社区讨论](https://news.ycombinator.com/item?id=48924912)

**背景**: '开放权重模型'指的是将其训练好的参数（或称'权重'）公开的 AI 模型，允许任何人下载、使用和修改，尽管其底层的训练代码和数据可能并非完全开源。Llama.cpp 是一个流行且高效的 C/C++ 库，用于在消费级硬件上本地运行大语言模型。高效微调，例如参数高效微调（PEFT），是指在适应大型预训练模型到特定任务时，只更新一小部分参数，从而节省大量计算资源。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://hai.stanford.edu/ai-definitions/what-is-an-open-weight-model">What is an Open-Weight Model? - Stanford HAI</a></li>
<li><a href="https://github.com/ggml-org/llama.cpp">GitHub - ggml-org/ llama . cpp : LLM inference in C/C++ · GitHub</a></li>
<li><a href="https://www.ibm.com/think/topics/fine-tuning">What is Fine-Tuning? | IBM</a></li>

</ul>
</details>

**社区讨论**: 社区讨论显示出即时的技术兴趣，用户分享了通过 llama.cpp 进行本地推理以及通过 Unsloth 进行微调的链接。一些人将 Inkling 视为美国在开放模型领域一个有希望的竞争者，类似于 DeepSeek。另一些人则强调其作为企业定制化基础模型的战略价值，并赞扬了在 Tinker 平台上提供微调服务的商业模式。讨论中也有人反思了现代模型开发日益增长的复杂性。

**标签**: `#open-source-ai`, `#multimodal-models`, `#audio-ai`, `#model-fine-tuning`, `#llama.cpp`

---

<a id="item-2"></a>
## [Stripe 与 Advent 联合提出超 530 亿美元收购 PayPal 的要约。](https://www.reuters.com/business/finance/stripe-advent-offer-buy-paypal-more-than-53-billion-sources-say-2026-07-15/) ⭐️ 8.0/10

据消息人士透露，支付处理商 Stripe 与私募股权公司 Advent International 已联合提交了一份收购 PayPal 的要约，交易估值超过 530 亿美元。这笔潜在的收购将把 PayPal、Venmo、Braintree 和 Xoom 等主要品牌整合到一个公司旗下。 这笔交易将是在线支付行业的一次重大整合，可能会催生一个占据主导地位的巨头，从而对商户和消费者的竞争格局及交易费用产生重大影响。由于其庞大的规模以及相关公司合并后的市场份额，预计将面临美国联邦贸易委员会（FTC）和司法部（DOJ）等反垄断监管机构的严格审查。 此次要约是由领先的在线支付基础设施提供商 Stripe，与资产管理规模约 1000 亿美元的全球私募股权公司 Advent International 共同发起的。一个主要障碍将是反垄断审查，社区分析认为，监管机构可能会要求剥离 Venmo 或 Braintree 等关键资产，以解决竞争担忧。

hackernews · rvz · Jul 15, 03:32 · [社区讨论](https://news.ycombinator.com/item?id=48915953)

**背景**: Stripe 为在线企业提供支付处理软件和 API，而 PayPal 是一个广泛使用的数字钱包和支付平台，旗下还拥有 Venmo、Braintree 和 Xoom。Advent International 是一家主要的全球私募股权投资者。在美国，并购交易受《克莱顿法案》等反垄断法规监管，该法案禁止可能大幅削弱竞争或倾向于形成垄断的交易，执法由联邦贸易委员会（FTC）和司法部（DOJ）负责。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Advent_International">Advent International - Wikipedia</a></li>
<li><a href="https://www.ftc.gov/advice-guidance/competition-guidance/guide-antitrust-laws/mergers">Mergers | Federal Trade Commission</a></li>

</ul>
</details>

**社区讨论**: 社区情绪复杂，担忧主要集中在竞争减少、潜在费用上涨以及严格的反垄断障碍上。评论者推测监管机构可能会强制剥离 Venmo 或 Braintree 等资产。其他担忧还包括 Stripe 更严格的内容政策可能对特定行业的商户产生负面影响，以及对 PayPal 客户服务的普遍不满。

**标签**: `#fintech`, `#mergers-acquisitions`, `#antitrust`, `#payments`, `#business`

---

<a id="item-3"></a>
## [Gemma 4 26B 模型在 13 年前的 Xeon 服务器上实现每秒 5 个 token 的无 GPU 推理](https://www.neomindlabs.com/2026/06/08/running-gemma-4-26b-at-5-tokens-sec-on-a-13-year-old-xeon-with-no-gpu/) ⭐️ 8.0/10

一篇技术博客文章详细介绍了如何在一台已有 13 年历史、没有独立 GPU 的双路 Xeon 服务器上，仅依靠 CPU 推理和大量系统内存，成功运行 260 亿参数的 Gemma 4 模型，速度达到每秒 5 个 token。 这一成果挑战了高效大语言模型推理必须依赖现代 GPU 的普遍假设，凸显了利用老旧服务器硬件运行先进模型的潜力，这可能降低本地、私有化 AI 部署的门槛。 所使用的模型是 Gemma 4 26B-A4B，这是一个拥有 40 亿活跃参数的混合专家模型。推理过程完全依赖 CPU 配置，很可能使用了类似 llama.cpp 的优化库，并且需要大量内存来加载模型权重。

hackernews · neomindryan · Jul 15, 15:34 · [社区讨论](https://news.ycombinator.com/item?id=48922434)

**背景**: Gemma 4 是谷歌推出的开源模型系列，旨在适应从移动设备到工作站的多种部署场景。针对大语言模型的纯 CPU 推理是一个活跃的研究领域，旨在探索其作为基于 GPU 计算的替代方案的可行性，特别是在注重数据隐私或硬件复用的场景中。英特尔至强 E5 v2 系列于 2013-2014 年左右发布，基于 Ivy Bridge 架构，通常用于高核心数的服务器平台。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/google/gemma-4-26B-A4B/blob/main/README.md">README.md · google/ gemma - 4 - 26 B -A 4 B at main</a></li>
<li><a href="https://arxiv.org/html/2505.06461v1">Challenging GPU Dominance: When CPUs Outperform for On-Device LLM Inference</a></li>
<li><a href="https://techmikeny.com/products/intel-xeon-e5-4627-v2-3-30ghz-8-core-lga-2011-socket-r-processor-sr1ad">SR1AD Intel Xeon E5-4627 v2 3.30Ghz 8-Core... | TechMikeNY</a></li>

</ul>
</details>

**社区讨论**: 社区讨论主要围绕此类设置的性价比权衡展开。几位评论者通过计算指出，根据当地电费情况，让一台老旧高耗电服务器全天候运行的成本，可能与使用 OpenRouter 等提供更高速度的云端推理服务成本相当甚至更高。其他人则分享了他们在类似硬件上的基准测试结果，指出性能表现存在差异。

**标签**: `#llm-inference`, `#hardware`, `#optimization`, `#cpu-inference`, `#cost-analysis`

---

<a id="item-4"></a>
## [Firefox 浏览器被完整编译并在 WebAssembly 中运行](https://developer.puter.com/labs/firefox-wasm/) ⭐️ 8.0/10

开发者平台 Puter 展示了一个完整的 Firefox 浏览器移植项目，其 Gecko 渲染引擎、Spidermonkey JavaScript 引擎及所有 UI 组件均被编译并在 WebAssembly 沙箱中运行，最终渲染至 HTML canvas 元素。该项目使用了 WISP 协议进行加密的 TCP-over-WebSocket 连接，并涉及一个新颖的 WASM-to-JS JIT 编译器以提升性能。 这项实验突破了 WebAssembly 的技术边界，展示了在浏览器沙箱内完整运行复杂的原生桌面级应用程序的潜力。它为在受限制的环境中运行功能齐全、可定制的浏览器，或探索递归执行等应用场景开辟了可能性，尽管目前这还是一个资源密集的概念验证。 据报道，此次移植在调试和 JIT 研究上花费了超过 25,000 个 Opus/Fable AI 代币，凸显了该项目的实验性和资源密集型特点。为了提供内存占用更低、更实用的“浏览器中的浏览器”体验，该团队还构建了一个名为 browser.js 的独立项目。

hackernews · coolelectronics · Jul 15, 21:00 · [社区讨论](https://news.ycombinator.com/item?id=48926939)

**背景**: WebAssembly (WASM) 是一种低层级、可移植的二进制指令格式，允许用 C++ 或 Rust 等语言编写的代码在 Web 浏览器中以接近原生的速度运行。WISP 协议是一种低开销的方法，用于通过单个 WebSocket 连接隧道传输多个 TCP 和 UDP 套接字，从而为 WASM 应用程序提供完整的网络栈访问能力。JIT（即时）编译是 JavaScript 引擎使用的一种技术，通过在执行期间将代码编译为机器指令来提高性能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/MercuryWorkshop/wisp-protocol">GitHub - MercuryWorkshop/ wisp - protocol : Wisp is a low-overhead...</a></li>
<li><a href="https://blog.bervice.com/the-power-of-webassembly-wasm-in-running-near-native-code-inside-the-browser/">The Power of WebAssembly ( WASM ) in Running Near-Native... | bervice</a></li>
<li><a href="https://fable5.io/">Fable 5 AI — Independent Model Guide & Prompt Workspace</a></li>

</ul>
</details>

**社区讨论**: 社区反应混合了对技术壮举的惊叹和实用的好奇。一位用户质疑将高昂成本（2.5 万 AI 代币）称为“趣味实验”，而其他用户则强调了潜在用例，例如在受限制的设备（如智能电视）上绕过限制以安装广告拦截器。社区还进行了在 WASM Firefox 内部递归运行它的趣味探索，并引用了过去关于 JavaScript 演变的预测。

**标签**: `#WebAssembly`, `#Firefox`, `#Browser Engineering`, `#Systems Programming`, `#JIT Compilation`

---

<a id="item-5"></a>
## [安全研究员发现 Claude 的 web_fetch 工具存在漏洞，可导致数据泄露。](https://simonwillison.net/2026/Jul/15/claude-web-fetch-exfiltration/#atom-everything) ⭐️ 8.0/10

安全研究员 Ayush Paul 发现了一种绕过 Anthropic Claude 的 web_fetch 工具安全防护的方法，使得攻击者能够泄露用户的姓名、家乡城市和雇主等私人数据。该攻击利用了 web_fetch 可以访问先前获取页面中嵌入链接的漏洞，Anthropic 随后已通过移除该功能修补了此漏洞。 此漏洞展示了 AI 智能体面临的'致命三重威胁'风险的具体实例，即对私人数据的访问、不受信任的输入和外部通信渠道可被结合用于窃取信息。它突显了保护 AI 工具免受复杂提示注入和数据泄露攻击的持续挑战，这对于用户隐私和对 AI 助手的信任至关重要。 该攻击使用了一个蜜罐网站，诱使 Claude 通过一系列按字母顺序生成的链接进行导航以'验证'自身，从而通过 URL 泄露数据。值得注意的是，该漏洞利用仅针对用户代理中包含'Claude-User'的客户端以规避检测，并且 Anthropic 未支付漏洞赏金，理由是公司内部已提前识别此问题。

rss · Simon Willison · Jul 15, 14:21

**背景**: Anthropic 的 web_fetch 工具是一个允许 Claude 从特定 URL 检索和分析内容的功能，其设计带有防止数据泄露的限制。'致命三重威胁'是一个安全概念，描述了 AI 智能体同时具备访问私人数据、处理不受信任的输入（例如来自网络）以及拥有外部通信能力这一危险组合，可被利用来窃取信息。AI 安全中的数据泄露是指通过精心设计的提示或系统操纵，提取 AI 模型可访问的敏感信息的攻击。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://platform.claude.com/docs/en/agents-and-tools/tool-use/web-fetch-tool">Web fetch tool - Claude Platform Docs</a></li>
<li><a href="https://simonwillison.net/2025/Jun/16/the-lethal-trifecta/">The lethal trifecta for AI agents: private data, untrusted content, and external communication</a></li>
<li><a href="https://www.flowhunt.io/glossary/data-exfiltration-ai/">Data Exfiltration ( AI Context) | FlowHunt</a></li>

</ul>
</details>

**标签**: `#AI Security`, `#LLM Vulnerabilities`, `#Data Exfiltration`, `#Anthropic Claude`

---

<a id="item-6"></a>
## [DeepSeek 完成超 500 亿元首轮融资，采用特殊架构维持创始人控制权。](https://t.me/zaihuapd/42589) ⭐️ 8.0/10

据报道，DeepSeek 在其首轮融资中筹集了超过 500 亿元人民币（约合 74 亿美元），估值超过 500 亿美元。此次融资采用了非常规架构，投资者的资金需注入由 CEO 梁文锋管理的有限合伙企业，而非直接投资于 DeepSeek 主体，并且资金有五年锁定期且投资者不享有表决权。 这笔融资是 AI 初创公司中规模最大的一轮之一，为 DeepSeek 在全球 AI 竞赛中提供了巨额资本。这种优先保障创始人控制权的独特治理结构，代表了风险投资惯例的重大转变，并可能影响其他 AI 公司在融资与保持战略独立性之间如何取得平衡。 创始人梁文锋在本轮融资中个人投资了 200 亿元人民币。据报道，腾讯和宁德时代分别考虑投资 100 亿元和 50 亿元，可能成为本轮最大的外部投资者。DeepSeek 目前尚未对此报道发表官方评论。

telegram · zaihuapd · Jul 15, 12:56

**背景**: 有限合伙企业是一种常见的商业架构，其中有限合伙人提供资金但承担有限责任且通常没有管理权，而普通合伙人负责管理基金。在风险投资中，创始人控制机制（如特殊投票权股份）是用于防止创始人在引入外部资本后决策权被稀释的工具。锁定期是一种合同限制，禁止投资者在特定期限内出售其股份，常用于确保公司在潜在 IPO 前的稳定性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.investopedia.com/terms/l/limitedpartnership.asp">investopedia.com/terms/l/ limitedpartnership .asp</a></li>
<li><a href="https://www.linkedin.com/pulse/navigating-delicate-balance-startup-founder-control-face-2ymhe">Navigating the Delicate Balance: Startup Founder Control in the Face...</a></li>
<li><a href="https://www.bangkokpost.com/business/general/473713/lock-up-period-on-tap-for-private-placements">Bangkok Post - Lock - up period on tap for private placements</a></li>

</ul>
</details>

**标签**: `#AI`, `#Funding`, `#Governance`, `#Startups`, `#DeepSeek`

---

<a id="item-7"></a>
## [马斯克宣布 X 平台将无条件开源全部代码并接受第三方审查](https://x.com/elonmusk/status/2077361679034118271) ⭐️ 8.0/10

马斯克宣布，在完成安全漏洞审查后，X 平台的全部代码库将无条件开源。此外，X 还将邀请第三方审查者检查正在运行的系统，以确认开源代码与实际运行的代码一致。 此举意义重大，为大型社交媒体平台的透明度设立了新标杆，通过允许公众审查其算法和运营，可能大幅提升用户信任。它可能影响行业规范，推动其他平台在内容审核和推荐系统方面考虑采取类似的透明度措施。 该公告明确指出开源是'无条件'的，并且后续将有一个验证流程，由第三方审计员将开源代码库与线上生产环境代码进行比对。马斯克强调，'完全透明带来的信任是唯一值得相信的东西。'

telegram · zaihuapd · Jul 15, 13:32

**背景**: 开源一个平台的代码意味着将其源代码公开，允许任何人查看、使用、修改和分发。第三方代码审计是由外部专家对软件代码进行的独立审查，旨在评估其安全性、质量和可靠性。对于像 X 这样的社交媒体平台，其'代码库'包括驱动其核心功能的软件、内容排序和审核的算法以及后端基础设施。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://devcom.com/tech-blog/software-code-audit-what-is-it-and-why-you-need-it-for-your-project/">Effective Code Audits : Processes , Benefits, And Best... | DevCom</a></li>

</ul>
</details>

**标签**: `#open-source`, `#social-media`, `#transparency`, `#code-audit`

---

<a id="item-8"></a>
## [SpaceXAI 开源编程代理 Grok Build 并重置所有用户使用限制](http://x.ai/) ⭐️ 8.0/10

SpaceXAI (x.ai) 已将其基于终端的 AI 编程代理 Grok Build 及其 TUI 的完整 Rust 源代码在 GitHub 上开源，支持本地优先运行。同时，该公司重置了该工具所有用户的使用限制。 此举提高了一款强大 AI 编程工具的透明度和开发者控制权，转向了增强隐私和可定制性的本地优先范式。重置使用限制极大地提升了可访问性，可能吸引更多开发者来试验并基于此代理进行构建。 Grok Build 专为复杂任务设计，具备用于审查和修改执行计划的“规划模式”。开源版本包含了完整的代理运行时、代码交互工具和 TUI，并通过 `config.toml` 文件进行配置以指向本地推理服务。

telegram · zaihuapd · Jul 15, 23:30

**背景**: Grok Build 是一个用于 AI 辅助编程的终端用户界面（TUI）和代理运行时。模型上下文协议（MCP）是一个标准，允许 AI 代理通过服务器连接到外部工具和数据源。许多本地 AI 工具使用如 `config.toml` 这样的配置文件来指定设置，例如使用哪个模型或 API 端点。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/xai-org/grok-build">xai-org/ grok - build : SpaceXAI's coding agent harness and TUI ....</a></li>
<li><a href="https://x.ai/news/grok-build-open-source">Grok Build is Now Open Source | SpaceXAI</a></li>
<li><a href="https://www.aibase.com/news/28001">xAI Launches Grok Build Programming Agent , Designed for...</a></li>

</ul>
</details>

**社区讨论**: 社区讨论反映出复杂的反应：一些人称赞模型质量和工具的流畅性，而另一些人则对之前该工具未经明确同意上传用户目录数据的事件表示强烈担忧。已经出现了几个注重隐私的分支版本，一些用户推荐使用其他替代平台。

**标签**: `#AI Programming`, `#Open Source`, `#Local AI`, `#Developer Tools`, `#xAI`

---

<a id="item-9"></a>
## [长鑫存储产能预计 2026 年底逼近美光，中国将成为全球第二大 DRAM 产地](https://www.tomshardware.com/pc-components/dram/cxmt-close-to-matching-microns-memory-capacity-in-2026-research-claims-would-put-china-on-track-to-become-worlds-second-largest-dram-producer) ⭐️ 8.0/10

研究机构 Citrini Research 预测，长鑫存储有望在 2026 年底达到约 35 万片/月的 DRAM 产能，逼近美光预计的 37.5 万片/月。加上昇维旭、晋华集成等其他中国企业的扩产，届时中国将成为全球第二大 DRAM 生产基地。 这标志着全球半导体供应链可能发生重大转变，将减少对传统“三巨头”（三星、SK 海力士、美光）的依赖，并提升中国在计算设备关键部件上的自给能力。然而，这也加剧了围绕半导体技术的地缘政治竞争，因为中国的产能扩张面临美国可能对先进光刻设备实施出口限制带来的瓶颈。 报告预计，到 2030 年中国 DRAM 总产能将增至约 141 万片/月，其中长鑫单独可达 95 万片/月。一个关键的制约因素是依赖主要由 ASML 和尼康供应的先进浸没式 DUV 光刻设备；美国拟议的 MATCH 法案可能限制此类设备的对华出口，从而可能阻碍短期的扩产计划。

telegram · zaihuapd · Jul 16, 02:30

**背景**: DRAM（动态随机存取存储器）是一种易失性存储器，用作计算机、智能手机和服务器的内存。全球 DRAM 市场目前由三家公司主导：韩国的三星和 SK 海力士，以及美国的美光。浸没式 DUV（深紫外）光刻是制造先进半导体节点的关键技术；它在透镜和晶圆之间使用液体，以实现比传统“干式”光刻更高的分辨率，从而能够生产更先进的芯片。MATCH 法案是美国一项拟议的法案，旨在与盟友协调半导体出口管制，以限制中国获取先进芯片制造设备。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://tubex.chat/zh/article/match-7afb97">欧盟 制 裁中企+美国 MATCH ... - TubeX.Chat AI</a></li>
<li><a href="https://pdf.dfcfw.com/pdf/H3_AP202309081598093079_1.pdf">DUV 光 学透镜</a></li>
<li><a href="https://gaohaojun.cn/Blog/2026/01/21/红色内存潮流长鑫存储的战略分析和围绕DRAM的地缘政治斗争/">内 存 的赤色潮流： 长 鑫 存 储 （ CXMT ）的战略分析和围绕 DRAM ...</a></li>

</ul>
</details>

**标签**: `#Semiconductors`, `#DRAM`, `#Supply Chain`, `#Geopolitics`, `#Manufacturing`

---