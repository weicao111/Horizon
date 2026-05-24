---
layout: default
title: "Horizon Summary: 2026-05-24 (ZH)"
date: 2026-05-24
lang: zh
---

> From 20 items, 4 important content pieces were selected

---

1. [英特尔 80386 处理器微码被成功反汇编与分析](#item-1) ⭐️ 8.0/10
2. [从第一性原理出发的深度学习性能优化基础指南（2022 年）](#item-2) ⭐️ 8.0/10
3. [苹果开源 corecrypto 密码库，附带量子安全算法的形式化验证证明](#item-3) ⭐️ 8.0/10
4. [微软财报意外披露 OpenAI 单季度巨亏约 115 亿美元。](#item-4) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [英特尔 80386 处理器微码被成功反汇编与分析](https://www.reenigne.org/blog/80386-microcode-disassembled/) ⭐️ 8.0/10

一篇博客文章详细介绍了对英特尔 80386 处理器微码的成功反汇编与分析，该工作基于 Ken Shirriff 提供的芯片微码 ROM 的高分辨率图像。其输出是一个文本文件，以一种新的方言表示了微码指令。 这是一项重要的逆向工程成就，它深入揭示了基础 x86 CPU 的内部运作机制，有助于计算机架构历史研究和保存。这项工作也催生了像 z386 这样的项目，该项目旨在围绕原始微码构建一个开源的 80386 实现。 此次反汇编是针对 80386 的某个特定修订版进行的，需要注意的是，该处理器在其 22 年的生产周期中经历了许多微小的改动。该过程涉及分析芯片裸片图像来重建微码，而非对整个晶体管级电路进行建模。

hackernews · nand2mario · May 23, 12:11 · [社区讨论](https://news.ycombinator.com/item?id=48247004)

**背景**: 微码是 CPU 内部的一种低级固件层，它将复杂的机器指令翻译成硬件可以直接执行的更简单的微操作。在现代 x86 处理器中，微码通常处理复杂和专用的指令，并且可以通过操作系统进行更新。逆向工程微码涉及提取和破译这种专有的、处理器特定的代码，以理解其语义和内部工作原理。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.reenigne.org/blog/80386-microcode-disassembled/">80386 microcode disassembled - Reenigne blog</a></li>
<li><a href="https://wiki.gentoo.org/wiki/Microcode">Microcode - Gentoo wiki</a></li>
<li><a href="https://arxiv.org/abs/1910.00948">[1910.00948] Reverse Engineering x86 Processor Microcode Reverse engineering x86 processor microcode | Proceedings of ... Reverse Engineering x86 Processor Microcode GitHub - RUB-SysSec/Microcode: Microcode Updates for the ... CustomProcessingUnit: Reverse Engineering and Customization ... CustomProcessingUnit: Reverse Engineering and Customization ...</a></li>

</ul>
</details>

**社区讨论**: Hacker News 上的讨论显示出很高的参与度，用户们对从芯片裸片图像中提取微码的技术过程表示着迷，并对所使用的具体处理器修订版感到好奇。讨论还提到了相关的项目（如 z386）以及学习微编程的资源。

**标签**: `#reverse-engineering`, `#computer-architecture`, `#microcode`, `#x86`, `#hardware`

---

<a id="item-2"></a>
## [从第一性原理出发的深度学习性能优化基础指南（2022 年）](https://horace.io/brrr_intro.html) ⭐️ 8.0/10

2022 年，Horace 发表了一篇题为《从第一性原理出发让深度学习“飞速”运行》的深度技术指南，阐述了优化深度学习性能的核心硬件与软件原理。该指南分解了计算、内存带宽和延迟等概念，以说明如何在现代 GPU 上实现最大吞吐量。 这份指南很重要，因为它提供了对性能瓶颈的基础性理解，这对于研究人员和工程师高效训练和部署日益庞大的模型至关重要。它强调了软硬件协同设计的关键作用，并通过这些领域的持续改进，解释了英伟达在 AI 硬件领域保持领先地位的原因。 该指南强调，实现峰值性能需要平衡计算（例如来自 CUDA 核心和张量核心的 TFLOPS）与内存带宽，因为后者常常成为限制因素。它还讨论了内核融合和混合精度训练等实用优化技术，以更好地利用硬件能力。

hackernews · tosh · May 23, 11:50 · [社区讨论](https://news.ycombinator.com/item?id=48246889)

**背景**: 深度学习性能严重依赖 GPU 等并行处理硬件。英伟达的 GPU 使用 CUDA 核心进行通用并行计算，并使用专门的张量核心来加速 AI 基础性的矩阵运算。混合精度训练是一种使用较低精度（如 FP16）算术来加速计算并减少内存使用的技术，同时通过精心的缩放来保持模型精度。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/CUDA">CUDA - Wikipedia</a></li>
<li><a href="https://arxiv.org/abs/1710.03740">[1710.03740] Mixed Precision Training</a></li>
<li><a href="https://docs.nvidia.com/deeplearning/performance/mixed-precision-training/index.html">Train With Mixed Precision - NVIDIA Docs</a></li>

</ul>
</details>

**社区讨论**: 社区评论称赞这篇文章是经典且富有洞察力的资源，强调了英伟达在硬件方面显著且持续的竞争优势。一些用户指出了在不同运行时和硬件目标上进行性能优化的实际复杂性和缺乏可移植性，将其描述为“巨大的混乱”。其他人则讨论了文章中提出的具体技术细节，例如 Python 操作中的性能怪象。

**标签**: `#deep-learning`, `#performance`, `#gpu`, `#systems`, `#optimization`

---

<a id="item-3"></a>
## [苹果开源 corecrypto 密码库，附带量子安全算法的形式化验证证明](https://security.apple.com/blog/formal-verification-corecrypto/) ⭐️ 8.0/10

苹果于 5 月 22 日开源了其 corecrypto 库，提供了经过形式化验证的、符合 NIST 标准的量子安全算法 ML-KEM 和 ML-DSA 的实现。此次发布包含了端到端的形式化验证数学证明，以及供独立专家评估的定制验证工具和 Isabelle 理论库。 此举极大地提升了依赖 corecrypto 进行基础加密运算的超过 25 亿台活跃苹果设备的安全透明度和可信度。通过开源经过形式化验证的后量子密码学实现，苹果为软件保障设立了高标准，并为推动更广泛的软件安全领域发展贡献了关键工具。 形式化验证证明确保了 C 语言代码和手工优化的 ARM64 汇编实现均严格符合 NIST 标准。来自 corecrypto 的量子安全密码学已部署于 iMessage、VPN 等服务中。

telegram · zaihuapd · May 23, 04:49

**背景**: Corecrypto 是苹果在其操作系统中使用的基础、底层密码库，被 Security 和 CryptoKit 等框架所依赖。ML-KEM（FIPS 203）和 ML-DSA（FIPS 204）是 NIST 标准化的后量子密码算法，旨在抵御未来量子计算机的攻击，分别用于密钥交换和数字签名。形式化验证使用数学证明技术，常借助 Isabelle 等定理证明器工具，来严格证明软件代码正确实现了其规范。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/apple/corecrypto">GitHub - apple/corecrypto: Apple corecrypto · GitHub</a></li>
<li><a href="https://security.apple.com/blog/formal-verification-corecrypto/">A blueprint for formal verification of Apple corecrypto - Apple Security Research</a></li>
<li><a href="https://myitbasics.com/post-quantum-algorithms-ml-kem-ml-dsa-guide/">PQC Algorithms: ML-KEM vs ML-DSA Guide | Part 2 of 6</a></li>
<li><a href="https://en.wikipedia.org/wiki/Isabelle_(proof_assistant)">Isabelle (proof assistant) - Wikipedia</a></li>

</ul>
</details>

**标签**: `#cryptography`, `#formal-verification`, `#quantum-computing`, `#open-source`, `#security`

---

<a id="item-4"></a>
## [微软财报意外披露 OpenAI 单季度巨亏约 115 亿美元。](https://t.me/zaihuapd/41537) ⭐️ 8.0/10

微软最新财报显示，其采用权益法核算对 OpenAI 的投资，导致单季度净利润减少了 31 亿美元。根据微软持有约 27%的股权推算，OpenAI 该季度净亏损约 115 亿美元，这一亏损规模是其上半年 43 亿美元营收的近三倍。 此次披露罕见且可信地揭示了尖端 AI 开发所需的惊人“烧钱速度”，挑战了关于行业领先者近期盈利能力的假设。它凸显了 AI 竞赛巨大的资本密集性，并在实现正向现金流之前，对这种重投资商业模式的长期可持续性提出了疑问。 亏损估算是基于权益法会计原则，即投资者按持股比例确认被投资方的损益。若按税前损失和微软 32.5%的实际持股比例计算，隐含的亏损可能超过 120 亿美元。微软目前已向 OpenAI 投入 116 亿美元，占其 130 亿美元承诺投资额的绝大部分。

telegram · zaihuapd · May 23, 07:40

**背景**: 权益法是一种会计方法，适用于投资者对被投资方具有重大影响但未形成控制的情况（通常持股比例在 20%至 50%之间）。采用此法时，投资者需按其持股比例确认被投资方的净损益，并计入自身的利润表。OpenAI 是一家领先的 AI 研究和部署公司，以 ChatGPT 等产品闻名，微软是其最大的投资者和战略云合作伙伴。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://kpmg.com/cn/zh/home/insights/2024/09/business-combinations-ed-ias28.html">应用权益法 - 毕马威中国</a></li>
<li><a href="https://www.forbes.com/sites/paulocarvao/2026/05/21/anthropic-openai-enterprise-ai-profitability/">OpenAI And Anthropic Are Testing Two Very Different AI Business Models</a></li>

</ul>
</details>

**标签**: `#OpenAI`, `#Microsoft`, `#AI Economics`, `#Corporate Finance`, `#Tech Investment`

---