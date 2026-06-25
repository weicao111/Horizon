---
layout: default
title: "Horizon Summary: 2026-06-25 (ZH)"
date: 2026-06-25
lang: zh
---

> From 27 items, 6 important content pieces were selected

---

1. [OpenAI 发布其首款定制 AI 推理芯片 'Jalapeno'，由 Broadcom 制造。](#item-1) ⭐️ 9.0/10
2. [Anthropic 指控阿里巴巴大规模非法提取 Claude AI 模型能力。](#item-2) ⭐️ 8.0/10
3. [高通宣布收购 AI 初创公司 Modular 及其 Mojo 编程语言](#item-3) ⭐️ 8.0/10
4. [台积电宣布对其所有先进制程（7 纳米及以下）代工价格上调 5%至 10%。](#item-4) ⭐️ 8.0/10
5. [Cloudflare 等科技巨头提议 PACT 协议，旨在用加密令牌替代验证码。](#item-5) ⭐️ 8.0/10
6. [美光科技公布 2026 财年 Q3 创纪录业绩，营收同比暴增 346%，AI 内存需求成主要驱动力](#item-6) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [OpenAI 发布其首款定制 AI 推理芯片 'Jalapeno'，由 Broadcom 制造。](https://techcrunch.com/2026/06/24/openai-unveils-its-first-custom-chip-built-by-broadcom/) ⭐️ 9.0/10

2026 年 6 月 24 日，OpenAI 宣布了其首款定制 AI 推理芯片，名为 'Jalapeno'，该芯片是与半导体设计合作伙伴 Broadcom 共同开发，并由台积电（TSMC）负责制造。 这标志着 OpenAI 的重大战略转变，从依赖 NVIDIA GPU 等第三方硬件转向开发自己的专用芯片，此举可能显著提升其 AI 模型的运行性能和成本效益，并影响更广泛的 AI 硬件格局。 据报道，该芯片从设计到生产仅用了九个月，OpenAI 声称这一过程通过使用其自身的 AI 模型进行部分设计和优化而得以加速。它是一款专门的推理芯片，这意味着它针对运行已训练好的 AI 模型进行了优化，而非用于训练模型。

hackernews · jamdesk · Jun 24, 17:47 · [社区讨论](https://news.ycombinator.com/item?id=48663324)

**背景**: AI 芯片通常专门用于训练模型（需要高精度和大规模并行计算）或推理（运行已训练好的模型，通常优先考虑效率和低延迟）。Broadcom 是定制专用集成电路（ASIC）设计服务的领先提供商，该服务涉及为客户特定需求定制芯片。像谷歌（TPU）和 AWS（Inferentia）这样的公司也已开发定制 AI 芯片以获得性能和成本优势。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.brownstoneresearch.com/bleeding-edge/training-vs-inference/">Training vs . Inference - Brownstone Research</a></li>
<li><a href="https://www.broadcom.com/products/custom-silicon/asics">Application-specific Integrated Circuits (ASICs)</a></li>
<li><a href="https://aws.amazon.com/ai/machine-learning/inferentia/">AI Chip - Amazon Inferentia - AWS</a></li>

</ul>
</details>

**社区讨论**: 社区讨论凸显了技术上的好奇心和猜测。关键点包括：对 OpenAI 声称使用自家模型加速芯片设计过程的兴趣，但对其营销意义存在一些怀疑；澄清了台积电（TSMC）是制造合作伙伴；以及关于替代芯片架构的讨论，例如将权重烧录到 ROM 中以实现极致效率的架构，正如 Taalas 等初创公司所做的那样。

**标签**: `#artificial-intelligence`, `#hardware`, `#semiconductors`, `#openai`, `#machine-learning`

---

<a id="item-2"></a>
## [Anthropic 指控阿里巴巴大规模非法提取 Claude AI 模型能力。](https://www.reuters.com/world/china/anthropic-says-alibaba-illicitly-extracted-claude-ai-model-capabilities-2026-06-24/) ⭐️ 8.0/10

Anthropic 正式指控中国科技巨头阿里巴巴策划了一场大规模、未经授权的行动，以提取其 Claude AI 模型的能力，该公司称这是其历史上已知规模最大的蒸馏攻击。据称，该操作涉及中国经销商以大幅折扣提供 Claude API 访问权限，以补贴收集用户日志和推理轨迹，用作训练数据。 这一指控凸显了人工智能行业在知识产权和安全方面面临的重大挑战，模型提取攻击可能削弱专有 AI 系统的竞争优势和经济价值。它也突显了全球 AI 竞赛中不断升级的地缘政治和竞争紧张局势，获取先进模型能力是关键的战略资产。 据描述，这种提取方法是一种“蒸馏”操作，即用一个能力更强的模型的输出来训练一个能力较弱的模型。据报道，经销商通过共享账户、使用欺诈性支付方式以及向中国 AI 实验室转售模型输出和推理链，以低于官方价格 70-90% 的价格提供 Claude 代币。

hackernews · htrp · Jun 24, 19:48 · [社区讨论](https://news.ycombinator.com/item?id=48664814)

**背景**: 模型能力提取，或称模型蒸馏，是一种训练较小或能力较弱的模型来模仿更大、更复杂模型输出的技术。这可以通过黑盒方法（仅使用最终输出）或分析内部推理的更针对性方法来实现。像 Anthropic 这样的 AI 公司在开发其大语言模型 (LLM) 上投入巨大，此类提取攻击对其知识产权和商业模式构成直接威胁。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://cybersecuritynews.com/anthropic-accuses-alibaba/">Anthropic Accuses Alibaba of 'Illicitly' Accessing Its Claude AI Models ...</a></li>
<li><a href="https://creati.ai/ai-news/2026-06-25/anthropic-accuses-alibaba-illicitly-extracting-claude-ai-model-capabilities/">Anthropic Accuses Alibaba of Illicitly Extracting Claude AI Model ...</a></li>
<li><a href="https://beyondscale.tech/blog/ai-model-extraction-attacks-defense-guide">AI Model Extraction Attacks: Stop LLM Theft | BeyondScale</a></li>

</ul>
</details>

**社区讨论**: 社区情绪复杂，一些用户指出其中的讽刺意味：AI 公司在未经明确许可的情况下使用大量网络数据进行训练，现在却抱怨自己的模型被用于训练。另一些用户则认为，被指控的行为是科技行业中标准（尽管激进）的竞争做法，类似于逆向工程。讨论还深入探讨了不同蒸馏方法的技术细节。

**标签**: `#ai-ethics`, `#intellectual-property`, `#geopolitics`, `#large-language-models`, `#industry-competition`

---

<a id="item-3"></a>
## [高通宣布收购 AI 初创公司 Modular 及其 Mojo 编程语言](https://www.reuters.com/business/qualcomm-buy-ai-startup-modular-2026-06-24/) ⭐️ 8.0/10

高通宣布收购 AI 初创公司 Modular，该公司以开发 Mojo 编程语言和高性能编译器栈而闻名。据报道，这笔交易价值约 40 亿美元，于 2026 年 6 月 24 日公布。 此次收购是高通为增强其 AI 和边缘计算能力而采取的战略举措，旨在直接挑战英伟达在 AI 软件领域凭借 CUDA 栈建立的主导地位。这标志着高通希望超越移动芯片业务，成为面向大规模 AI 推理的全栈硬件和软件提供商。 Modular 的 Mojo 语言是一种基于 MLIR 编译器框架构建的、类似 Python 的专有系统编程语言，旨在面向 CPU、GPU 和 ASIC 等多种硬件。此次收购紧随近期基于 ARM 的超级计算机的兴起，也是高通更广泛技术组合构建的一部分，其中包括对 RISC-V 和其他 AI 技术的投资。

hackernews · timmyd · Jun 24, 13:49 · [社区讨论](https://news.ycombinator.com/item?id=48659798)

**背景**: Modular 是一家 AI 基础设施公司，由 LLVM 和 Swift 项目的关键创建者 Chris Lattner 创立。其旗舰产品 Mojo 编程语言旨在将 Python 的易用性与 C++或 Rust 的性能相结合，专为 AI 和高性能计算设计。该语言利用 MLIR 编译器框架，能高效地为各种硬件加速器生成代码，使其成为 AI 开发中替代英伟达 CUDA 生态系统的潜在选择。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mojo_(programming_language)">Mojo (programming language)</a></li>
<li><a href="https://mojolang.org/">Mojo</a></li>

</ul>
</details>

**社区讨论**: 社区情绪复杂，一些人对收购的时机感到意外，并对 Mojo 专注于 Python-like 语法提出质疑。另一些人则将此举与更广泛的行业转变联系起来，例如基于 ARM 的超级计算的兴起以及对 CUDA 替代方案的需求。一个值得注意的讨论点是其中存在的讽刺性，因为 Modular 过去曾批评硬件公司在构建成功的 AI 软件栈方面的失败。

**标签**: `#acquisitions`, `#artificial-intelligence`, `#compilers`, `#semiconductors`, `#edge-computing`

---

<a id="item-4"></a>
## [台积电宣布对其所有先进制程（7 纳米及以下）代工价格上调 5%至 10%。](https://36kr.com/newsflashes/3866472254411779) ⭐️ 8.0/10

台积电已陆续通知客户，将上调晶圆代工价格，涨价范围不仅包括市场传闻的 3 纳米制程，更扩大至 7 纳米及以下的所有先进制程。整体涨幅约为 5%至 10%，将影响其约 75%的晶圆营收来源。 此举意义重大，标志着台积电多年来最广泛、最强有力的定价行动，将直接增加依赖其先进芯片的各大科技公司（涉及 AI、智能手机和高性能计算领域）的成本。这一举措反映了先进半导体制造市场的巨大需求和定价权，可能影响全球下游电子和 AI 行业的成本结构与盈利能力。 此次涨价全面适用于 7 纳米及以下的制程节点，包括最新的 3 纳米技术。根据行业数据，截至 2026 年，台积电一片 300 毫米晶圆的成本在 28 纳米节点约为 3000 美元，在 3 纳米节点则高达约 19500 美元，这为此轮涨价的规模提供了背景参考。

telegram · zaihuapd · Jun 24, 05:45

**背景**: 在半导体制造中，“制程节点”（如 7 纳米、3 纳米）指的是芯片上最小特征的尺寸，数字越小代表技术越先进、晶体管密度越高、性能越强。台积电（台湾积体电路制造公司）是全球领先的专用半导体代工厂，为苹果、英伟达、AMD 等公司制造芯片。先进制程节点（通常指 7 纳米及以下）对于生产用于智能手机、AI 加速器和数据中心的最强大、最节能的处理器至关重要。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://siliconanalysts.com/data/wafer-pricing">Wafer Pricing by Process Node (2026) — $3,000 at 28nm to ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/7_nm_process">7 nm process - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/3_nm_process">3 nm process - Wikipedia</a></li>

</ul>
</details>

**标签**: `#semiconductors`, `#foundry`, `#supply-chain`, `#manufacturing`, `#tsmc`

---

<a id="item-5"></a>
## [Cloudflare 等科技巨头提议 PACT 协议，旨在用加密令牌替代验证码。](https://www.techtimes.com/articles/318891/20260623/cloudflare-chrome-firefox-plan-replace-captchas-cryptographic-tokens.htm) ⭐️ 8.0/10

6 月 22 日，Cloudflare 联合 Google Chrome、Mozilla Firefox、Microsoft Edge 和 Shopify 发起了一项跨行业倡议，旨在开发并推动一个名为“私有访问控制令牌”（PACT）的新网络协议成为标准。该协议旨在用保护隐私的加密令牌替代传统的验证码，让用户在一次验证后即可证明自己是人类，而无需泄露身份或浏览历史。 这项倡议意义重大，因为它解决了与验证码相关的普遍用户体验挫折和隐私担忧，验证码通常被认为是侵入性且耗时的。如果被采纳，PACT 可以为数十亿用户简化网络身份验证，减少合法流量的摩擦，并为区分人类和机器人设定一个以隐私为中心的新标准。 PACT 协议基于 IETF 的 Privacy Pass 标准，并利用盲签名技术来确保令牌的匿名性。然而，该提案仍处于早期阶段，关键的治理问题尚未解决，例如确定令牌发行方，并且苹果公司尚未加入该联盟。

telegram · zaihuapd · Jun 24, 06:30

**背景**: 验证码被广泛用于防止机器人滥用在线服务，但常因用户体验差和隐私风险而受到批评。Privacy Pass 是一个现有的 IETF 协议，它使用带有盲签名的加密令牌，允许用户证明他们之前已经解决过挑战，而无需透露是哪一个挑战或关联他们的活动。PACT 基于此概念，旨在创建一个更通用的验证码替代方案。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://hacks.mozilla.org/2026/06/pact-anonymous-credentials-for-the-web/">PACT: Anonymous Credentials for the Web - hacks.mozilla.org</a></li>
<li><a href="https://www.ietf.org/archive/id/draft-ietf-privacypass-protocol-16.html">Privacy Pass Issuance Protocol - Internet Engineering Task Force</a></li>
<li><a href="https://www.techtimes.com/articles/318891/20260623/cloudflare-chrome-firefox-plan-replace-captchas-cryptographic-tokens.htm">Cloudflare, Chrome, and Firefox Plan to Replace CAPTCHAs With Cryptographic Tokens</a></li>

</ul>
</details>

**标签**: `#Web Security`, `#Privacy`, `#Authentication`, `#Protocols`, `#CAPTCHA`

---

<a id="item-6"></a>
## [美光科技公布 2026 财年 Q3 创纪录业绩，营收同比暴增 346%，AI 内存需求成主要驱动力](https://www.globenewswire.com/news-release/2026/06/24/3317151/14450/en/micron-technology-inc-reports-record-results-for-the-third-quarter-of-fiscal-2026.html) ⭐️ 8.0/10

美光科技公布了 2026 财年第三季度财报，单季营收达到 414.6 亿美元，同比增长 346%，净利润为 282.4 亿美元，这主要受 AI 基础设施对高性能内存的爆发式需求驱动。公司还宣布 HBM4 已大规模量产，并预计 HBM4E 将于 2027 年投产。 这一创纪录的业绩突显了市场对先进内存芯片，尤其是对训练和运行大型 AI 模型至关重要的高带宽内存（HBM）的持续强劲需求。美光的出色表现和乐观预期标志着半导体行业的范式转变，凸显了内存已成为 AI 时代的关键瓶颈和增长引擎。 美光的 Non-GAAP 毛利率从去年同期的 39%飙升至 84.9%，其数据中心业务营收同比暴增 653%。公司已签署 16 份长期战略协议以锁定未来 3-5 年的订单，并预计内存紧缺将持续至 2027 年以后。

telegram · zaihuapd · Jun 24, 22:22

**背景**: 高带宽内存（HBM）是一种先进的 DRAM 技术，它通过硅通孔（TSV）技术将多个内存芯片垂直堆叠并高速互连，提供比传统内存高得多的带宽。这项技术对于 GPU 等 AI 加速器至关重要，因为它们需要快速访问数据来处理海量数据集。HBM4 是最新一代产品，而 HBM4E 是其增强版，提供更高的速度和带宽，预计在 2027 年左右推出。Non-GAAP 财务指标是对标准 GAAP 会计数据的调整，通常会排除一次性或非现金项目，以展示公司的核心运营绩效。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/High_Bandwidth_Memory">High Bandwidth Memory - Wikipedia</a></li>
<li><a href="https://www.ersaelectronics.com/blog/hbm4-hbm4e">HBM4 compared to HBM4E</a></li>
<li><a href="https://www.investopedia.com/articles/financial-analysis/062716/gaap-vs-nongaap-which-should-you-consider-evaluation.asp">GAAP vs. Non-GAAP: Key Differences Explained - Investopedia GAAP vs. Non-GAAP: Key Differences and SEC Rules Non-GAAP Financial Measures and Metrics - Deloitte What's the Difference Between GAAP vs. Non-GAAP? | The Motley ... Understanding Non GAAP vs GAAP: A Clear Guide to Financial ... GAAP vs. Non-GAAP (Definitions, Comparison and Examples) Non-GAAP Financial Measures - SEC.gov</a></li>

</ul>
</details>

**标签**: `#Semiconductors`, `#Financial Results`, `#AI Infrastructure`, `#Memory`, `#HBM`

---