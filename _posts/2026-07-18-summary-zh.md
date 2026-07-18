---
layout: default
title: "Horizon Summary: 2026-07-18 (ZH)"
date: 2026-07-18
lang: zh
---

> From 27 items, 7 important content pieces were selected

---

1. [首次在宜居带内的类地岩石行星 LHS 1140 b 上探测到大气层。](#item-1) ⭐️ 9.0/10
2. [月之暗面开源 Kimi K3，这是一个具备原生视觉和 100 万上下文窗口的 2.8 万亿参数模型，在 Frontend Code Arena 中排名第一。](#item-2) ⭐️ 9.0/10
3. [Kimi K3 在 pelican 基准测试中的分析揭示了隐藏提示与分词差异。](#item-3) ⭐️ 8.0/10
4. [开源 AI 模型市场份额超越闭源模型，增长势头迅猛](#item-4) ⭐️ 8.0/10
5. [华为昇腾 950 超节点首次公开亮相，算力达英伟达同级系统 6.7 倍](#item-5) ⭐️ 8.0/10
6. [Meta 拟向 Anthropic 出租 AI 算力，潜在两年期交易规模高达 1000 亿美元。](#item-6) ⭐️ 8.0/10
7. [SpaceX 正与五角大楼谈判数十亿美元的 AI 算力交易](#item-7) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [首次在宜居带内的类地岩石行星 LHS 1140 b 上探测到大气层。](https://www.bbc.com/news/articles/cy4kdd1e0ejo) ⭐️ 9.0/10

天文学家首次探测到一颗名为 LHS 1140 b 的岩石、地球大小的系外行星拥有大气层，该行星位于其母恒星的宜居带内，这颗红矮星距离地球 48 光年。这一发现是通过詹姆斯·韦伯太空望远镜（JWST）实现的。 这一发现是寻找太阳系外宜居世界的一个重要里程碑，因为大气层的存在是潜在地表液态水和已知生命形式的关键先决条件。它证明了 JWST 有能力对小型岩石行星的大气进行表征，极大地推动了天体生物学领域的发展。 该行星围绕一颗温度较低的红矮星运行，这类恒星以剧烈的恒星活动而闻名，可能剥离行星的大气层，因此这次探测显得尤为引人注目。包括行星从恒星后方经过时的发射光谱在内的初步观测，已经排除了 LHS 1140 b 是一颗气态"迷你海王星"的可能性。

hackernews · neversaydie · Jul 17, 14:06 · [社区讨论](https://news.ycombinator.com/item?id=48947560)

**背景**: 系外行星是指围绕太阳以外的恒星运行的行星。'宜居带'是指恒星周围的一个区域，该区域的条件可能允许液态水存在于行星表面，而水是生命的关键成分。詹姆斯·韦伯太空望远镜（JWST）于 2021 年发射，是一台强大的红外天文台，通过研究穿过行星大气的星光来分析其成分，在这方面具有独特优势。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.bbc.com/news/articles/cy4kdd1e0ejo">First atmosphere found around Earth-like planet LHS 1140b - BBC</a></li>
<li><a href="https://science.nasa.gov/exoplanets/habitable-zone/">The Habitable Zone - NASA Science</a></li>
<li><a href="https://www.pnas.org/doi/10.1073/pnas.2416190122">A first look at rocky exoplanets with JWST | PNAS</a></li>

</ul>
</details>

**社区讨论**: 社区讨论突出了技术性辩论，包括对一颗围绕活跃红矮星运行的岩石行星能否保有大气层的质疑，并有澄清指出 JWST 数据已排除了气态"迷你海王星"的假说。成员们还推测了未来的技术，如太阳透镜望远镜和星际探测器，而另一些人则思考了这对费米悖论的影响，指出技术文明可被探测到的时间窗口可能极其短暂。

**标签**: `#astronomy`, `#exoplanets`, `#astrobiology`, `#space-exploration`, `#jwst`

---

<a id="item-2"></a>
## [月之暗面开源 Kimi K3，这是一个具备原生视觉和 100 万上下文窗口的 2.8 万亿参数模型，在 Frontend Code Arena 中排名第一。](https://t.me/zaihuapd/42637) ⭐️ 9.0/10

月之暗面（Moonshot AI）发布并开源了 Kimi K3，这是一个基于创新的 Kimi Delta Attention (KDA) 和 Attention Residuals 架构构建的 2.8 万亿参数模型，具备原生视觉理解能力和 100 万 token 的上下文窗口。在第三方基准测试 Frontend Code Arena 中，K3 以 1679 分的成绩超越 Claude Fable 5 等模型，跃居榜首。 此次发布标志着全球首个 3 万亿参数级别的开源模型诞生，极大地降低了获取前沿规模 AI 的门槛，有望加速相关研究和应用开发。其在竞争激烈的前端编程基准测试中的领先表现，证明了其在代码生成这一 AI 辅助软件开发关键领域的强大能力。 该模型采用了混合线性注意力架构，每 1 个完整注意力层搭配 3 个 KDA 层，以优化性能与效率之间的平衡。虽然在 Frontend Code Arena 的 7 个评测领域中 6 项居首，但据报道在游戏领域表现落后。

telegram · zaihuapd · Jul 18, 02:29

**背景**: Kimi Delta Attention (KDA) 是一种新颖的线性注意力机制，它改进了 Gated DeltaNet 架构，引入了逐通道衰减控制，以实现更精确的内存管理。Frontend Code Arena 是一个专注于评估 AI 模型在前端工程和代码生成任务中能力的竞争性基准测试。Attention Residuals (AttnRes) 是一种技术，它使模型能够选择性地从之前的层中检索信息，而不是均匀地累积，从而起到提升计算效率的作用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2510.26692">Kimi Linear: An Expressive, Efficient Attention Architecture Kimi K3 - Kimi API Platform GitHub - MoonshotAI/Kimi-Linear Images hwilner/kimi-delta-attention - GitHub Kimi Linear: An Expressive, Efficient Attention Architecture Linear Attention: Kimi Delta Attention | Jianyu Huang Moonshot AI Releases Kimi K3: A 2.8 Trillion Parameter Open ...</a></li>
<li><a href="https://officechai.com/ai/kimi-k3-beats-fable-5-gpt-5-6-sol-on-frontend-code-arena/">Kimi K3 Beats Fable 5, GPT 5.6 Sol On Frontend Code Arena</a></li>
<li><a href="https://xhinker.medium.com/attention-residuals-attnres-from-kimi-ai-complete-deep-dive-in-plain-language-dd84b4035957">Attention Residuals (AttnRes) from Kimi. ai : Complete Deep... | Medium</a></li>

</ul>
</details>

**标签**: `#Large Language Models`, `#Open Source AI`, `#AI Benchmarking`, `#Frontend Programming`, `#Computer Vision`

---

<a id="item-3"></a>
## [Kimi K3 在 pelican 基准测试中的分析揭示了隐藏提示与分词差异。](https://simonwillison.net/2026/Jul/16/kimi-k3/) ⭐️ 8.0/10

对 Kimi K3 模型在非正式 'pelican 基准测试'（提示词为 '生成一只鹈鹕骑自行车的 SVG'）上的表现进行技术分析，发现了存在隐藏系统提示的证据，以及与其他模型相比显著的令牌计数差异。该分析还强调了这一简单测试如何能揭示模型行为的细节以及当前大语言模型评估方法的局限性。 这很重要，因为它展示了简单、非常规的基准测试如何能暴露隐藏的实现细节，如系统提示和分词策略，而这些细节对用户通常是不透明的。它强调需要更细致的评估方法，超越传统指标，以理解模型在真实世界中的行为、成本和速度之间的权衡。 向 Kimi K3 发送 'hi' 提示词被计为 86 个输入令牌，这表明存在一个约 85 个令牌的隐藏系统提示，很可能是一个推理努力提示。核心鹈鹕提示词的令牌计数在不同模型间差异巨大（例如，OpenAI 模型计为 10 个令牌，Claude Opus 4.7 计为 30 个），突显了分词差异如何影响成本和性能比较。

hackernews · droidjj · Jul 17, 14:21 · [社区讨论](https://news.ycombinator.com/item?id=48947717)

**背景**: '鹈鹕骑自行车' 是由开发者 Simon Willison 创建的一个针对大语言模型的非正式基准测试，基于单一提示词 '生成一只鹈鹕骑自行车的 SVG'。它评估大语言模型遵循指令、理解空间关系以及生成结构化 SVG 代码的能力。系统提示是随用户输入一起发送的隐藏指令，用于指导模型行为。分词是将文本分解为模型处理单元（令牌）的过程，它直接影响成本和性能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/simonw/pelican-bicycle">GitHub - simonw/pelican-bicycle: LLM benchmark: Generate an SVG of a pelican riding a bicycle · GitHub</a></li>
<li><a href="https://grokipedia.com/page/Pelican_on_a_bicycle_AI_benchmark">Pelican on a bicycle (AI benchmark) — Grokipedia</a></li>
<li><a href="https://learn.snyk.io/lesson/llm-system-prompt-leakage/">System prompt leakage in LLMs | Tutorial and examples | Snyk Learn</a></li>

</ul>
</details>

**社区讨论**: 社区讨论围绕鹈鹕图像是否真的不在训练数据中展开了辩论，鉴于其在网上的普遍性。用户强调了该基准测试在比较 Kimi、Claude Opus 和 Fable 等模型之间的成本与速度权衡方面的实用性。也有人对该基准测试的单次运行性质及其无法评估更关键的'智能体'能力（如在长对话中可靠使用工具）表示担忧。

**标签**: `#llm`, `#benchmarking`, `#ai-evaluation`, `#tokenization`, `#prompt-engineering`

---

<a id="item-4"></a>
## [开源 AI 模型市场份额超越闭源模型，增长势头迅猛](https://stateofopensource.ai/) ⭐️ 8.0/10

基于 OpenRouter 数据的分析显示，开源 AI 模型市场份额迅速增长，在短短四个月内从落后于闭源模型（60%对 40%）转变为领先（63%对 37%）。开源模型处理的聚合令牌量激增近 5 倍，从 3 月 19 日的 8880 亿枚增长到最近的 4.19 万亿枚。 这一转变标志着一个重要的行业趋势，即开源模型正成为成本效益高、灵活且透明的 AI 部署的首选，可能挑战 OpenAI 和 Anthropic 等专有供应商的主导地位。超大规模云提供商和设备制造商的快速采用可能会重塑竞争格局，并加速设备端 AI 应用的发展。 该数据来源于 OpenRouter 平台，该平台聚合了对各种 AI 模型的访问，为现实世界的使用趋势提供了一个参考指标。需要注意的是，许多流行的“开源”模型在技术上是“开放权重”的，这意味着其模型权重是公开的，但完整的训练代码和数据可能并未公开，这影响了真正的开放性和可审计性。

hackernews · rellem · Jul 17, 14:31 · [社区讨论](https://news.ycombinator.com/item?id=48947825)

**背景**: 开源 AI 模型的架构和权重通常是公开可用的，这与 GPT-4 或 Claude 等闭源模型形成对比，后者是专有的，只能通过 API 访问。OpenRouter 是一项服务，充当了来自不同提供商的众多 AI 模型的统一接口，允许用户轻松比较和切换模型。开源与闭源模型之间的争论通常围绕成本、控制权、透明度以及特定任务的性能展开。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openrouter.ai/">OpenRouter</a></li>
<li><a href="https://editorialge.com/open-vs-closed-ai-models/">Open Vs Closed AI Models : Which is Best for Regulated Workloads?</a></li>
<li><a href="https://huggingface.co/blog/daya-shankar/open-source-llms">Best Open - Source LLM Models in 2026: Coding, Local, Agentic AI ...</a></li>

</ul>
</details>

**社区讨论**: 社区情绪复杂，一些人认为开源模型的崛起对闭源模型公司构成生存威胁，因为其在成本和灵活性上对超大规模云提供商和设备制造商更具优势。另一些人则批评源分析报告的呈现风格过于通用，很可能是 AI 生成的，质疑此类报告背后高管洞察的深度。一个被强调的关键数据点是开源模型的令牌量在四个月内实现了惊人的 5 倍增长。

**标签**: `#open-source`, `#artificial-intelligence`, `#market-trends`, `#llm`, `#data-analysis`

---

<a id="item-5"></a>
## [华为昇腾 950 超节点首次公开亮相，算力达英伟达同级系统 6.7 倍](https://www.ithome.com/0/978/019.htm) ⭐️ 8.0/10

在 2026 世界人工智能大会（WAIC）上，华为首次公开亮相了其昇腾 950 超节点（Atlas 950 SuperPoD）AI 计算系统真机。据中银证券报告，该系统提供 1 EFLOPS FP8 和 2 EFLOPS FP4 算力，其总算力据称达到了英伟达搭载 144 张卡的同级别 NVL144 系统的 6.7 倍。 此次发布是对英伟达在高性能 AI 计算基础设施领域主导地位的一次重大挑战，尤其是在难以获取英伟达最新技术的市场。如果其性能宣称得到验证，该系统将为训练下一代大型 AI 模型提供一个强大且可扩展的替代方案，可能重塑 AI 硬件的竞争格局。 该系统基于华为自研的灵衢（UnifiedBus）互联协议和超节点架构，支持业界最大的 1024 卡规模，并拥有 256 TB 的全局统一内存。华为还指出，更早的昇腾 384 超节点已商用落地 750 多套，并同期展出了 Atlas 850E 风冷超节点，企业无需液冷改造即可在标准风冷机房部署。

telegram · zaihuapd · Jul 17, 10:27

**背景**: 昇腾 950 超节点是一个大规模 AI 计算集群，它使用华为自研的灵衢互联协议，将数千个昇腾神经网络处理器（NPU）连接成一台逻辑上的单一机器。EFLOPS 是衡量计算性能的单位，表示每秒进行一百亿亿次（10^18）浮点运算，而 FP8 和 FP4 是用于 AI 训练和推理的低精度数值格式，旨在提升速度和能效。英伟达的 NVL 系统是其用于大规模 AI 训练的旗舰平台，通过高速 NVLink 互连技术连接多张 GPU。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.itbear.com.cn/html/2025-09/960596.html">华为发布灵衢互联协议与系列超节点，引领AI算力基础设施新变革-人工智能-ITBear科技资讯</a></li>
<li><a href="https://lucaberton.com/blog/huawei-atlas-950-superpod-ai-infrastructure/">Huawei Atlas 950 AI SuperPoD : 8,192 NPUs as One Machine</a></li>
<li><a href="https://lambda.ai/blog/the-essential-guide-to-gpus">The Essential Guide to GPUs for AI, Training and Inference</a></li>

</ul>
</details>

**标签**: `#AI Hardware`, `#High-Performance Computing`, `#Huawei`, `#NVIDIA`, `#AI Infrastructure`

---

<a id="item-6"></a>
## [Meta 拟向 Anthropic 出租 AI 算力，潜在两年期交易规模高达 1000 亿美元。](https://www.nytimes.com/2026/07/17/technology/meta-anthropic-ai-computing-power.html) ⭐️ 8.0/10

Meta 正与 AI 初创公司 Anthropic 进行早期谈判，拟将其 AI 数据中心算力出租给后者，潜在交易规模高达 1000 亿美元，为期两年。该方案由 Anthropic 于今年 6 月提出，若达成协议，Anthropic 将按月付款，且双方均可提前退出。 这笔潜在交易凸显了 AI 算力的严重短缺，这已成为 AI 发展的关键瓶颈。对 Meta 而言，这标志着一个战略转变，可能从其巨额基础设施投资中开辟重要的新收入来源，同时也为 Anthropic 提供了扩展其 AI 模型所需的关键资源。 交易尚未最终确定，谈判仍处于早期阶段。Meta 今年计划投入高达 1450 亿美元，其中大量资金用于 AI 与数据中心建设，这为其出租闲置算力创造了潜在条件。

telegram · zaihuapd · Jul 18, 01:14

**背景**: AI 算力指的是训练和运行大型 AI 模型所需的专用硬件（如 GPU）及相关数据中心基础设施。目前这些资源出现严重短缺，据报道 GPU 租赁价格已大幅上涨。Anthropic 是一家领先的 AI 公司，以开发 Claude 系列大语言模型而闻名。为了获得稳定的 AI 基础设施访问权，企业之间签订长期租赁协议的趋势日益明显。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://tomtunguz.com/ai-compute-crisis-2026/">The Beginning of Scarcity in AI | Tomasz Tunguz</a></li>
<li><a href="https://en.wikipedia.org/wiki/Anthropic">Anthropic - Wikipedia</a></li>
<li><a href="https://www.globaldatacenterhub.com/p/why-metas-26b-leaseback-rewrote-ai">Why Meta's $26B Leaseback Rewrote AI Infrastructure Financing</a></li>

</ul>
</details>

**标签**: `#AI Infrastructure`, `#Cloud Computing`, `#Business Strategy`, `#Generative AI`, `#Meta`

---

<a id="item-7"></a>
## [SpaceX 正与五角大楼谈判数十亿美元的 AI 算力交易](https://www.wsj.com/tech/ai/spacex-in-talks-to-provide-computing-power-for-pentagons-ai-push-15e752e4) ⭐️ 8.0/10

SpaceX 正与美国国防部谈判，拟向其提供数据中心算力以运行人工智能模型，潜在交易金额高达数十亿美元。谈判仍在进行中，存在破裂可能，但若达成协议，这将是 SpaceX 与五角大楼关系深化的最新一笔重大交易。 这笔交易意义重大，标志着 SpaceX 正式进军利润丰厚且具有关键战略意义的国防 AI 基础设施市场，直接与老牌云巨头竞争。它也凸显了五角大楼为国家安全和军事行动获取先进、机密云与 AI 能力的迫切需求。 五角大楼近期已批准 SpaceX 以及亚马逊、谷歌、微软和甲骨文等公司在机密环境中使用其 AI 模型及相关技术。SpaceX 近几个月还与 Anthropic 和谷歌签署了类似的算力供应协议，这表明其云计算业务正在大幅扩张。

telegram · zaihuapd · Jul 18, 01:44

**背景**: SpaceX 主要以火箭发射和 Starlink 卫星互联网闻名，现正通过出售其过剩的 AI 算力来扩展云计算业务。机密计算是一种云技术，它利用基于硬件的可信执行环境（TEE）在处理过程中保护数据，这对于处理敏感的政府和军事数据至关重要。五角大楼推动 AI 应用，是其更广泛的 IT 基础设施现代化和利用 AI 服务于各种国防应用努力的一部分。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.cloud.google.com/confidential-computing/docs/confidential-computing-overview">Confidential Computing overview | Google Cloud Documentation</a></li>
<li><a href="https://techcrunch.com/2026/07/01/meta-like-spacex-looks-to-turn-excess-ai-compute-into-cash/">Meta, like SpaceX, looks to turn excess AI compute into cash</a></li>

</ul>
</details>

**标签**: `#AI Infrastructure`, `#Defense Technology`, `#Cloud Computing`, `#SpaceX`, `#Public Sector AI`

---