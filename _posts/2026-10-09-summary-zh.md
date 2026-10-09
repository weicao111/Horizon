---
layout: default
title: "Horizon Summary: 2026-10-09 (ZH)"
date: 2026-10-09
lang: zh
---

> From 29 items, 4 important content pieces were selected

---

1. [OpenAI 撤回三项 AI 生成的数学成果，凸显验证挑战。](#item-1) ⭐️ 8.0/10
2. [OpenAI API 为 GPT-6.1 Sol 模型新增 Ultrafast 模式，速度最高提升约 8 倍。](#item-2) ⭐️ 8.0/10
3. [SpaceX 拟收购覆盖全美的低频段频谱许可证，为 Starlink Mobile 铺路](#item-3) ⭐️ 8.0/10
4. [中国天眼 FAST 发现首个包含脉冲星的原生三体系统](#item-4) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [OpenAI 撤回三项 AI 生成的数学成果，凸显验证挑战。](https://twitter.com/danintheory/status/2108065033070789090) ⭐️ 8.0/10

OpenAI 已从其公开的 'math' 代码库中撤回了三项数学成果，相关记录可在其版本历史中查看。这一行动是在发现 AI 生成的证明存在问题后采取的，引发了关于自动定理证明可靠性的讨论。 这一事件凸显了验证 AI 生成的数学证明正确性所面临的重大挑战，这是 AI 辅助研究的一个关键前沿领域。随着 AI 系统越来越多地用于复杂推理任务，它引发了关于科学严谨性以及建立强大验证框架必要性的关键问题。 撤回记录在代码库的历史文件中，其中列出了诸如撤回特定论文和修复错误等变更。社区讨论表明，并非代码库中的所有成果都使用了 Lean 等工具进行形式化验证，其中混合了已验证和未验证的内容。

hackernews · sashank_1509 · Oct 8, 07:05 · [社区讨论](https://news.ycombinator.com/item?id=50002650)

**背景**: 自动定理证明（ATP）是一个使用计算机程序来生成数学陈述的形式化证明的子领域。形式化验证则应用数学上的严谨性，来证明一个系统（如 AI 模型的输出）在定义的约束下永远不会违反特定属性。OpenAI 等机构已开发出能够生成数学证明的 AI 模型（如 GPT-f），推动了机器辅助推理的边界。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Automated_theorem_proving">Automated theorem proving</a></li>
<li><a href="https://predictablemachines.com/blog/formal-verification-in-ai-and-why-it-matters/">Formal Verification in AI and Why It Matters | Predictable Machines</a></li>
<li><a href="https://www.deeplearning.ai/the-batch/the-proof-is-in-the-network">A Transformer Model that Generates Mathematical Proofs</a></li>

</ul>
</details>

**社区讨论**: 社区评论对完全由 AI 生成的证明的可靠性表示怀疑，指出即使在 Lean 等系统中经过形式化验证的证明，也可能在意图上存在细微错误。有人将此过程比作具有版本发布和补丁的软件工程，另一些人则质疑验证过程本身，想知道这些错误是由人类数学家发现的还是由另一个 AI 模型发现的。

**标签**: `#AI-Research`, `#Formal-Verification`, `#Mathematics`, `#OpenAI`, `#Scientific-Integrity`

---

<a id="item-2"></a>
## [OpenAI API 为 GPT-6.1 Sol 模型新增 Ultrafast 模式，速度最高提升约 8 倍。](https://developers.openai.com/api/docs/changelog) ⭐️ 8.0/10

OpenAI 在其 Responses API (v1/responses) 中为 GPT-6.1 Sol 模型推出了一个名为 Ultrafast 的最快服务层级，其生成速度相比 Standard 层级最高可提升约 8 倍。该新层级对所有 API 用户开放，价格是 Standard 层级的 6 倍，短上下文场景下，输入 token 价格约为每百万 12 美元，缓存输入 token 每百万 0.60 美元，输出 token 每百万 60 美元。 此举意义重大，因为它为构建对延迟敏感的应用（如实时聊天机器人、交互式智能体或复杂工作流自动化）的开发者提供了一个关键工具，可以大幅降低响应时间。这反映了行业提供分层性能选项的更广泛趋势，允许开发者根据其具体应用需求，在成本和速度之间进行权衡。 Ultrafast 模式是 Responses API 的一部分，该 API 专为有状态的交互设计，并能利用内置工具。显著的提速伴随着高昂的成本溢价，这使其成为那些延迟是主要约束且预算允许的特定用例的专业选择。

telegram · zaihuapd · Oct 9, 00:00

**背景**: GPT-6.1 Sol 是 OpenAI GPT-6 Sol 系列中的一个高效推理模型，专为复杂问题解决、软件工程和知识工作而设计。OpenAI Responses API (v1/responses) 是一个用于与模型创建有状态交互的端点，允许将先前响应的输出用作输入，并通过文件搜索、网络搜索等工具扩展能力。API 定价通常基于 token 使用量，输入、输出以及有时缓存 token 的费率是分开的。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/index/introducing-gpt-6-1-sol/">Introducing GPT-6.1 Sol | OpenAI</a></li>
<li><a href="https://developers.openai.com/api/reference/responses/overview">Responses Overview | OpenAI API Reference</a></li>
<li><a href="https://developers.openai.com/api/docs/pricing">Pricing | OpenAI API</a></li>

</ul>
</details>

**标签**: `#OpenAI`, `#API`, `#GPT-6`, `#AI-Services`, `#Performance`

---

<a id="item-3"></a>
## [SpaceX 拟收购覆盖全美的低频段频谱许可证，为 Starlink Mobile 铺路](https://x.com/SpaceX/status/2108291133025698301) ⭐️ 8.0/10

SpaceX 宣布已达成协议，拟收购一套覆盖全美的低频段频谱许可证组合，具体涉及 800 MHz 频段上高达 14 MHz 的成对频谱。公司计划将这批频谱与 Starlink 第二代（Gen2）卫星星座结合，以支持其 Starlink Mobile 服务在全国范围内提供高速移动宽带。 此举解决了一个关键的技术短板，使 Starlink Mobile 有望在室内和复杂环境中提供服务，从而将 SpaceX 定位为美国主要的移动网络运营商，直接与 AT&T、Verizon 等传统运营商竞争。这标志着向无处不在的卫星移动宽带迈出了重要一步，可能颠覆现有电信市场格局，并将连接扩展至偏远地区。 此次收购的频谱属于优质的 800 MHz 低频段，其价值在于强大的穿透建筑物能力和远距离传播特性，这有助于解决高频卫星信号的覆盖局限。交易对方是 Grain Management 公司，这批频谱将与即将部署的 Starlink 第二代（Gen2）星座整合，以增强 Starlink Mobile 服务。

telegram · zaihuapd · Oct 9, 01:04

**背景**: Starlink 是 SpaceX 的卫星互联网星座，为全球尤其是偏远地区提供宽带服务。低频段频谱（如 600-900 MHz）在电信领域备受青睐，因为其波长较长，与中频或高频频谱相比，能提供更好的覆盖范围和穿透障碍物的能力。Starlink Mobile 是一项旨在通过卫星提供直连手机（direct-to-cell）连接的服务，未来可能让标准智能手机无需专用硬件即可连接卫星网络。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cnbc.com/2026/10/08/spacex-spectrum-license-att-verizon-tmobile.html">SpaceX spectrum license hammers shares of AT&T ... - CNBC</a></li>
<li><a href="https://www.satellitetoday.com/connectivity/2026/10/08/spacex-moves-to-acquire-nationwide-low-band-spectrum-for-starlink-mobile/">SpaceX Moves to Acquire Nationwide Low-Band Spectrum for ...</a></li>

</ul>
</details>

**标签**: `#SpaceX`, `#Telecommunications`, `#Satellite Internet`, `#Spectrum`, `#Starlink`

---

<a id="item-4"></a>
## [中国天眼 FAST 发现首个包含脉冲星的原生三体系统](https://nao.cas.cn/news/gd/202610/t20261009_8289939.html) ⭐️ 8.0/10

中欧科学家独立确认，由中国天眼 FAST 发现的脉冲星 PSR J0435+3233 属于首例仍在演化阶段的原生三体系统。该系统由一颗脉冲星、一颗白矮星和一颗类太阳恒星组成，内外轨道周期分别为 8 天和 73.5 年，相关成果于 2026 年 10 月 9 日发表在《天体物理学杂志快报》上。 这一发现意义重大，因为它为研究多星系统中大质量恒星的复杂演化，特别是毫秒脉冲星的形成路径，提供了一个罕见且原始的天然实验室。它验证了等级三合星演化的理论模型，并展现了 FAST 望远镜高精度计时能力在揭示此类复杂宇宙系统方面的独特优势。 该系统位于银河系场中，而非致密星团内，这有力地支持了其作为从同一分子云中共同诞生的原生三体系统的起源。长达 73.5 年的外轨道周期，以及一颗类太阳恒星与一颗再循环脉冲星、一颗白矮星共存，使得该系统对于恒星演化研究而言异常罕见且信息丰富。

telegram · zaihuapd · Oct 9, 05:14

**背景**: 脉冲星是一种高度磁化的旋转中子星，从其磁极发射电磁辐射束，当辐射束扫过地球时，可以被观测到有规律的脉冲。原生三体系统指的是从同一气体云中共同诞生，并在整个演化过程中始终保持引力束缚的三颗恒星，这与后期通过动力学捕获形成的系统不同。中国的 500 米口径球面射电望远镜（FAST）是世界上最大的单口径射电望远镜，以其卓越的灵敏度著称，这对于探测微弱的脉冲星信号以及实现表征此类三体系统所需的精确计时测量至关重要。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/html/2608.01227">The PSR J0435+3233 Triple System</a></li>
<li><a href="https://en.wikipedia.org/wiki/Neutron_star">Neutron star - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Five-hundred-meter_Aperture_Spherical_Telescope">Five-hundred-meter Aperture Spherical Telescope - Wikipedia</a></li>

</ul>
</details>

**标签**: `#astronomy`, `#astrophysics`, `#pulsar`, `#FAST-telescope`, `#triple-system`

---