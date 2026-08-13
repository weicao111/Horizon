---
layout: default
title: "Horizon Summary: 2026-08-13 (ZH)"
date: 2026-08-13
lang: zh
---

> From 34 items, 10 important content pieces were selected

---

1. [阿里通义千问团队开源 2.4 万亿参数 AI 模型 Qwen 3.8-Max。](#item-1) ⭐️ 9.0/10
2. [Zed 编辑器推出 Delta：面向 AI 智能体的实时协作环境](#item-2) ⭐️ 8.0/10
3. [Tailscale 将数据库损坏溯源至一个存在 16 年的 SQLite WAL 重置 bug](#item-3) ⭐️ 8.0/10
4. [AI 工具可能正在掏空中级软件工程师的角色](#item-4) ⭐️ 8.0/10
5. [蒂莫西·高尔斯分析大语言模型的数学能力优势与局限。](#item-5) ⭐️ 8.0/10
6. [马斯克宣布未来所有特斯拉车型将集成星链，Robotaxi Cybercab 率先搭载。](#item-6) ⭐️ 8.0/10
7. [企业级 SSD 占据 NAND 出货量 48%，长江存储首次跻身全球前三](#item-7) ⭐️ 8.0/10
8. [微信团队发布 WeLM 大语言模型家族，以资源效率为核心并采用 MoE 架构](#item-8) ⭐️ 8.0/10
9. [DeepSeek-V4-Flash 正式版 API 上线公测，性能大幅提升](#item-9) ⭐️ 8.0/10
10. [白宫拟扩大 AI 政策框架，将开源模型纳入发布前安全测试](#item-10) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [阿里通义千问团队开源 2.4 万亿参数 AI 模型 Qwen 3.8-Max。](https://t.me/zaihuapd/43151) ⭐️ 9.0/10

阿里通义千问团队正式发布并宣布开源 Qwen 3.8-Max 模型，其总参数量达 2.4 万亿，活跃参数为 950 亿，这是 Qwen 首次开源其 'Max' 级别的模型权重。该模型基于 Qwen 3.5 架构，在自主编码和任务执行方面表现出色，据称可自主运行超 10 天完成项目构建，并在 24 小时内参与竞赛。 此次发布是开源 AI 在规模和能力上的一次重大飞跃，拓展了公开可用模型的边界，并可能在自主软件开发和长期任务执行方面催生新的应用。它加剧了高端大语言模型领域的竞争，对 Kimi k3 和 DeepSeek V4-Pro 等前沿模型构成挑战，并可能让开发者和研究人员更容易获得最先进的 AI 性能。 该模型采用混合专家架构，总参数量 2.4 万亿，其中活跃参数为 950 亿；初始发布的模型权重为 BF16 和 FP8 精度，完整的 BF16 模型约需 4.9TB 存储空间。值得注意的是，当前开源的权重版本缺少官方版本中的一些功能，例如视觉输入支持和默认的 100 万上下文长度。

telegram · zaihuapd · Aug 12, 16:13

**背景**: Qwen 是阿里巴巴开发的大语言模型系列。Qwen 3.8-Max 所基于的 Qwen 3.5 架构采用了稀疏混合专家设计，在推理时只激活一部分参数（即'活跃'参数），这使得运行超大规模模型更加高效。在 AI 模型中，'参数'是训练过程中学习到的内部变量，而像 FP8（8 位浮点数）这样的精度格式被用来降低存储和运行这些模型所需的内存和计算成本。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://medium.com/data-science-in-your-pocket/qwen-3-5-explained-architecture-upgrades-over-qwen-3-benchmarks-and-real-world-use-cases-af38b01e9888">Qwen 3.5 Explained: Architecture, Upgrades Over Qwen ... - Medium</a></li>
<li><a href="https://0xbenzo.dev/blog/understanding-model-parameters/">Understanding Model Parameters: Total Parameters vs Active ...</a></li>
<li><a href="https://developer.nvidia.com/blog/floating-point-8-an-introduction-to-efficient-lower-precision-ai-training/">Floating-Point 8: An Introduction to Efficient, Lower-Precision AI Training | NVIDIA Technical Blog</a></li>

</ul>
</details>

**社区讨论**: 社区讨论聚焦于技术和实际考量，指出模型体积庞大且初期缺乏易于部署的量化版本，这可能限制其即时可用性。人们对模型宣称的性能感到兴奋，并将其与 Claude Opus 4.5 等模型比较，但也对部署成本以及开源权重版本缺少视觉等功能表示担忧。用户还将其与 Kimi k3、DeepSeek V4-Pro 等竞品模型进行比较，将其置于一个竞争激烈的格局中。

**标签**: `#Large Language Models`, `#Open Source AI`, `#Model Scaling`, `#Autonomous Agents`

---

<a id="item-2"></a>
## [Zed 编辑器推出 Delta：面向 AI 智能体的实时协作环境](https://zed.dev/blog/introducing-delta) ⭐️ 8.0/10

Zed 代码编辑器推出了名为 Delta 的新功能，它支持在编辑器内与 AI 智能体进行实时协作对话。该功能将代码和对话集成到一个统一的工作区，使开发者和 AI 能够无缝协作。 这一进展意义重大，因为它弥合了 AI 辅助编码工具与协作开发工作流之间的鸿沟，可能改变开发者与 AI 在代码审查、调试和指导等任务中的交互方式。它使 Zed 成为创建人机协作原生功能的多人协作环境的先驱。 Delta 基于名为 DeltaDB 的技术构建，该技术提供操作级版本控制，以保存 AI 智能体的所有见解并将其与代码关联。该功能不仅旨在促进人机协作，还支持诸如通过审查导致特定代码更改的对话历史来指导初级工程师等场景。

hackernews · khy · Aug 12, 18:19 · [社区讨论](https://news.ycombinator.com/item?id=49276574)

**背景**: Zed 是一款由 Atom 和 Tree-sitter 的创建者开发的高性能、多人协作代码编辑器。AI 编码智能体是一种可以自主编写、修改、调试和重构代码的软件工具，它超越了基本的代码补全，能够理解多文件上下文并执行多步骤任务。更广泛的趋势是将此类智能体深度集成到开发环境中以提高生产力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://shapeof.com/archives/2025/8/deltadb_from_zed.html">DeltaDB From Zed (the Code Editor) - shapeof.com</a></li>
<li><a href="https://aitoolly.com/ai-news/article/2026-08-13-zed-introduces-delta-a-new-multiplayer-environment-for-collaborative-coding-with-ai-agents-and-real">Zed Delta: Multiplayer Coding Environment for AI Agents</a></li>
<li><a href="https://agentic.ai/best/coding-agents">21 Best AI Coding Agents in 2026 — Agentic.ai</a></li>

</ul>
</details>

**社区讨论**: 社区情绪复杂，一些人质疑多人编辑对独立开发者的实用性，而另一些人则看到了 Delta 在指导工作和审查 AI 推理过程方面的价值。一个值得注意的担忧是 AI 生成的代码摘要可能冗长且不准确，不过该功能保存对话历史的能力被视为提高可追溯性的潜在解决方案。

**标签**: `#code-editors`, `#ai-assistants`, `#developer-tools`, `#collaboration`

---

<a id="item-3"></a>
## [Tailscale 将数据库损坏溯源至一个存在 16 年的 SQLite WAL 重置 bug](https://tailscale.com/blog/sqlite-wal-reset-bug) ⭐️ 8.0/10

Tailscale 详细说明了他们如何将控制平面中反复出现的数据库损坏事件，溯源至 SQLite 预写日志（WAL）检查点逻辑中一个潜伏的数据竞争条件。SQLite 开发者估计该 bug 已存在至少 16 年。该公司资助开发了一个开源的 SQLite VFS 垫片调试工具，该工具几乎立即帮助隔离了这个被命名为 'WAL-Reset bug' 的缺陷。 这一发现意义重大，因为它揭示了一个在 SQLite 这样基础且被广泛信任的数据库库中，长期隐藏的严重 bug，该 bug 可能导致已提交的事务消失，引发数据损坏。它凸显了复杂调试工具以及用户与开源维护者之间协作的极端重要性，这对于发现那些即使经过广泛测试也可能漏网的、基于竞争条件的复杂问题至关重要。 该 bug 是 WAL 模式下检查点操作与写入事务之间一种罕见的数据竞争，即使在单进程访问时也可能损坏数据库，这与 SQLite 在单写入者场景下安全的普遍假设相悖。在调查过程中，Tailscale 和 SQLite 开发者还发现了第二个与之无关的、与过时表达式索引相关的 bug。

hackernews · ropbear · Aug 12, 14:22 · [社区讨论](https://news.ycombinator.com/item?id=49272832)

**背景**: SQLite 是一个被广泛使用的、无服务器的、独立的 SQL 数据库引擎，被嵌入到无数应用程序中。其预写日志（WAL）模式是一个受欢迎的特性，它通过允许读操作与写操作并发进行来提高并发性。检查点是一个将 WAL 文件中的更改转移回主数据库文件的过程，以保持主文件大小可控。Tailscale 是一种零配置 VPN 服务，使用 SQLite 作为其控制平面的数据库。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://tailscale.com/blog/sqlite-wal-reset-bug">How Tailscale helped find the SQLite WAL-Reset bug</a></li>
<li><a href="https://antithesis.com/blog/2026/wal-reset-bug/">Breaking the WAL | Antithesis</a></li>
<li><a href="https://www.youngju.dev/blog/2026-07-16-sqlite-wal-reset-bug.en">The SQLite WAL - Reset Bug : A Data Corruption Race That Hid for 15...</a></li>

</ul>
</details>

**社区讨论**: 社区赞扬了这篇写得很好的技术深度文章以及该公司资助开源调试工具的举措。评论强调了尽管是单写入者设计，但对竞争条件如何具体发生感到兴趣，对基础软件工程的赞赏，以及对这类 bug 存在时间之长的反思。一位用户引用了 Dijkstra 关于测试只能证明 bug 存在而非其不存在的名言。

**标签**: `#sqlite`, `#databases`, `#debugging`, `#tailscale`, `#concurrency`

---

<a id="item-4"></a>
## [AI 工具可能正在掏空中级软件工程师的角色](https://blog.florianherrengt.com/ai-removing-middle-class-software-engineering.html) ⭐️ 8.0/10

一篇博客文章及其引发的高参与度讨论（743 分，679 条评论）探讨了一个假设：AI 驱动的开发工具正在自动化常规的中级编程任务。这一趋势被认为可能会减少对那些主要职责是将高级设计转化为代码的工程师的需求。 这预示着软件工程就业市场可能发生结构性转变，纯实现工作的价值下降，而系统设计、批判性思维和问题分解等高级技能的价值则被提升。这迫使科技行业的数百万从业者重新评估职业路径和技能发展。 讨论强调，AI 可能会自动化那些依赖搜索常见实现问题的“Stack Overflow 工程师”角色。一个关键的警告是，如果 AI 被缺乏积极性或技能不足的工程师使用，可能会放大不良实践，导致技术债增加。

hackernews · florianherrengt · Aug 12, 13:20 · [社区讨论](https://news.ycombinator.com/item?id=49271994)

**背景**: 大型语言模型（LLMs）已经发展到能够驱动智能编码助手，这些助手可以根据自然语言提示生成、解释和重构代码。这些工具正越来越多地被集成到开发环境（IDE）中，自动化代码合成和测试生成等任务。所谓“中级”工程角色，通常指专注于实现明确定义的规范、解决常见编码问题的职位，而非高级架构或创新研究。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://dl.acm.org/doi/10.1145/3715754">Demystifying LLM-Based Software Engineering Agents</a></li>
<li><a href="https://nmn.gl/blog/ai-midlevel-engineer">Is AI ready to be a mid-level engineer? | N’s Blog</a></li>
<li><a href="https://www.linkedin.com/pulse/mark-zuckerberg-bold-prediction-ai-replace-mid-level-software-bajaj-duxvc">Mark Zuckerberg Bold Prediction: AI to Replace Mid-Level ...</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍认同 AI 正在自动化常规的实现工作，将其比作“Stack Overflow 工程师的自动化”。大家一致认为批判性思维和理解 AI 生成代码的能力至关重要，并担心 AI 可能被缺乏积极性的工程师用来放大不良实践。一些人指出，“优秀”工程师的定义仍然是主观的，但所有人都强调需要仔细审查 AI 的输出。

**标签**: `#artificial-intelligence`, `#software-engineering`, `#future-of-work`, `#llm`, `#career`

---

<a id="item-5"></a>
## [蒂莫西·高尔斯分析大语言模型的数学能力优势与局限。](https://gowers.wordpress.com/2026/08/12/what-sort-of-maths-are-llms-good-at/) ⭐️ 8.0/10

数学家蒂莫西·高尔斯于 2026 年 8 月 12 日发表了一篇博客文章，系统性地探讨了大语言模型（LLMs）擅长和持续失败的具体数学问题类型。这篇文章引发了广泛讨论，超过 130 条评论围绕 AI 在形式化数学推理中的潜力和局限展开了辩论。 这项分析之所以重要，是因为它从专家视角细致地剖析了 AI 在数学领域当前的能力边界，这一领域正考验着机器的推理和创造力极限。理解这些能力与局限，对于指导未来 AI 辅助定理证明的研究，以及设定 AI 在数学发现中作用的现实预期至关重要。 高尔斯提出，LLMs 达到更高水平的一个关键标志，将是它们能够产生新颖、令人惊讶且优雅的证明，这些证明不易被偶然发现。讨论还指出，当前 AI 在数学上的成功通常涉及大量采样和搜索（如 AlphaCode）来寻找解或反例，而非进行深刻的演绎推理。

hackernews · ColinWright · Aug 12, 10:04 · [社区讨论](https://news.ycombinator.com/item?id=49270022)

**背景**: 大语言模型（LLMs）是在海量文本语料上训练、用于预测下一个词的 AI 系统，但它们在编码和解决数学谜题等任务上已显示出令人惊讶的能力。形式化推理和定理证明对 AI 来说是一个重大挑战，它要求超越模式匹配、具备逻辑严密性和正确性保证。该领域正在探索将 LLMs 与形式化验证系统（如 Lean 证明助手）相结合，以期将模型的启发式能力与符号化方法的可靠性结合起来。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://gowers.wordpress.com/">Gowers's Weblog | Mathematics related discussions</a></li>
<li><a href="https://cacm.acm.org/research/formal-reasoning-meets-llms-toward-ai-for-mathematics-and-verification/">Formal Reasoning Meets LLMs: Toward AI for Mathematics and Verification – Communications of the ACM</a></li>
<li><a href="https://en.wikipedia.org/wiki/Automated_reasoning">Automated reasoning - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 社区评论延伸了这一分析，指出 AI 当前的数学优势通常在于对例子或反例的暴力搜索，正如 AlphaCode 等项目所展现的。一位评论者链接了 AI 数学成就列表，并观察到一种针对著名、清晰陈述问题的社会学趋势。评论中也存在对 AI 潜在弱点的推测，例如在处理并发代码或时序逻辑方面，并一致认为真正新颖、优美的证明仍然是 AI 难以企及的高标准。

**标签**: `#artificial-intelligence`, `#large-language-models`, `#mathematics`, `#theorem-proving`, `#ai-research`

---

<a id="item-6"></a>
## [马斯克宣布未来所有特斯拉车型将集成星链，Robotaxi Cybercab 率先搭载。](https://www.techspot.com/news/113429-elon-musk-every-tesla-have-starlink-starting.html) ⭐️ 8.0/10

埃隆·马斯克宣布，未来所有特斯拉车型都将集成星链卫星互联网，即将推出的 Robotaxi Cybercab 已率先展示，其车顶后部集成了最高速率达 375 Mbps 的 V5 天线。该卫星连接将用于自动驾驶出租车服务的导航、客户服务和车队管理。 这一集成确保了特斯拉自动驾驶出租车车队无处不在的高带宽连接，这对于可靠的导航、实时车队管理以及乘客娱乐服务（如 4K 视频流）至关重要。它代表了特斯拉与 SpaceX 星链之间一次重要的战略协同，可能为自动驾驶汽车行业的连接性树立新标准。 集成的天线是新型、更紧凑且更节能的星链 V5 型号，提供最高 375 Mbps 的速率，略低于前代 V4 的 400+ Mbps。马斯克澄清，卫星链路并非车辆安全运行所必需，主要用于依赖连接的服务。

telegram · zaihuapd · Aug 12, 03:53

**背景**: 星链是由 SpaceX 运营的卫星互联网星座，在全球范围内提供高速、低延迟的互联网服务。星链 V5 是最新一代用户终端，比前代产品显著更小、更轻且更节能。Robotaxi（自动驾驶出租车）是一种设计为在没有人类驾驶员的情况下运营的自动驾驶汽车，需要持续、可靠的连接来进行导航、远程监控和乘客服务。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://starlink.com/public-files/specification_sheet_starlink_V5.pdf">WITH ROUTER MINI Specifications</a></li>
<li><a href="https://finance.yahoo.com/technology/articles/why-tesla-bolted-starlink-dish-141000280.html?fr=sycsrp_catchall">Why Tesla Bolted a Starlink Dish Into a Robotaxi That Doesn ...</a></li>
<li><a href="https://www.cubic3.com/blog/robotaxi-connectivity-foundations/">Robotaxi Connectivity Explained in Simple Terms | Cubic³</a></li>

</ul>
</details>

**标签**: `#Tesla`, `#Starlink`, `#Autonomous Vehicles`, `#Satellite Internet`, `#Connectivity`

---

<a id="item-7"></a>
## [企业级 SSD 占据 NAND 出货量 48%，长江存储首次跻身全球前三](https://china.counterpointresearch.com/%e6%9c%8d%e5%8a%a1%e5%99%a8%e9%9c%80%e6%b1%82%e6%8e%a8%e5%8d%87%e4%bc%81%e4%b8%9a%e7%ba%a7-ssd-%e5%8d%a0-nand-%e5%87%ba%e8%b4%a7%e9%87%8f%e7%99%be%e5%88%86%e4%b9%8b-48/) ⭐️ 8.0/10

Counterpoint 报告显示，在 AI 推理工作负载推动下，2026 年第二季度企业级 SSD 占全球 NAND 位元出货量的 48%，同比接近翻倍。中国的长江存储（YMTC）以 14%的份额首次超越铠侠，跻身全球 NAND 出货量前三名。 这一转变意味着，企业级存储（尤其是 AI 基础设施）正成为 NAND 闪存市场的主要驱动力，重塑着行业的重点和收入来源。长江存储出货量跃居全球第三，是全球半导体格局中的一个重要里程碑，凸显了中国在这一关键技术领域日益增强的竞争力，尽管仍面临地缘政治和营收方面的挑战。 尽管出货份额很高，但由于其产品组合偏向消费级 SSD 而非高价值的企业级型号，长江存储的营收仅排名第五。报告还预测，到今年年底，企业级 SSD 将消耗超过一半的 NAND 位元总量，突显了该细分市场日益增强的主导地位。

telegram · zaihuapd · Aug 12, 11:00

**背景**: NAND 闪存是 SSD（固态硬盘）中的核心存储部件。企业级 SSD 专为数据中心和服务器的高耐用性和持续性能而设计，与优先考虑个人设备成本效益的消费级 SSD 有显著不同。长江存储（YMTC）是中国主要的 3D NAND 闪存制造商，采用集成器件制造（IDM）模式运营。'NAND 位元出货量'指的是出货的内存总容量（以位为单位计量），是衡量闪存行业市场份额的关键指标。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.kingston.com/en/blog/pc-performance/enterprise-versus-client-ssd">The Difference Between Enterprise & Client SSD - Kingston Technology</a></li>
<li><a href="https://xenospectrum.com/en/ymtc-q2-2026-nand-shipment-share/">China's YMTC Ranks 3rd Globally in NAND Bit Shipments —14...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Yangtze_Memory_Technologies">Yangtze Memory Technologies - Wikipedia</a></li>

</ul>
</details>

**标签**: `#Semiconductors`, `#Storage`, `#AI Hardware`, `#Market Analysis`, `#Supply Chain`

---

<a id="item-8"></a>
## [微信团队发布 WeLM 大语言模型家族，以资源效率为核心并采用 MoE 架构](https://x.com/Weixin_WeChat/status/2087509298310209718) ⭐️ 8.0/10

微信研究团队发布了 WeLM 大语言模型系列，其中 WeLM-80B（激活参数量 3B）模型已应用于微信内的 AI 智能体“小微”。另一款正在研发中的更大模型 WeLM-617B（激活参数量 23B）采用了混合专家（MoE）架构，旨在处理更复杂的任务。 此次发布意义重大，它代表了来自拥有数十亿用户的主导平台——腾讯/微信的一个主要大语言模型系列，直接将 AI 能力集成到海量现实应用中。其对资源效率的关注，特别是通过 MoE 架构，解决了 AI 规模化部署中的一个关键挑战，即降低推理时的计算成本，这可能为工业界高效、可部署的大模型树立趋势。 WeLM-80B 模型每次推理仅激活 30 亿参数，现已部署用于处理对话、搜索和操作微信原生功能等任务。即将推出的 WeLM-617B MoE 模型，在总计 6170 亿参数中每次推理激活 230 亿参数，旨在为小程序开发和工具生成等复杂场景提供更强的通用理解和推理能力。

telegram · zaihuapd · Aug 12, 13:58

**背景**: 大语言模型（LLM）是在海量文本数据上训练的 AI 系统，用于理解和生成类人文本。混合专家（MoE）架构是一种模型设计，其中模型由许多子网络（“专家”）组成，但对于任何给定输入，只激活一个小的、被选中的子集。这种稀疏性使得模型可以拥有非常大的总参数量（存储广泛知识），同时保持每次推理的计算成本较低，因为只使用“激活参数”。这使得 MoE 成为构建能力更强且更高效模型的关键技术。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2507.11181">[2507.11181] Mixture of Experts in Large Language Models</a></li>
<li><a href="https://medium.com/@csburakkilic/understanding-moe-architectures-the-difference-between-total-and-active-parameters-ad1d161fccaa">Understanding MoE Architectures: The Difference Between Total and Active Parameters | by Burak Kılıç | Medium</a></li>

</ul>
</details>

**标签**: `#Large Language Models`, `#AI Efficiency`, `#MoE`, `#Industry AI`, `#WeChat`

---

<a id="item-9"></a>
## [DeepSeek-V4-Flash 正式版 API 上线公测，性能大幅提升](https://t.me/zaihuapd/43149) ⭐️ 8.0/10

2026 年 7 月 31 日，DeepSeek 上线了其 V4-Flash 模型的正式版 API 公测，该模型在智能体和编码能力的基准测试中表现出显著的性能提升。模型在 Terminal Bench 2.1 上得分为 82.7，在 Cybergym 上得分为 76.7，在 DSBench-FullStack 上得分为 68.7，在 DSBench-Hard 上得分为 59.6，远超 V4-Pro-Preview 版本。 此次发布为开发者提供了官方、稳定的访问渠道，使其能够利用一个能力显著增强的模型来构建 AI 智能体和编码助手。尤其是在复杂、真实世界的智能体任务和全栈开发方面的性能飞跃，使 DeepSeek-V4-Flash 在快速发展的 AI 领域中成为一个极具竞争力的选择。 正式版 V4-Flash 模型原生支持 Responses API 格式，并针对 Codex 进行了专门适配。模型的结构和尺寸与预览版保持一致，但在关键的智能体和编码基准测试中性能提升显著。

telegram · zaihuapd · Aug 12, 15:30

**背景**: DeepSeek 是一家知名的 AI 研究公司，以其大语言模型而闻名。新闻中提到的基准测试是专门的评估工具：Terminal Bench 2.1 用于衡量智能体在容器化环境中完成复杂任务的能力；Cybergym 测试 AI 复现已知软件漏洞的能力；而 DSBench-FullStack 和 DSBench-Hard 分别是 DeepSeek 用于评估全栈和具有挑战性的编码任务的内部基准。API（应用程序编程接口）允许开发者将模型的能力集成到他们自己的应用程序中。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.tbench.ai/news/terminal-bench-2-1">Terminal-Bench 2.1</a></li>
<li><a href="https://llm-boss.com/benchmarks/cybergym">CyberGym (Cybersecurity vulnerability reproduction) benchmark — AI ...</a></li>
<li><a href="https://deepseekv4guide.org/guides/flash-benchmarks">DeepSeek V4 Flash Benchmarks : 2026 Scores | DeepSeek V4 Guide</a></li>

</ul>
</details>

**标签**: `#AI`, `#LLM`, `#API`, `#Benchmark`, `#DeepSeek`

---

<a id="item-10"></a>
## [白宫拟扩大 AI 政策框架，将开源模型纳入发布前安全测试](https://www.wired.com/story/the-white-house-is-going-to-expand-its-ai-policy/) ⭐️ 8.0/10

据报道，白宫正修订其 AI 指南以扩大监管范围，计划在未来数月内将开源 AI 模型纳入框架，一旦其达到'前沿'能力阈值，就必须接受发布前的安全测试。由于政治顾虑，该框架目前仍属自愿性质。 此举意义重大，因为它通过将安全义务扩展到开源社区，可能重塑全球 AI 发展格局，在促进创新与管控风险之间寻求平衡。它也凸显了确保 AI 安全与维持美国（尤其是相对于中国的）竞争力之间的紧张关系。 此次政策扩展目前是自愿的，部分原因是特朗普阵营担心正式监管会帮助中国追赶美国。具体细节，如可能长达 30 天的测试要求，仍在讨论中，部分官员担忧这会抑制美国企业发展。

telegram · zaihuapd · Aug 13, 00:43

**背景**: 美国现行的 AI 政策框架是通过与领先 AI 公司的自愿承诺建立的，主要侧重于在发布前对最强大的闭源模型进行测试和安全保障。'前沿'AI 模型通常被定义为在关键基准测试中显著优于其他广泛部署的模型，因此带来独特风险，需要加强防护措施。发布前安全测试是指在模型公开发布前，评估其是否存在被滥用或失控等潜在危害。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.frontiermodelforum.org/uploads/2025/02/FMF-Issue-Brief-on-Thresholds-for-Frontier-AI-Safety-Frameworks.pdf">PDF Version of Thresholds for Frontier AI Safety Frameworks</a></li>
<li><a href="https://elpa.space/articles/pre-release-model-testing-ai-safety-state-power/">Pre - Release Model Testing Is the New Border Between AI Safety and...</a></li>

</ul>
</details>

**标签**: `#AI Policy`, `#AI Safety`, `#Open Source AI`, `#Government Regulation`, `#US-China Tech`

---