---
layout: default
title: "Horizon Summary: 2026-09-08 (ZH)"
date: 2026-09-08
lang: zh
---

> From 27 items, 7 important content pieces were selected

---

1. [研究人员使用消费级 GPU 成功分解了 1990 年代证书颁发机构的 512 位 RSA 密钥。](#item-1) ⭐️ 8.0/10
2. [llm CLI 工具 0.35 版本新增对 OpenAI GPT-6 Astra 模型的支持。](#item-2) ⭐️ 8.0/10
3. [华为发布采用逻辑折叠架构的麒麟 9050 Pro 芯片](#item-3) ⭐️ 8.0/10
4. [中国最高人民法院发布司法解释，明确 AI 纠纷中换脸、算法杀熟等责任](#item-4) ⭐️ 8.0/10
5. [联合国环境规划署报告预测全球升温峰值约 1.8°C，将突破《巴黎协定》1.5°C 目标](#item-5) ⭐️ 8.0/10
6. [美国审查中国 AI 企业海外获取英伟达芯片渠道，包括远程云访问](#item-6) ⭐️ 8.0/10
7. [字节跳动讨论训练参数规模超 5 万亿的大语言模型](#item-7) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [研究人员使用消费级 GPU 成功分解了 1990 年代证书颁发机构的 512 位 RSA 密钥。](https://mcpherrin.ca/2026/09/07/rsa.html) ⭐️ 8.0/10

一名研究人员成功分解了属于 1990 年代一个历史证书颁发机构的 512 位 RSA 密钥，仅使用消费级 GPU 在大约两天内完成了这项任务。这项工作需要一个定制的 TLS 实现来与 Netscape Communicator 4.51 等遗留软件交互。 这一演示凸显了历史上曾用于电子商务的 512 位 RSA 加密在实际中已变得脆弱。它强调了保留旧的、弱加密数据的风险，因为现代消费级硬件现在可以追溯性地破解它，这对数据隐私和历史安全审计具有重要影响。 分解是在消费级 GPU 上完成的，而非专用硬件，目标是那个时代某个特定证书颁发机构的密钥。研究人员指出，那个时期的大量流量并未使用临时密钥，这使得一旦长期密钥被破解，进行这种追溯性解密成为可能。

hackernews · ahlCVA · Sep 8, 01:16 · [社区讨论](https://news.ycombinator.com/item?id=49604637)

**背景**: RSA 是一种广泛使用的公钥密码系统，其安全性依赖于分解两个大质数乘积的难度。512 位 RSA 密钥在 1990 年代被认为是强大的，但在 1999 年首次被公开破解；如今，2048 位或更大的密钥已成为标准。证书颁发机构（CA）是颁发数字证书的实体，这些证书是用于安全网页浏览的 TLS/SSL 加密的基础。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/RSA_Factoring_Challenge">RSA Factoring Challenge - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/RSA_(cryptosystem)">RSA (cryptosystem) - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Certificate_authority">Certificate authority - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 社区讨论强调了使用消费级硬件在两天内破解密钥的技术成就，以及当时大量流量未加密或使用静态密钥的历史背景。有人担忧政府可能现在记录加密数据，以便随着技术进步在未来进行解密。一些用户还指出自动化 SSL 报告给该设置多个'F'评级的幽默之处，以及这对构建超兼容网站的实际用途。

**标签**: `#cryptography`, `#security`, `#retrocomputing`, `#RSA`

---

<a id="item-2"></a>
## [llm CLI 工具 0.35 版本新增对 OpenAI GPT-6 Astra 模型的支持。](https://simonwillison.net/2026/Sep/7/llm/) ⭐️ 8.0/10

llm 命令行工具发布了 0.35 版本，其核心更新是新增了对 OpenAI 新款旗舰模型 GPT-6 Astra 的支持，对应的模型代码为 `gpt-6-astra`。 此次集成使得使用流行 llm CLI 工具的开发者和研究人员能够立即访问并试验 OpenAI 最先进的模型，该模型专门针对复杂的、长周期的智能体任务、科学工作和计算机操作进行了优化。这代表了一次快速工具更新，确保了开发者生态与前沿 AI 能力保持同步。 此次更新内容简洁，主要是在工具的配置中添加了新的模型标识符。GPT-6 Astra 以其在智能体工作流、高级分析和计算机操作能力方面的优势而著称，但其效益取决于具体任务，因为它是专门为此类长周期和科学应用进行调优的。

rss · Simon Willison · Sep 7, 23:54

**背景**: llm 是由 Simon Willison 创建的一个命令行界面（CLI）工具和 Python 库，用于与 OpenAI、Anthropic、Google 等提供商的各种大型语言模型（LLM）进行交互。它简化了从终端或脚本中直接向 LLM 发送提示词和接收响应的过程。GPT-6 Astra 是 OpenAI 最新的旗舰模型，定位为处理复杂、多步骤智能体任务的重大进步，这些任务涉及使用计算机和浏览器、深度研究和科学工作。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://llm.datasette.io/en/latest/">LLM : A CLI utility and Python library for interacting with Large...</a></li>
<li><a href="https://github.com/simonw/llm">GitHub - simonw/ llm : Access large language models from the...</a></li>
<li><a href="https://openrouter.ai/openai/gpt-6-astra">GPT - 6 Astra - API Pricing & Benchmarks | OpenRouter</a></li>

</ul>
</details>

**标签**: `#openai`, `#llm`, `#gpt-6-astra`, `#cli`, `#ai-tools`

---

<a id="item-3"></a>
## [华为发布采用逻辑折叠架构的麒麟 9050 Pro 芯片](https://www.news.cn/20260907/adf46c5c003240d28cc3cf6de54f9b5f/c.html) ⭐️ 8.0/10

华为于 9 月 7 日发布了其新款旗舰芯片麒麟 9050 Pro，这是首款采用新型“逻辑折叠”架构的芯片。该芯片随 Mate XT 2 三折叠手机一同亮相，标志着华为自 Mate40 系列后时隔六年重返高性能芯片开发领域。 此次发布标志着华为在高端半导体领域的一次重大技术回归，可能对现有的市场领导者构成挑战。逻辑折叠架构代表了一项旨在克服传统微缩极限的重大创新，可能影响未来以提高性能和能效为目标的芯片设计趋势。 逻辑折叠架构通过内部“垂直互联通道”垂直堆叠芯片层，类似于加装“电梯”，以缩短信号路径、降低时延并提升性能。据报道，该设计在不依赖 EUV 光刻技术的情况下，实现了相比前代芯片 55% 的晶体管密度提升，但详细的性能基准测试数据尚未公布。

telegram · zaihuapd · Sep 7, 08:20

**背景**: 华为的麒麟芯片是其为智能手机设计的自研系统级芯片（SoC），但由于美国贸易限制导致其难以获得先进制造能力，其发展曾面临重大挑战。逻辑折叠是一种新颖的 3D 芯片设计方法，通过垂直堆叠逻辑单元来提高密度和性能，以应对传统 2D 平面微缩（摩尔定律）的局限。垂直互联通道，如硅通孔（TSV），是通过在堆叠层之间建立电气连接来实现此类 3D 集成的关键技术。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.huaweicentral.com/huawei-logicfolding-architecture-everything-you-need-to-know/">Huawei LogicFolding Architecture: Everything you need to know</a></li>
<li><a href="https://www.techtimes.com/articles/326836/20260907/huawei-kirin-9050-pro-launches-logicfolding-moves-roadmap-silicon.htm">Huawei Kirin 9050 Pro Launches: LogicFolding Moves From Roadmap to Silicon</a></li>
<li><a href="https://en.wikipedia.org/wiki/Through-silicon_via">Through-silicon via - Wikipedia</a></li>

</ul>
</details>

**标签**: `#semiconductors`, `#mobile-technology`, `#hardware-innovation`, `#huawei`

---

<a id="item-4"></a>
## [中国最高人民法院发布司法解释，明确 AI 纠纷中换脸、算法杀熟等责任](https://www.cnr.cn/news/20260907/t20260907_527806795.shtml) ⭐️ 8.0/10

9 月 7 日，中国最高人民法院发布了关于人工智能纠纷案件的司法解释，共 5 部分 24 条。该解释明确，未经同意使用 AI 制作可识别的人脸、声音等可能构成人格权侵权；实施算法价格歧视或利用 AI 冒充他人代言诱导消费的，应承担相应责任，并可依法支持惩罚性赔偿请求。 这是全球首批由最高法院直接针对深度伪造、算法歧视等新兴 AI 危害责任发布的综合性司法指南之一。它为受害者、平台和开发者提供了关键的法律确定性，并可能影响全球 AI 治理和责任框架的规范形成。 该司法解释还依法规制了利用 AI 实施“网络开盒”、“人肉搜索”等侵害自然人隐私权的行为。其内容广泛，涵盖了自动驾驶、知识产权等问题，为复杂的 AI 纠纷提供了结构化的法律处理路径。

telegram · zaihuapd · Sep 7, 09:32

**背景**: 深度伪造（Deepfake）指利用 AI 生成的合成媒体，如视频或音频，能够逼真地冒充真人，引发了关于同意、欺诈和诽谤的担忧。算法价格歧视，俗称“大数据杀熟”，是指在线平台利用算法，基于用户的数据画像，对同一商品或服务向不同用户收取不同价格的行为。AI 冒充是指利用 AI 模仿他人的形象或声音，通常用于虚假代言或诈骗等欺骗性目的。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://stackcyber.com/posts/ai-deepfake-laws">Deepfake Legislation Tracker: Federal, State Laws</a></li>
<li><a href="https://lawreview.uchicago.edu/print-archive/algorithmic-price-discrimination-when-demand-function-both-preferences-and">Algorithmic Price Discrimination When Demand Is a Function of Both Preferences and (Mis)perceptions | The University of Chicago Law Review</a></li>
<li><a href="https://www.aol.com/articles/companies-increasingly-falling-victim-ai-170000990.html">Companies are increasingly falling victim to AI impersonation ... - AOL</a></li>

</ul>
</details>

**标签**: `#AI Regulation`, `#Legal Tech`, `#Algorithmic Bias`, `#Deepfakes`, `#Autonomous Vehicles`

---

<a id="item-5"></a>
## [联合国环境规划署报告预测全球升温峰值约 1.8°C，将突破《巴黎协定》1.5°C 目标](http://www.unep.org/resources/limiting-overshoot-navigating-exceedance) ⭐️ 8.0/10

联合国环境规划署的一份新报告指出，根据当前的排放轨迹，本世纪全球升温峰值预计将达到约 1.8°C，这将突破《巴黎协定》设定的 1.5°C 长期温控目标。报告负责人承认，各国当前的减排行动速度未能达到所需水平。 这一预测至关重要，因为突破 1.5°C 阈值将大幅增加触发危险且可能不可逆转的气候临界点的风险，例如冰盖崩塌或洋流发生重大转变。这些发现凸显了当前气候政策与实现国际气候目标所需行动之间的巨大差距，强调了全球采取更雄心勃勃的减缓行动的紧迫性。 报告特别警告，一旦超过 1.5°C 的阈值，气候系统触发危险临界点的风险将会加剧。值得注意的是，这一预测是基于当前的政策和轨迹，意味着通过果断且加速的全球行动，结果仍然可以改变。

telegram · zaihuapd · Sep 8, 03:05

**背景**: 1.5°C 目标是《巴黎协定》——一项于 2015 年通过的国际气候变化条约——确立的关键长期温控目标。主要由政府间气候变化专门委员会汇编的科学评估表明，升温超过 1.5°C 会显著增加严重气候影响的风险。气候临界点是地球系统中的一些阈值，一旦被突破，可能导致大规模、快速且通常不可逆转的变化，例如格陵兰冰盖融化或亚马逊雨林退化。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.unep.org/resources/emissions-gap-report">Emissions Gap Report</a></li>
<li><a href="https://www.umweltbundesamt.de/en/topics/climate-energy/the-15degc-goal-of-the-paris-agreement">The 1.5°C goal of the Paris Agreement | Umweltbundesamt</a></li>
<li><a href="https://en.wikipedia.org/wiki/Tipping_points_in_the_climate_system">Tipping points in the climate system - Wikipedia</a></li>

</ul>
</details>

**标签**: `#climate-change`, `#environmental-science`, `#policy`, `#sustainability`

---

<a id="item-6"></a>
## [美国审查中国 AI 企业海外获取英伟达芯片渠道，包括远程云访问](https://t.me/zaihuapd/43676) ⭐️ 8.0/10

美国商务部工业与安全局（BIS）正系统性审查中国 AI 企业如何在海外获取和使用英伟达芯片，包括通过租用其他国家算力的远程访问方式。此次审查是在一名白宫高官公开指控月之暗面（Moonshot AI）通过泰国一方远程访问非法获取英伟达芯片后几天内启动的。 此次审查是美国针对中国执行半导体出口管制的一次重大升级，直接瞄准了可能削弱现有制裁效力的法律灰色地带。此举可能严重限制中国 AI 企业获取训练先进模型（如拥有 2.8 万亿参数的 Kimi K3）所需的关键算力，影响全球 AI 竞赛和云计算市场格局。 审查内容包括整理两份国家名单：涉嫌将受限芯片走私入境中国的黑市所在地，以及中国企业远程租用芯片的国家。一个关键的法律问题是 BIS 是否有权限制此类远程云访问，因为根据现行规则，远程访问芯片本身并不违法。

telegram · zaihuapd · Sep 8, 03:35

**背景**: 美国工业与安全局（BIS）负责执行包括半导体在内的先进技术出口管制，以保护国家安全。英伟达的高性能 GPU 对于训练最先进的 AI 模型至关重要，但受到对中国的严格出口限制。据报道，中国 AI 公司（如月之暗面）一直在寻求通过提供远程 GPU 访问的海外数据中心或云服务来获取替代性算力，这种做法处于监管的灰色地带。月之暗面近期发布了 Kimi K3 模型，这是一个拥有 2.8 万亿参数的巨型开源模型，其性能可与美国领先模型相媲美。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.bis.gov/">Homepage | Bureau of Industry and Security</a></li>
<li><a href="https://en.wikipedia.org/wiki/Kimi_(AI)">Kimi (AI) - Wikipedia</a></li>
<li><a href="https://cloud.google.com/gpu">Cloud GPUs (Graphics Processing Units) | Google Cloud</a></li>

</ul>
</details>

**标签**: `#AI Regulation`, `#Semiconductor Export Controls`, `#US-China Tech Competition`, `#Geopolitics`, `#Cloud Computing`

---

<a id="item-7"></a>
## [字节跳动讨论训练参数规模超 5 万亿的大语言模型](https://t.me/zaihuapd/43677) ⭐️ 8.0/10

据报道，字节跳动正就训练一个参数规模超 5 万亿的大语言模型进行早期讨论，该项目由 Seed Foundation 负责人项亮主导，并与大语言模型预训练数据负责人沈科合作。若该计划落地，其规模将超越阿里的 Qwen 3.8-Max（2.4 万亿参数）和月之暗面的 K3，成为国内已知参数规模最大的模型。 此举标志着字节跳动加码追求 AI 能力上限，直接挑战其他中国科技巨头在更大、更强模型领域的竞争。一个成功的 5 万亿参数模型可能显著推动 AI 在复杂推理和编程等领域的发展，同时重塑基础模型的竞争格局。 该计划目前仍处于早期讨论阶段，尚未最终确定。字节跳动联合创始人张一鸣在近期的一次全员会上明确反对'蒸馏'路线，认为其只是复制 Claude 等模型的已有能力，并鼓励团队以追求智能上限为目标，接受短期落后以打造有特色的模型。

telegram · zaihuapd · Sep 8, 04:05

**背景**: 字节跳动 Seed 是该公司的基础模型研究部门，成立于 2023 年，致力于探索通用智能的新方法。模型蒸馏是一种将知识从庞大复杂的'教师'模型转移到更小、更高效的'学生'模型的技术。目前国内已知参数规模最大的模型是阿里巴巴于 2026 年 8 月发布的 Qwen 3.8-Max，其拥有 2.4 万亿参数。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://seed.bytedance.com/">ByteDance Seed</a></li>
<li><a href="https://en.wikipedia.org/wiki/Knowledge_distillation">Knowledge distillation - Wikipedia</a></li>
<li><a href="https://openlm.ai/qwen3.8/">Qwen3.8 | OpenLM.ai</a></li>

</ul>
</details>

**标签**: `#AI`, `#Large Language Models`, `#ByteDance`, `#Machine Learning`, `#Industry News`

---