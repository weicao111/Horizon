---
layout: default
title: "Horizon Summary: 2026-05-22 (ZH)"
date: 2026-05-22
lang: zh
---

> From 29 items, 6 important content pieces were selected

---

1. [AI GPU 对 HBM 内存的需求推高了消费电子设备 RAM 的成本。](#item-1) ⭐️ 8.0/10
2. [MATLAB 创造者、数值计算先驱 Cleve Moler 逝世。](#item-2) ⭐️ 8.0/10
3. [Freenet 重新设计为基于 WebAssembly 合约的去中心化键值存储平台](#item-3) ⭐️ 8.0/10
4. [礼来公司药物 retatrutide 在三期肥胖试验中实现平均减重 28.3%](#item-4) ⭐️ 8.0/10
5. [字节跳动开源 3B 参数统一多模态模型 Lance，可同时处理图像视频理解与生成。](#item-5) ⭐️ 8.0/10
6. [中国八部门联合整治非法跨境证券业务，老虎证券、富途控股等平台被立案调查。](#item-6) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [AI GPU 对 HBM 内存的需求推高了消费电子设备 RAM 的成本。](https://davidoks.blog/p/ai-is-killing-the-cheap-smartphone) ⭐️ 8.0/10

一篇详细分析指出，用于 AI 训练 GPU 的高带宽内存（HBM）需求激增，正在挤占先进的半导体制造产能，这反过来又提高了用于智能手机和笔记本电脑的 DDR 和 LPDDR 内存的生产成本和市场价格。 这种供应链的转变直接影响消费电子产品的可负担性，随着制造商将内存成本上涨转嫁给消费者，可能导致智能手机和笔记本电脑价格上涨。这突显了 AI 基础设施的爆炸式增长如何对更广泛的技术市场产生切实的、通胀性的影响。 文章指出，建造一个先进的 DRAM 制造工厂需要 150 亿至 200 亿美元，并且一个新工厂需要数年时间才能达到可接受的生产良率。内存制造的技术复杂性和高资本密集度，限制了供应端对不同内存类型（如 HBM 和 DDR）之间突然的需求变化做出快速反应的能力。

hackernews · d0ks · May 21, 21:55 · [社区讨论](https://news.ycombinator.com/item?id=48229319)

**背景**: 高带宽内存（HBM）是一种专为高性能计算设计的 DRAM。它将多个内存芯片垂直堆叠，并使用非常宽的数据总线，与传统平铺在电路板上的 DDR（双倍数据速率）内存相比，可实现更高的带宽和更低的功耗。LPDDR（低功耗 DDR）是为移动设备优化的变体，在这些设备中电源效率至关重要。AI 训练 GPU（如 NVIDIA 的 H200）需要海量的快速内存带宽，因此 HBM 成为其首选，而笔记本电脑和手机等消费设备主要使用 DDR 和 LPDDR。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/High_Bandwidth_Memory">High Bandwidth Memory - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/LPDDR">LPDDR - Wikipedia</a></li>
<li><a href="https://www.nvidia.com/en-us/data-center/h200/">H200 GPU | NVIDIA</a></li>

</ul>
</details>

**社区讨论**: 评论者认为这篇文章对内存市场动态进行了引人入胜的深入解释，有人指出其标题未能完全体现文章价值。一个关键的讨论点质疑了手机 RAM 消耗增加的趋势是否不可避免，认为软件优化和使用更旧的算法可以让设备使用更少的内存，从而可能缓解成本压力。

**标签**: `#semiconductors`, `#hardware`, `#economics`, `#supply-chain`, `#ai-hardware`

---

<a id="item-2"></a>
## [MATLAB 创造者、数值计算先驱 Cleve Moler 逝世。](https://www.mathworks.com/company/aboutus/founders/clevemoler.html) ⭐️ 8.0/10

MATLAB 编程语言和环境的创造者、数学家兼计算机科学家 Cleve Moler 已经去世。他最初在 1970 年代末开发了 MATLAB，作为一种教学工具，旨在让学生无需编译 FORTRAN 代码即可交互式地访问矩阵软件库。 Moler 创造的 MATLAB 成为了数十年来科学计算、工程教育和研究的基础工具，直接影响着数百万工程师和科学家。其设计理念和成功也启发了 SciPy/NumPy 等主要开源科学计算生态系统的发展，这些系统是现代数据科学和人工智能的基石。 MATLAB 的原始版本名为 MATrix LABoratory，是用 FORTRAN 语言编写的，大约有 2000 行代码。虽然 MATLAB 本身演变成了商业产品，但其交互式矩阵操作和数值算法可访问性的核心理念，成为了后续工具效仿的典范。

hackernews · mychele · May 22, 02:35 · [社区讨论](https://news.ycombinator.com/item?id=48231319)

**背景**: 数值计算涉及使用算法通过数值近似来解决数学问题，这在工程学、物理科学和数据分析中至关重要。MATLAB 是一种专门为数值计算、矩阵操作和算法实现而设计的高级语言和交互式环境。它的诞生源于 Moler 在数值线性代数经典 FORTRAN 库方面的工作，以及他希望让这些工具在教学上更易获取的愿望。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Numerical_computing">Numerical computing</a></li>
<li><a href="https://en.wikipedia.org/wiki/MATLAB">MATLAB - Wikipedia</a></li>
<li><a href="https://www.mathworks.com/company/technical-articles/a-brief-history-of-matlab.html">A Brief History of MATLAB - MATLAB & Simulink</a></li>

</ul>
</details>

**社区讨论**: 社区表达了深深的敬意和感激，强调了 Moler 在数值方法和创建基础 FORTRAN 库方面的奠基性作用。评论者指出 MATLAB 对工程教育的深远影响，以及它作为开源数据科学栈（NumPy、SciPy）直接灵感来源的角色。许多人分享了 MATLAB 如何引领他们进入编程领域，并成为他们学习和职业生涯中不可或缺工具的个人故事。

**标签**: `#obituary`, `#numerical-computing`, `#matlab`, `#scientific-computing`, `#history`

---

<a id="item-3"></a>
## [Freenet 重新设计为基于 WebAssembly 合约的去中心化键值存储平台](https://freenet.org/) ⭐️ 8.0/10

Freenet 的原始创建者发布了该项目的彻底重新设计版本，其架构现在是一个全局的、去中心化的键值存储，其中键是用于定义和管理状态的 WebAssembly 合约。新平台自 2024 年 12 月起已投入运行，并已托管了诸如 River（去中心化聊天）和 Delta（去中心化内容管理系统）等应用程序。 这次重新设计标志着一个基础性点对点项目的重大演进，将其从一个文件共享网络转变为一个可编程的去中心化应用（dApp）平台。通过使用 WebAssembly 合约和可交换的合并操作来强制实现状态一致性，它为构建抗审查、无服务器、可直接在浏览器中运行的 Web 应用提供了一种新颖的架构。 一个核心的技术创新是要求每个合约为其状态定义一个可交换的合并操作，这使得更新能像“病毒”一样传播，并在几秒钟内实现全局一致性。应用程序从网络下载并在 Web 浏览器中运行，通过 WebSocket 本地连接到 Freenet 节点，而非远程数据中心；不过，目前尚未提供移动端安装程序。

hackernews · sanity · May 21, 14:34 · [社区讨论](https://news.ycombinator.com/item?id=48223362)

**背景**: Freenet 最初于 21 世纪初推出，是一个为抗审查通信和发布而设计的点对点平台。2023 年年中，原始代码库更名为 Hyphanet，而这个新的“Freenet”代表了一个独立的、彻底重写的版本。去中心化键值存储是一种非关系型数据库，它将唯一的键映射到值，是构建像 Amazon DynamoDB 这样可扩展、容错的分布式系统的基础构件。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Hyphanet">Hyphanet - Wikipedia</a></li>
<li><a href="https://dev.to/josephakayesi/design-a-distributed-key-value-store-2f">Design a Distributed Key-Value Store - DEV Community</a></li>

</ul>
</details>

**社区讨论**: 社区讨论揭示了关于项目治理的重大争议，有一条评论指控此次重设计是一个“幕后决定”，抛弃了原团队的工作。技术方面，人们对状态合并模型对于投票系统等复杂应用的实用性提出了担忧，并询问了关于引导、延迟、磁盘使用限制以及命名/匿名性将如何解决等问题。

**标签**: `#decentralization`, `#peer-to-peer`, `#webassembly`, `#distributed-systems`

---

<a id="item-4"></a>
## [礼来公司药物 retatrutide 在三期肥胖试验中实现平均减重 28.3%](https://www.prnewswire.com/news-releases/lillys-triple-agonist-retatrutide-delivered-powerful-weight-loss-in-pivotal-phase-3-obesity-trial-302778859.html) ⭐️ 8.0/10

礼来公司宣布，其三重激动剂药物 retatrutide 在关键的三期 TRIUMPH-1 肥胖试验中达到了所有主要和关键次要终点，最高剂量组（12 毫克）在 80 周内实现了平均 28.3%的减重。此外，该组中有 45.3%的参与者减重至少 30%。 这一结果代表了肥胖症药物治疗有效性的重大飞跃，可能为减肥药物设定新的疗效基准，并在利润丰厚的 GLP-1 及多激动剂市场竞争中加剧竞争。如此显著的减重效果可能为数百万肥胖及相关合并症患者带来更好的健康结果。 该试验招募了约 2500 名患有肥胖或超重且至少伴有一种体重相关合并症的成年人。最常见的副作用是胃肠道反应，公司报告未观察到心脏或肝脏安全问题，且因不良事件导致的停药率（4.1%）低于安慰剂组（4.9%）。

telegram · zaihuapd · May 22, 02:18

**背景**: Retatrutide 是一种新型的'三重激动剂'，能同时激活三种激素受体：GIP、GLP-1 和胰高血糖素。这种多靶点方法旨在增强代谢效应，如抑制食欲和增加能量消耗，其效果预期会超越单激动剂或双激动剂（如司美格鲁肽或替尔泊肽）。TRIUMPH 临床项目正是为了评估 retatrutide 在患有肥胖或超重的成年人中进行长期体重管理的效果。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.retatrutide.med/knowledge-base/mechanism-of-action">Mechanism of Action : How Retatrutide 's Triple Receptor Agonism...</a></li>
<li><a href="https://medical.lilly.com/us/products/answers/what-retatrutide-clinical-trials-are-being-conducted-in-people-with-obesity-or-overweight-229656">What retatrutide clinical trials are being conducted in people with...</a></li>
<li><a href="https://www.fiercebiotech.com/biotech/eli-lillys-triple-g-drug-drives-deep-weight-loss-phase-3-obesity-trial">Lilly’s triple-G drug drives deep weight loss in phase 3 trial</a></li>

</ul>
</details>

**标签**: `#pharmaceuticals`, `#clinical-trials`, `#obesity-treatment`, `#biotechnology`

---

<a id="item-5"></a>
## [字节跳动开源 3B 参数统一多模态模型 Lance，可同时处理图像视频理解与生成。](https://mp.weixin.qq.com/s/Xbfq72cr1796RZxJIs3L1A) ⭐️ 8.0/10

字节跳动开源了轻量级多模态模型 Lance，其激活参数量仅为 30 亿，原生统一了图像理解、视频理解、图像生成、视频生成和跨模态编辑任务。该模型采用 Apache 2.0 许可，权重已在 Hugging Face 平台开放，并在 GenEval 图像生成和 VBench 视频生成等基准测试中取得了领先结果。 此次发布意义重大，因为它提供了一个规模相对较小、却能统一执行图像和视频的理解与生成任务的模型，使得先进的多模态 AI 技术更易于获取且更高效。宽松的 Apache 2.0 许可证以及在 Hugging Face 等主流平台的可用性，降低了研究人员和开发者的使用门槛，有望加速内容创作、交互式 AI 等领域的创新。 Lance 采用了共享上下文与双流专家架构，分别使用 Qwen2.5-VL 和 Wan2.2 编码器来处理理解与生成任务，同时促进信息交换。该模型还采用了模态感知位置编码来解决序列边界混淆问题，这是在统一框架内处理混合输入和输出模态的关键技术细节。

telegram · zaihuapd · May 22, 06:40

**背景**: 统一多模态模型是 AI 领域的一个发展趋势，旨在将图像、文本、视频等多种模态集成到单一架构中，以联合执行推理和生成任务。这类模型通常采用专门的架构，例如双流设计，为不同类型的数据保持独立的处理路径，同时实现跨模态交互。其目标是超越独立的、特定于任务的模型，转向能够执行多样化多模态功能的、更通用且高效的 AI 系统。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/AIDC-AI/Awesome-Unified-Multimodal-Models">Awesome Unified Multimodal Models - GitHub</a></li>
<li><a href="https://www.emergentmind.com/topics/unified-multimodal-models-umms">Unified Multimodal Models (UMMs) Overview - emergentmind.com</a></li>
<li><a href="https://www.emergentmind.com/topics/dual-stream-context-architecture-0b723934-4838-4e1a-9555-1cfb22d8863f">Dual-Stream Context Architecture</a></li>

</ul>
</details>

**标签**: `#multimodal-ai`, `#computer-vision`, `#open-source`, `#generative-ai`, `#video-generation`

---

<a id="item-6"></a>
## [中国八部门联合整治非法跨境证券业务，老虎证券、富途控股等平台被立案调查。](https://mp.weixin.qq.com/s?__biz=MzA4NzAzMDgwMw==&amp;mid=2651090403&amp;idx=3&amp;sn=bca72a940ac72bef356f29b5b9576ac1&amp;chksm=8a1670281e2bc67d2df3608a313ba9fdaf0fcd2f43ce44475c6bf273b386af2e4f9d8e8e2e2b&amp;scene=0&amp;xtrack=1) ⭐️ 8.0/10

中国证监会等八部门联合印发整治方案，明确未经批准的境外机构不得在境内开展招揽客户、开户、传输交易指令或划转资金等业务。方案设定了两年的集中整治期，期间只允许存量投资者单向卖出并转出资金。 此次整治行动影响深远，将彻底改变中国内地零售投资者参与境外市场的格局，迫使老虎证券、富途等热门金融科技平台清退内地业务。这标志着中国政府对跨境资本流动的监管收紧，旨在引导投资者通过港股通、QDII 等官方合规渠道进行境外投资。 证监会已对老虎证券、富途控股、长桥证券的相关主体立案调查并作出行政处罚事先告知，拟没收其全部违法所得并依法严厉处罚。这些机构被指未经核准，在境内非法从事证券经纪、融资融券、公募基金销售及期货经纪等业务。

telegram · zaihuapd · May 22, 08:26

**背景**: 老虎证券、富途控股等跨境互联网券商长期以来为内地投资者提供了交易美股、港股等境外证券的渠道。在中国，开展跨境证券业务需要获得专门的监管批准。政府已建立官方的对外投资渠道，例如合格境内机构投资者（QDII）制度，允许持牌境内机构进行境外投资；以及粤港澳大湾区“跨境理财通”，为湾区居民提供个人跨境投资对方市场理财产品的便利化安排。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://zh.wikipedia.org/zh-sg/跨境理财通">跨境理财通 - 维基百科，自由的百科全书</a></li>
<li><a href="https://www.hkma.gov.hk/gb_chi/key-functions/international-financial-centre/wealth-management-connect/">香港金融管理局 - 粤港澳大湾区跨境理财通</a></li>

</ul>
</details>

**标签**: `#Financial Regulation`, `#Fintech`, `#Cross-Border Investment`, `#Securities Law`, `#China Tech`

---