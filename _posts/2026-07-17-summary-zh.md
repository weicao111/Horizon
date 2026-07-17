---
layout: default
title: "Horizon Summary: 2026-07-17 (ZH)"
date: 2026-07-17
lang: zh
---

> From 36 items, 6 important content pieces were selected

---

1. [Kimi K3 发布：具备 100 万上下文窗口的新型开源前沿 AI 模型，挑战西方顶级模型。](#item-1) ⭐️ 8.0/10
2. [Puter 将 Firefox 编译为 WebAssembly，使其能在另一个浏览器标签页内运行。](#item-2) ⭐️ 8.0/10
3. [Thinking Machines Lab 发布 Inkling，一个拥有 9750 亿参数、采用 Apache 2.0 许可的开放权重多模态 AI 模型。](#item-3) ⭐️ 8.0/10
4. [日本计划购买 2.75 万块英伟达 Rubin 芯片，打造机器人主权 AI 数据中心](#item-4) ⭐️ 8.0/10
5. [台积电再投千亿美元赴美建厂，AI 热潮驱动下 Q2 利润飙升 77%创新高。](#item-5) ⭐️ 8.0/10
6. [特斯拉在北美启动无方向盘自动驾驶汽车 Cybercab 的量产。](#item-6) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Kimi K3 发布：具备 100 万上下文窗口的新型开源前沿 AI 模型，挑战西方顶级模型。](https://www.kimi.com/blog/kimi-k3) ⭐️ 8.0/10

Moonshot AI 发布了其迄今为止最强大的模型 Kimi K3，该模型拥有 2.8 万亿参数和 100 万 token 的上下文窗口。该模型以开源权重形式发布，定价为每百万输入 token 3 美元，每百万输出 token 15 美元。 此次发布标志着中国模型在全球前沿模型竞争中的一次重大进展，直接挑战 Claude 和 GPT-4 等西方顶级模型。其开源权重和高性能可能会加速高级 AI 能力的商品化，影响全球 AI 战略和定价格局。 基准测试表明，Kimi K3 的性能与 Fable 或 Sol 等模型相当，在许多方面超越了 GPT-4 Opus。然而，对于一款来自中国的开源权重模型，其定价明显偏高，与 Anthropic 的 Sonnet 系列定价相近。

hackernews · vincent_s · Jul 16, 14:46 · [社区讨论](https://news.ycombinator.com/item?id=48935342)

**背景**: '开源权重' AI 模型是指将训练好的模型参数（权重）公开，允许用户在自己的硬件上下载、运行和研究该模型。100 万 token 的上下文窗口使得模型能够在单个提示中处理和推理极长的文档或对话，这种能力此前仅限少数前沿模型具备。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://hai.stanford.edu/ai-definitions/what-is-an-open-weight-model">What is an Open-Weight Model? - Stanford HAI</a></li>
<li><a href="https://medium.com/@prashantsahdev/the-1-million-token-context-window-a-game-changer-or-a-computational-challenge-2fb9320ef800">The 1 Million Token Context Window : A Game Changer or... | Medium</a></li>
<li><a href="https://artificialanalysis.ai/models/comparisons/kimi-k2-vs-gpt-4">Kimi K2 vs GPT-4: Model Comparison - artificialanalysis.ai</a></li>

</ul>
</details>

**社区讨论**: 社区进行了深入的技术和战略分析。讨论重点包括该模型针对特定任务的高成本，辩论中国实验室是否在战略性地将 AI 智能商品化以利于硬件销售，并分析了其性能基准，认为它已跻身顶级竞争者行列。

**标签**: `#artificial-intelligence`, `#large-language-models`, `#open-source`, `#ai-competition`, `#machine-learning`

---

<a id="item-2"></a>
## [Puter 将 Firefox 编译为 WebAssembly，使其能在另一个浏览器标签页内运行。](https://simonwillison.net/2026/Jul/16/firefox-in-webassembly/#atom-everything) ⭐️ 8.0/10

Puter 公司成功将 Firefox 浏览器（特别是其 Gecko 引擎）编译为 WebAssembly，使得整个浏览器可以作为沙盒应用在另一个浏览器标签页内运行。该项目据称使用了价值约 25,000 美元的 Claude Opus 和 Fable 模型 AI 算力，并通过在 Chrome 中运行的 WebAssembly 版 Firefox 实例内加载一个实时博客页面来演示这一成果。 这一成就是一个重要的技术里程碑，它突破了 WebAssembly 的边界，展示了其在 Web 沙箱内安全运行像整个浏览器引擎这样复杂的、原生级应用的潜力。它为新颖的 Web 应用、高级的浏览器内虚拟化以及软件在 Web 上的分发与隔离新范式开辟了可能性。 该演示要求所有网络流量通过 Wisp 协议经由 WebSocket 连接，通过 Puter 的服务器进行代理，这是由于浏览器对任意网络连接的限制所必需的。虽然 Puter 声称对 HTTPS 流量支持端到端加密，但项目对服务器端代理的依赖导致在流量高峰（例如在 Hacker News 上被讨论时）基础设施成本增加。

rss · Simon Willison · Jul 16, 23:34

**背景**: WebAssembly (Wasm) 是一种低级的二进制指令格式，设计为 C/C++ 和 Rust 等高级语言的便携式编译目标，使它们能在 Web 浏览器的安全沙箱内以接近原生的速度运行。Gecko 引擎是驱动 Firefox 浏览器的核心渲染和 JavaScript 引擎。Wisp 协议是一种低开销的规范，用于在单个 WebSocket 连接上隧道传输多个 TCP 和 UDP 套接字，在这类旨在规避浏览器网络限制的项目中非常有用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/MercuryWorkshop/wisp-protocol">GitHub - MercuryWorkshop/ wisp - protocol : Wisp is a low-overhead...</a></li>
<li><a href="https://www.anthropic.com/claude/opus">Claude Opus \ Anthropic</a></li>
<li><a href="https://www.anthropic.com/claude/fable">Claude Fable \ Anthropic</a></li>

</ul>
</details>

**标签**: `#WebAssembly`, `#Firefox`, `#Browser`, `#Systems`, `#Compilation`

---

<a id="item-3"></a>
## [Thinking Machines Lab 发布 Inkling，一个拥有 9750 亿参数、采用 Apache 2.0 许可的开放权重多模态 AI 模型。](https://simonwillison.net/2026/Jul/16/inkling/#atom-everything) ⭐️ 8.0/10

由 Mira Murati 领导的 Thinking Machines Lab 发布了其首个开放权重模型 Inkling，这是一个拥有 9750 亿总参数（410 亿活跃参数）的专家混合（Mixture-of-Experts）Transformer 模型。它是一个在 45 万亿个文本、图像、音频和视频 token 上训练的多模态模型，并采用宽松的 Apache 2.0 许可证发布。 此次发布意义重大，因为它引入了一个来自美国实验室的、具有商业友好许可的大规模开放权重模型，增强了开放 AI 生态系统，并为 NVIDIA Nemotron 和 Gemma 4 等其他主要开放模型提供了一个可行的替代选择。其多模态能力和 Apache 2.0 许可证使其成为微调和商业应用的强大基础模型。 该模型并未定位为前沿模型，而是作为通过该实验室的 Tinker 训练平台进行定制的强大基础模型。随附的模型卡和训练数据文档异常简短，后者仅说明数据来自公共互联网和第三方。一个更小的 2760 亿参数版本（Inkling-Small）已承诺发布但尚未推出。

rss · Simon Willison · Jul 16, 15:35

**背景**: '专家混合'（Mixture-of-Experts，MoE）Transformer 架构引入了稀疏性，允许模型扩展到巨大的总参数量，同时仅为每个输入激活一个子集，从而使训练和推理的计算效率更高。'开放权重'模型在某个许可证下发布模型训练好的参数（权重），这不同于'开源'模型，后者还包括训练代码、数据集和完整文档。Apache 2.0 许可证是一种宽松的开源许可证，允许商业使用、修改和分发，并包含明确的专利授权。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mixture_of_experts">Mixture of experts - Wikipedia</a></li>
<li><a href="https://neysa.ai/blog/open-weights-open-source/">Open Weights vs Open Source: What’s the Real Difference?</a></li>
<li><a href="https://www.mindstudio.ai/blog/gemma-4-apache-2-license-commercial-use">What Is Gemma 4's Apache 2.0 License? Why It Matters More Than the Model Itself | MindStudio</a></li>

</ul>
</details>

**标签**: `#AI`, `#Open Source`, `#Machine Learning`, `#Multimodal Models`

---

<a id="item-4"></a>
## [日本计划购买 2.75 万块英伟达 Rubin 芯片，打造机器人主权 AI 数据中心](https://www.bloomberg.com/news/articles/2026-07-16/japan-to-buy-nvidia-rubin-chips-to-build-sovereign-ai-for-robots) ⭐️ 8.0/10

日本计划购买 2.75 万块英伟达下一代 Rubin 芯片，由新成立的 Noetra 公司牵头建设一个主权 AI 数据中心。该项目获得日本政府 3.87 万亿日元（约合 240 亿美元）的拨款，旨在开发面向机器人的本土基础模型，首个 AI 模型计划于明年 3 月发布。 此举是日本在 AI 和机器人领域建立技术主权、减少对外国（主要是美国和中国）技术依赖的重大战略举措。它旨在使日本在全球机器人市场竞争中占据重要份额，目标是到 2040 年占据 30%以上的市场，并寻求在全球 AI 格局中创造'第三种选择'。 该项目的联盟包括软银、丰田支持的 Preferred Networks 和 NEC 等日本主要企业。其明确目标是在几年内开发出机器人专用的基础模型版本，整个倡议被定位为对抗美国和中国 AI 主导地位的地缘政治替代方案。

telegram · zaihuapd · Jul 16, 10:59

**背景**: 英伟达的 Rubin 平台是其下一代 AI 超级计算架构，作为 Blackwell 的继任者发布，包含六种新芯片，设计为一个集成系统协同工作。主权 AI 指的是一个国家开发和控制其自身的 AI 基础设施、数据和模型的能力，以确保安全、治理和经济独立性。机器人基础模型是大规模预训练的 AI 模型，旨在为机器人提供跨不同任务和环境的广泛泛化能力，超越了传统的单一任务模型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Rubin_(microarchitecture)">Rubin (microarchitecture) - Wikipedia</a></li>
<li><a href="https://stlpartners.com/articles/data-centres/sovereign-ai/">Sovereign AI: What it is, country playbooks & data centre strategy (2025)</a></li>
<li><a href="https://arxiv.org/abs/2604.15395">[2604.15395] Foundation Models in Robotics: A Comprehensive ... T-RO Special Issue on Foundation Models for Robotics - IEEE ... Awesome Robot Foundation Models 2025–2026 - GitHub T-RO Special Issue on Foundation Models for Robotics Foundation models in robotics: Applications, - NSF Public Access</a></li>

</ul>
</details>

**标签**: `#AI Hardware`, `#Sovereign AI`, `#Robotics`, `#Industrial Policy`, `#NVIDIA`

---

<a id="item-5"></a>
## [台积电再投千亿美元赴美建厂，AI 热潮驱动下 Q2 利润飙升 77%创新高。](https://www.reuters.com/world/asia-pacific/tsmcs-second-quarter-profit-seen-hitting-record-ai-boom-2026-07-15/) ⭐️ 8.0/10

台积电宣布将再向美国亚利桑那州投资 1000 亿美元建厂，大幅扩大了其在美总投资规模。公司同时公布第二季度净利润同比飙升 77%，达到 7066 亿新台币（约 220 亿美元），创下历史新高并远超市场预期，并将 2026 年资本支出预测上调至 600 亿至 640 亿美元。 这项巨额投资标志着先进半导体制造正战略性回流美国，旨在地缘政治紧张局势下增强供应链韧性。创纪录的利润和增加的支出突显了台积电在全球 AI 热潮中的关键作用，其尖端芯片对于训练和运行大型 AI 模型至关重要。 新的投资可能为亚利桑那州带来约 4 座新工厂，该州目前已有 8 座工厂在建或规划中。台积电还预计其全年美元营收将增长略超 40%，这反映了对其用于 AI 芯片的先进制程节点的强劲需求。

telegram · zaihuapd · Jul 16, 12:29

**背景**: 台积电（台湾积体电路制造公司）是全球最大的芯片代工厂，为英伟达和苹果等公司生产半导体。半导体制造厂（晶圆厂）是高度专业化、资本密集型的工厂，用于在先进制程节点（如 3 纳米、2 纳米）上制造集成电路。全球半导体供应链历来是地理专业化的，但近期的脆弱性促使各方努力实现生产地点的多元化。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.taipeitimes.com/News/front/archives/2026/07/17/2003860881">TSMC lifts capex above US$64bn as AI use rises - Taipei Times</a></li>
<li><a href="https://finance.yahoo.com/markets/article/tsmc-raises-capex-and-revenue-forecast-highlighting-growing-ai-chip-demand-113101950.html">TSMC raises capex and revenue forecast, highlighting growing AI chip demand</a></li>
<li><a href="https://www.semiconductors.org/strengthening-the-global-semiconductor-supply-chain-in-an-uncertain-era/">Strengthening the Global Semiconductor Supply Chain in an Uncertain Era - Semiconductor Industry Association</a></li>

</ul>
</details>

**标签**: `#Semiconductors`, `#Artificial Intelligence`, `#Manufacturing`, `#Global Economy`, `#Supply Chain`

---

<a id="item-6"></a>
## [特斯拉在北美启动无方向盘自动驾驶汽车 Cybercab 的量产。](https://t.me/zaihuapd/42621) ⭐️ 8.0/10

特斯拉宣布，其专用自动驾驶汽车 Cybercab 已在北美启动量产。这款车型取消了方向盘、踏板和后视镜，整车架构和交互方式均为无人驾驶场景定制，是特斯拉推进 Robotaxi 业务的重要一步。 此举标志着特斯拉对专用、全自动驾驶汽车设计的重大投入，将加速从改装车向专用 Robotaxi 的转变。这可能通过提供自动驾驶网约车新商业模式来重塑城市交通，影响竞争对手和监管讨论。 Cybercab 是一款全新设计的车型，由车载 AI 直接接管行驶控制，取消了传统手动操控装置。然而，该公告未透露具体产量、部署时间表、传感器配置或自动驾驶系统的运行设计域（ODD）等细节。

telegram · zaihuapd · Jul 17, 03:06

**背景**: Robotaxi 是指用于商业网约车服务的自动驾驶汽车，是自动驾驶出行领域的关键商业模式。SAE 驾驶自动化等级定义了自动驾驶系统的能力，其中 Level 5 代表在所有条件下实现完全自动化。稳健的自动驾驶系统通常依赖于多传感器融合，即整合来自摄像头、激光雷达和雷达的数据，以实现可靠的感知。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://appscrip.com/blog/robotaxi-business-model/">The Robotaxi Business Model: A Comprehensive Guide for 2025</a></li>
<li><a href="https://www.tommerritt.com/about-levels-of-driving-automation/">About Levels of Driving Automation – Tom Merritt .com</a></li>
<li><a href="https://www.mdpi.com/1424-8220/25/19/6033">A Review of Multi-Sensor Fusion in Autonomous Driving - MDPI</a></li>

</ul>
</details>

**标签**: `#autonomous-vehicles`, `#tesla`, `#robotics`, `#transportation`, `#ai`

---