---
layout: default
title: "Horizon Summary: 2026-05-22 (ZH)"
date: 2026-05-22
lang: zh
---

> From 30 items, 7 important content pieces were selected

---

1. [AI GPU 对 HBM 的需求导致内存短缺，推高了消费电子产品价格。](#item-1) ⭐️ 8.0/10
2. [MATLAB 创造者、MathWorks 联合创始人 Cleve Moler 逝世。](#item-2) ⭐️ 8.0/10
3. [Freenet 重新设计为支持 WebAssembly 去中心化应用的去中心化键值存储平台](#item-3) ⭐️ 8.0/10
4. [FTC 对三家公司处以近百万美元罚款，因其就“主动聆听”AI 营销服务欺骗客户。](#item-4) ⭐️ 8.0/10
5. [礼来 retatrutide 在三期肥胖试验中实现平均减重 28.3%](#item-5) ⭐️ 8.0/10
6. [字节跳动开源 3B 统一多模态模型 Lance，可同时处理图像视频理解与生成。](#item-6) ⭐️ 8.0/10
7. [中国八部门联合整治非法跨境证券业务，老虎、富途、长桥被立案调查](#item-7) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [AI GPU 对 HBM 的需求导致内存短缺，推高了消费电子产品价格。](https://davidoks.blog/p/ai-is-killing-the-cheap-smartphone) ⭐️ 8.0/10

用于 AI GPU 的高带宽内存（HBM）需求激增，正在挤占半导体制造产能，导致用于智能手机和笔记本电脑的 DDR 和 LPDDR 内存出现短缺和价格上涨。这种生产重心的转移正直接影响消费电子产品的成本和供应。 这很重要，因为它揭示了蓬勃发展的 AI 硬件行业与消费者日常设备可负担性之间的直接经济联系。这可能导致智能手机和笔记本电脑价格上涨，可能减缓新技术的普及并加剧数字鸿沟。 文章指出，建造一个先进的 DRAM 制造工厂（fab）成本高达 150-200 亿美元，设备还需额外数十亿美元，并且需要数年时间才能实现高良品率。虽然 HBM 为 AI 工作负载提供了极高的带宽，但其生产工艺比标准的 DDR/LPDDR 内存更复杂、成本更高。

hackernews · d0ks · May 21, 21:55 · [社区讨论](https://news.ycombinator.com/item?id=48229319)

**背景**: 高带宽内存（HBM）是一种为极高数据传输速率设计的 3D 堆叠 DRAM，对 AI 和高性能计算 GPU 至关重要。相比之下，DDR（双倍数据速率）内存是台式机和高性能笔记本电脑的标准配置，而 LPDDR（低功耗 DDR）则针对能效进行了优化，普遍用于智能手机和平板电脑。所有这些内存类型的制造都需要争夺相同的先进半导体制造资源。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/High_Bandwidth_Memory">High Bandwidth Memory - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/LPDDR">LPDDR - Wikipedia</a></li>
<li><a href="https://intuitionlabs.ai/articles/hbm-vs-ddr-memory-comparison">HBM vs. DDR: Key Differences in Memory Technology Explained</a></li>

</ul>
</details>

**社区讨论**: 社区讨论强调，文章对内存市场机制进行了深入而精彩的解释。一位评论者对建造 DRAM 工厂的巨大成本和复杂性感到惊讶。另一位指出，标题未能充分体现文章的价值，即文章将 HBM 需求与消费电子设备的供应联系起来。进一步的讨论则质疑，软件优化和旧的内存标准是否能减轻对廉价手机的影响。

**标签**: `#semiconductors`, `#hardware`, `#economics`, `#ai-hardware`, `#supply-chain`

---

<a id="item-2"></a>
## [MATLAB 创造者、MathWorks 联合创始人 Cleve Moler 逝世。](https://www.mathworks.com/company/aboutus/founders/clevemoler.html) ⭐️ 8.0/10

数学家兼计算机程序员 Cleve Moler 已经逝世，他创造了最初的 MATLAB 并联合创立了 MathWorks。MathWorks 官网发布了这一消息，标志着科学计算领域一位奠基性人物的离去。 Moler 创造的 MATLAB 通过交互式环境使高级矩阵运算和算法变得易于使用，从而彻底改变了数值计算。他的工作为现代科学计算、工程教育和数据科学工具奠定了基础，影响了一代又一代的研究人员，并推动了 NumPy、SciPy 等开源生态系统的发展。 最初的 MATLAB 用 FORTRAN 编写，大约有 2000 行代码，由 Moler 在 1970 年代末创建，作为一个教学工具，让学生无需编译 FORTRAN 代码即可与线性代数和矩阵库函数进行交互。它在工程专业学生中的成功，最终促成了 MATLAB 的商业化以及 MathWorks 公司的成立。

hackernews · mychele · May 22, 02:35 · [社区讨论](https://news.ycombinator.com/item?id=48231319)

**背景**: MATLAB 是 MATrix LABoratory（矩阵实验室）的缩写，是由 MathWorks 开发的专有编程语言和数值计算环境。它被广泛应用于学术界和工业界，用于算法开发、数据分析、可视化和数值计算。数值分析是研究使用数值近似来解决数学分析问题的算法的学科，它是 MATLAB 等工具的核心。Cleve Moler 是数值方法领域的关键人物，在创建 MATLAB 之前，他曾为线性代数的经典 FORTRAN 库做出贡献。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/MATLAB">MATLAB - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Numerical_analysis">Numerical analysis - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 社区表达了深切的敬意和哀悼，强调了 Moler 在数值方法和创建 MATLAB 方面的奠基性作用。评论指出，MATLAB 是许多工程师接触编程的入门工具，并在数十年的教育和研究中发挥了重要作用。一些用户指出了 MATLAB 对现代开源数据科学栈（尤其是 NumPy/SciPy）的深远影响，同时也承认了当前在许多领域对开源替代品的偏好。

**标签**: `#obituary`, `#numerical-methods`, `#matlab`, `#scientific-computing`, `#history-of-computing`

---

<a id="item-3"></a>
## [Freenet 重新设计为支持 WebAssembly 去中心化应用的去中心化键值存储平台](https://freenet.org/) ⭐️ 8.0/10

点对点项目 Freenet（现更名为 Hyphanet）的原始创建者宣布了对该系统进行了一次彻底的、从头开始的重新设计，新版本已于去年 12 月上线运行。新版 Freenet 是一个全球性的去中心化键值存储平台，其键是 WebAssembly 合约，用于定义和管理应用状态，从而支持去中心化聊天（River）和内容管理系统（Delta）等应用。 这代表了一种构建去中心化应用（dApp）的新颖架构方法，它不依赖于中心化服务器或传统区块链，可能使抗审查和保护隐私的软件更易普及。通过使用 WebAssembly 合约进行状态管理，并采用独特的可交换合并操作来保证一致性，该项目旨在为新一代点对点网络应用提供可扩展且高效的基础。 一项核心技术创新是要求每个合约为其状态定义一个可交换的合并操作，这使得更新能在网络中快速传播，通常能在几秒内实现全局状态一致。该平台目前为主要的桌面操作系统提供了便捷的安装程序，支持通过本地 WebSocket 连接到 Freenet 节点，从而在网页浏览器中直接运行 dApp，但尚未支持移动端。

hackernews · sanity · May 21, 14:34 · [社区讨论](https://news.ycombinator.com/item?id=48223362)

**背景**: Freenet 是一个长期存在的、专注于抗审查通信的点对点项目，最初于 21 世纪初启动。2023 年，其原始代码库被拆分出来，成为一个更名为 Hyphanet 的独立项目，而 'Freenet' 这个名称则被重新用于指代这次全新的、从头设计的版本。去中心化键值存储是一种分布式系统，数据通过唯一的键进行存储和检索，通常设计为无需中央权威即可实现高可用性和可扩展性。WebAssembly (Wasm) 是一种可移植的二进制指令格式，允许由 Rust 或 C++ 等语言编译的代码在网页浏览器和其他环境中以接近原生的速度运行，正越来越多地用于智能合约和去中心化应用逻辑。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Hyphanet">Hyphanet - Wikipedia</a></li>
<li><a href="https://freenet.org/about/history/">Freenet's History</a></li>
<li><a href="http://adslab.cse.cuhk.edu.hk/pubs/socc19.pdf">Coupling Decentralized Key - Value Stores with Erasure Coding</a></li>

</ul>
</details>

**社区讨论**: 社区讨论揭示了关于项目治理的重大争议，有一条评论指控此次重新设计是一次"幕后决定"，边缘化了原始开发团队。技术性质疑集中在实际限制上，如启动速度、延迟、磁盘使用量以及去中心化命名（类似 DNS 的功能）的挑战。另一个关键担忧是状态合并模型是否足以解决复杂应用中的难题，例如需要复杂共识或用户身份验证的应用中的冲突解决。

**标签**: `#peer-to-peer`, `#decentralization`, `#webassembly`, `#distributed-systems`, `#privacy`

---

<a id="item-4"></a>
## [FTC 对三家公司处以近百万美元罚款，因其就“主动聆听”AI 营销服务欺骗客户。](https://simonwillison.net/2026/May/22/ftc-active-listening/#atom-everything) ⭐️ 8.0/10

美国联邦贸易委员会（FTC）要求 Cox Media Group 及另外两家公司支付近 100 万美元，以了结关于其“主动聆听”AI 营销服务欺骗客户的指控。FTC 发现，该服务并未如宣传那样监听消费者对话或使用语音数据，而只是转售从数据经纪人处获得的电子邮件列表。 这项和解是一项重要的监管行动，为打击“AI 洗白”（夸大或捏造 AI 能力以欺骗客户）树立了先例。它加强了数字时代的消费者保护，并向营销人员就数据收集和 AI 定向广告的虚假宣传发出了明确警告。 FTC 明确指出，将语音数据收集的同意条款隐藏在强制性的应用服务条款中，并不构成充分的“选择加入”式同意。作者之前的分析认为，“主动聆听”一词很可能是对现有广告定向技术的营销隐喻，而这些公司在宣传材料中误解或夸大了它。

rss · Simon Willison · May 22, 04:48

**背景**: 行为定向是一种常见的数字广告实践，它利用收集到的用户行为数据来投放相关广告。“主动聆听”被宣传为一种 AI 服务，声称利用智能设备麦克风捕捉实时对话数据以实现超精准广告投放，这助长了关于手机会“监听”以推送广告的长期消费者阴谋论。FTC 一直在加大打击 deceptive AI claims（欺骗性 AI 宣传，即“AI 洗白”）的力度。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.business-standard.com/technology/tech-news/is-your-phone-listening-marketing-firm-confirms-tech-behind-targeted-ads-124090400592_1.html">Is your phone listening ? Marketing firm confirms... - Business Standard</a></li>
<li><a href="https://dovetail.com/ux/what-is-behavioral-targeting/">What Is Behavioral Targeting ? Types, Examples, and FAQs</a></li>
<li><a href="https://directpaynet.com/ftc-deceptive-ai-claims-crackdown/">FTC Targets Deceptive AI Claims, Shopify and Stripe... - DirectPayNet</a></li>

</ul>
</details>

**标签**: `#AI Ethics`, `#Regulation`, `#Privacy`, `#Marketing`, `#FTC`

---

<a id="item-5"></a>
## [礼来 retatrutide 在三期肥胖试验中实现平均减重 28.3%](https://www.prnewswire.com/news-releases/lillys-triple-agonist-retatrutide-delivered-powerful-weight-loss-in-pivotal-phase-3-obesity-trial-302778859.html) ⭐️ 8.0/10

礼来公司宣布，其三重激动剂药物 retatrutide 在关键的 TRIUMPH-1 三期试验中达到了所有主要和关键次要终点。在为期 80 周、使用最高剂量 12 mg 的治疗中，参与者平均减重 28.3%，其中 45.3%的参与者减重至少 30%。 这一结果代表了药物肥胖治疗在疗效上的重大飞跃，可能为这一全球健康危机提供更强大的治疗选择。前所未有的减重百分比可能显著改善与体重相关的合并症，如 2 型糖尿病和心血管疾病。 该试验招募了约 2500 名患有肥胖或超重且至少伴有一种相关疾病的成年人。最常见的副作用是胃肠道反应，公司报告未观察到心脏或肝脏安全问题，且因不良事件停药率（4.1%）低于安慰剂组（4.9%）。

telegram · zaihuapd · May 22, 02:18

**背景**: Retatrutide 是一种新型的三重受体激动剂，可同时靶向 GLP-1、GIP 和胰高血糖素受体，这种机制旨在产生超越司美格鲁肽（Wegovy/Ozempic）等单通路药物的代谢效应。肥胖是一种慢性疾病，与多种严重合并症相关，包括 2 型糖尿病、心脏病和阻塞性睡眠呼吸暂停，即使适度的减重（5-15%）也能带来显著的健康益处。TRIUMPH 项目包括多项试验，旨在评估 retatrutide 在肥胖人群及特定相关病症患者中的疗效和安全性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://pmc.ncbi.nlm.nih.gov/articles/PMC12190491/">Retatrutide —A Game Changer in Obesity Pharmacotherapy - PMC</a></li>
<li><a href="https://www.ncbi.nlm.nih.gov/books/NBK574535/">Obesity and Comorbid Conditions - StatPearls - NCBI Bookshelf</a></li>
<li><a href="https://medical.lilly.com/us/products/answers/what-retatrutide-clinical-trials-are-being-conducted-in-people-with-obesity-or-overweight-229656">What retatrutide clinical trials are being conducted in people with obesity or overweight?</a></li>

</ul>
</details>

**标签**: `#pharmaceuticals`, `#clinical-trials`, `#obesity-treatment`, `#biotechnology`, `#healthcare`

---

<a id="item-6"></a>
## [字节跳动开源 3B 统一多模态模型 Lance，可同时处理图像视频理解与生成。](https://mp.weixin.qq.com/s/Xbfq72cr1796RZxJIs3L1A) ⭐️ 8.0/10

字节跳动开源了轻量级多模态模型 Lance，其激活参数量仅为 30 亿，原生统一了图像理解、视频理解、图像生成、视频生成和跨模态编辑，一个模型即可输出文本、图像和视频。该模型采用 Apache 2.0 许可，权重已在 Hugging Face 平台开放。 此次发布意义重大，因为它展示了一种在相对较小的参数量下，统一处理图像和视频的感知与生成任务的架构，这可能降低开发多模态 AI 应用的计算门槛。宽松的 Apache 2.0 许可证以及在 Hugging Face 等主流平台上的即时可用性，极大地增强了其可访问性，并为其广泛采用和创新提供了潜力。 Lance 采用了共享上下文与双流专家架构，分别使用 Qwen2.5-VL 编码器处理理解任务，Wan2.2 编码器处理生成任务，并通过模态感知位置编码来解决序列边界混淆问题。据报道，该模型在 GenEval 图像生成、VBench 视频生成等基准测试中取得了领先结果。

telegram · zaihuapd · May 22, 06:40

**背景**: 统一多模态模型是一种机器学习架构，旨在单个统一的框架内处理和生成不同类型的数据，如文本、图像和视频。它们通常使用统一的标记序列来表示各种模态，相比于为每个任务使用独立架构，这简化了模型设计。这一概念旨在实现不同形式数据之间无缝的交互，以同时服务于理解和生成任务。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.emergentmind.com/topics/unified-multimodal-models">Unified Multimodal Models</a></li>
<li><a href="https://braintitan.medium.com/transfusion-a-unified-multimodal-model-for-text-and-image-generation-ed67c7fcae4f">Transfusion: A unified multimodal model for text and image... | Medium</a></li>

</ul>
</details>

**标签**: `#multimodal-ai`, `#computer-vision`, `#open-source`, `#generative-ai`, `#model-architecture`

---

<a id="item-7"></a>
## [中国八部门联合整治非法跨境证券业务，老虎、富途、长桥被立案调查](https://mp.weixin.qq.com/s?__biz=MzA4NzAzMDgwMw==&amp;mid=2651090403&amp;idx=3&amp;sn=bca72a940ac72bef356f29b5b9576ac1&amp;chksm=8a1670281e2bc67d2df3608a313ba9fdaf0fcd2f43ce44475c6bf273b386af2e4f9d8e8e2e2b&amp;scene=0&amp;xtrack=1) ⭐️ 8.0/10

中国证监会等八部门联合印发整治非法跨境证券期货基金经营活动的方案，设定了为期两年的集中整治期，以清理存量业务。证监会已对老虎证券、富途证券、长桥证券境内外相关主体立案调查并作出行政处罚事先告知，拟没收其全部违法所得并依法严厉处罚。 此次整治是中国加强资本管制和金融监管的重要举措，直接影响数百万通过此类平台投资海外市场的大陆投资者。它迫使跨境金融科技行业进行重大重组，未来所有境外投资必须通过港股通、合格境内机构投资者（QDII）和跨境理财通等官方批准渠道进行，从而加强了监管监督和资本流动管理。 在为期两年的整治期内，存量投资者仅被允许进行单向卖出并转出资金；期满后，相关的境内网站、交易软件及配套服务器需全面关停。整治对象不仅包括境外机构，还包括协助展业的境内关联方、中介，以及提供开户通道或营销引流的信息平台和自媒体。

telegram · zaihuapd · May 22, 08:26

**背景**: 在中国，经营证券、期货和基金业务需要获得中国证监会颁发的特定许可证。老虎证券、富途证券等平台虽然在海外合法注册，但在未取得必要国内批准的情况下，一直积极向中国大陆投资者进行营销和提供服务。对于合法的跨境投资，中国监管机构已建立了诸如港股通（允许交易香港上市股票）、合格境内机构投资者（QDII，投资海外的基金）以及粤港澳大湾区跨境理财通等渠道。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://finance.stockstar.com/IG2026052200042755.shtml">证 监会重拳打击 非 法 跨 境 炒股 老虎、富途、长桥被查_财经频道_ 证 券 之星</a></li>
<li><a href="https://baike.baidu.com/item/跨境理财通/50994641">跨境理财通_百度百科 《港股QDII基金与港股通基金对比》 - 知乎 投资海外股市有哪些通道？对比QDII基金与港股通的优势劣势_港股通和qd... 划重点！“跨境理财通”2.0七问七答 - 腾讯新闻 港股QDII与港股通基金有何不同？_财富号_东方财富网</a></li>
<li><a href="https://m.guancha.cn/GuanJinRong/2026_05_22_818035.shtml">m.guancha.cn/GuanJinRong/2026_05_22_818035.shtml</a></li>

</ul>
</details>

**标签**: `#Financial Regulation`, `#Fintech`, `#Cross-Border Investment`, `#Tech Industry`, `#Business News`

---