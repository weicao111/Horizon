---
layout: default
title: "Horizon Summary: 2026-07-15 (ZH)"
date: 2026-07-15
lang: zh
---

> From 32 items, 8 important content pieces were selected

---

1. [美国批准英伟达 H200 AI 芯片向阿里巴巴、腾讯等中国主要科技公司销售](#item-1) ⭐️ 9.0/10
2. [Bonsai 27B：一个可运行在手机上的 270 亿参数压缩模型](#item-2) ⭐️ 8.0/10
3. [Cloudflare 推出 Precursor，通过持续行为验证引擎识别 AI 机器人和脚本。](#item-3) ⭐️ 8.0/10
4. [DeepSeek 完成超 500 亿元首轮融资，采用特殊架构维持创始人控制权。](#item-4) ⭐️ 8.0/10
5. [高德发布世界模型工坊 ABot-WorldStudio，内置'时空任意门'可生成交互式 3D 世界](#item-5) ⭐️ 8.0/10
6. [Telegram 短链接域名 t.me 遭注册局以 serverHold 状态冻结。](#item-6) ⭐️ 8.0/10
7. [DeepMind CEO 呼吁美国主导成立拥有发布前评估权的全球 AI 监管机构](#item-7) ⭐️ 8.0/10
8. [白宫将召集电力公司与数据中心开发商，推动自愿承诺以应对 AI 用电成本。](#item-8) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [美国批准英伟达 H200 AI 芯片向阿里巴巴、腾讯等中国主要科技公司销售](https://t.me/zaihuapd/42567) ⭐️ 9.0/10

美国商务部已批准向约 10 家中国主要企业销售英伟达 H200 AI 芯片，买家包括阿里巴巴、腾讯、字节跳动、京东等，联想和富士康等分销商也获得许可，单一客户最多可购买 7.5 万颗。但截至目前尚未有任何交付完成，部分中国企业在政府指导下转趋谨慎。 这一批准标志着中美高科技竞争中出现了一次重大且具体的政策调整，通过允许中国科技巨头获得尖端硬件，直接影响了全球 AI 基础设施竞赛。它凸显了美国出口管制政策、英伟达在关键市场的商业策略，以及中国在进口高端芯片与发展国产 AI 芯片之间权衡的复杂互动。 获批的 H200 芯片是英伟达最新的高性能 AI GPU，拥有 141 GB 的 HBM3e 内存，性能显著提升，例如相比旧的 A100 GPU，其 AI 模型微调速度可加快 5.5 倍。英伟达 CEO 黄仁勋最近的访华之行，被视为在持续的地缘政治紧张和监管审查下推动这些交易落地的重要尝试。

telegram · zaihuapd · Jul 15, 00:14

**背景**: 英伟达 H200 是一款为数据中心设计的尖端 AI 加速器 GPU，是 H100 的后续产品，是训练和运行大语言模型（LLM）及其他高要求 AI 工作负载的关键工具。出于国家安全考虑，美国政府实施了一系列不断演变的出口管制，例如“人工智能扩散框架”，旨在限制先进半导体和 AI 技术向包括中国在内的某些国家流动。这些管制为英伟达等希望在中国市场销售产品的公司创造了复杂的许可环境。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.nvidia.com/en-us/data-center/h200/">H200 GPU | NVIDIA</a></li>
<li><a href="https://media.bis.gov/sites/default/files/documents/05.07+Recission+of+AI+Diffusion+Press+Release.pdf">Department of Commerce Announces Rescission of Biden-Era ...</a></li>

</ul>
</details>

**标签**: `#AI Hardware`, `#Geopolitics`, `#Supply Chain`, `#Nvidia`, `#US-China Relations`

---

<a id="item-2"></a>
## [Bonsai 27B：一个可运行在手机上的 270 亿参数压缩模型](https://prismml.com/news/bonsai-27b) ⭐️ 8.0/10

PrismML 发布了 Bonsai 27B，这是 Qwen3.6-27B 模型的压缩版本，它采用 1-bit 和三元量化技术，将模型大小从约 50GB 压缩至 4GB 以下。这种压缩使得这个拥有 270 亿参数的模型能够在智能手机和笔记本电脑等移动设备上本地运行。 这代表了设备端人工智能领域的一次重大进展，可能重塑关于边缘设备能运行多大模型的假设。它使得更强大、更私密、更低延迟的 AI 应用能够直接在个人设备上运行，减少了对云端的依赖。 该模型提供 1-bit 和三元（值为 -1, 0, 1）量化版本，PrismML 声称其 1-bit 版本是首个能装入手机的 270 亿参数级别模型。然而，社区早期尝试在 LM Studio 等工具中运行其提供的 GGUF 或 MLX 文件时遇到了兼容性问题。

hackernews · xenova · Jul 14, 17:50 · [社区讨论](https://news.ycombinator.com/item?id=48910545)

**背景**: 像 270 亿参数的 Qwen 这样的大型语言模型计算成本高且内存占用大。量化是一种关键的压缩技术，它通过降低模型权重的数值精度（例如，从 16 位浮点数降至 4 位或 1 位整数），从而大幅减少其内存占用，使其能够在资源受限的设备上实现更快的推理。设备端推理因其数据隐私性、低延迟和离线功能等优势而备受关注。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.marktechpost.com/2026/07/14/prismml-releases-bonsai-27b-1-bit-and-ternary-builds-of-qwen3-6-27b-that-run-on-laptops-and-phones/">PrismML Releases Bonsai 27B: 1-bit and Ternary Builds of ...</a></li>
<li><a href="https://medium.com/@techresearchspace/what-is-quantization-in-llm-01ba61968a51">What is Quantization in LLM. Large Language Models comes in all… | by Nithin Devanand | Medium</a></li>
<li><a href="https://arxiv.org/abs/2409.00088">On-Device Language Models: A Comprehensive Review On-device large language models: a survey of model ... - Springer On-Device LLM Inference: The Definitive 2025-2026 Guide Fast On-device LLM Inference with NPUs | Proceedings of the ... Optimizing Inference for On-Device SLMs: A Guide to Local LLM ... On-Device Language Models: A Comprehensive Review</a></li>

</ul>
</details>

**社区讨论**: 社区讨论聚焦于将该模型与其他高效模型（如量化版的 Gemma 2 12B）进行实际比较，质疑其在工具调用能力上的性能取舍，并指出了与当前软件的集成挑战。此外，关于苹果公司与 PrismML 就这项用于 iPhone 的压缩技术进行谈判的报道也引起了显著关注。

**标签**: `#llm`, `#model-compression`, `#mobile-ai`, `#quantization`, `#on-device`

---

<a id="item-3"></a>
## [Cloudflare 推出 Precursor，通过持续行为验证引擎识别 AI 机器人和脚本。](https://blog.cloudflare.com/introducing-precursor/) ⭐️ 8.0/10

Cloudflare 于 7 月 13 日发布了新产品 Precursor，这是一个“持续行为验证”引擎。它通过客户端 JavaScript 在整个用户会话中持续监控，分析鼠标移动轨迹、键盘节奏、认知停顿等信号，以实时区分真人和脚本或 AI 代理。该产品定位为现有 Turnstile 服务的可选补充，目前面向企业版 Bot Management 用户提供免费测试，正式版计划于今年晚些时候上线。 这很重要，因为它代表了机器人和 AI 安全领域的重大演进，从一次性检查（如验证码）转向基于难以伪造的人类行为生物特征的持续、被动验证。随着 AI 代理日益复杂，这项技术对于保护网站和应用免受自动化欺诈、爬取和滥用至关重要，同时不会干扰合法用户体验。 Precursor 专注于机器难以模仿的生理信号，例如手腕带动鼠标产生的自然弧线轨迹以及思考时的微小延迟。收集的数据会被整理成基于会话的分析面板，并且该系统在设计上考虑了隐私因素，信号在 Cloudflare 的机器人保护基础设施内进行实时处理。

telegram · zaihuapd · Jul 14, 09:44

**背景**: Cloudflare 的 Turnstile 是一项广泛使用的服务，它在特定节点（如登录或结账时）弹出挑战（例如交互式谜题）来验证用户是否为真人。用于机器人检测的行为生物识别是一个成熟的研究领域，它分析独特的人类交互模式，如鼠标动力学和击键节奏，这些模式是自动化脚本难以令人信服地复制的。Precursor 在此基础上更进一步，将监控应用于整个用户会话，而不仅仅是单个时间点。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.cloudflare.com/introducing-precursor/">Introducing Precursor: detecting agentic behavior with ...</a></li>
<li><a href="https://www.sciencedirect.com/science/article/pii/S0031320322001248">BeCAPTCHA-Mouse: Synthetic mouse trajectories and improved ...</a></li>
<li><a href="https://cloudnews.tech/cloudflare-launches-precursor-to-detect-bots-throughout-the-entire-session/">Cloudflare Launches Precursor to Detect Bots Throughout the ...</a></li>

</ul>
</details>

**标签**: `#Cloudflare`, `#Bot Detection`, `#Web Security`, `#User Behavior Analytics`, `#AI Security`

---

<a id="item-4"></a>
## [DeepSeek 完成超 500 亿元首轮融资，采用特殊架构维持创始人控制权。](https://t.me/zaihuapd/42557) ⭐️ 8.0/10

中国 AI 初创公司 DeepSeek 完成了首轮融资，筹集资金超过 500 亿元人民币（约合 74 亿美元），估值超过 500 亿美元。此次融资采用了一种非常规架构：投资者需将资金注入由 CEO 梁文锋管理的有限合伙企业，而非直接投资于 DeepSeek 公司本身，并且需要接受五年锁定期且不享有表决权。 这笔巨额融资是私人 AI 公司中规模最大的之一，表明投资者对中国 AI 能力抱有强烈信心，可能加速全球 AI 竞赛。这种巩固创始人控制权的独特治理架构，挑战了传统的风险投资规范，并可能为其他寻求融资但不愿放弃决策权、由创始人主导的科技公司开创先例。 创始人梁文锋在本轮融资中个人投资了 200 亿元人民币。据报道，腾讯和宁德时代分别考虑投资 1000 亿元和 500 亿元，可能成为本轮最大的外部投资者。在此轮融资完成后约一个月，DeepSeek 据称已开始就新一轮融资与投资者进行初步洽谈，投前估值约为 710 亿美元。

telegram · zaihuapd · Jul 14, 11:06

**背景**: 有限合伙企业是风险投资中常见的基金结构，投资者（有限合伙人）提供资金但不参与日常管理，日常管理由普通合伙人负责。创始人控制机制是指旨在让创始人在筹集大量外部资金后仍能保留决策权（如投票控制权）的法律和财务架构。锁定期是指私人公司投资者在一定强制时间内不能赎回或出售其投资的期限，这为公司长期规划确保了资本稳定性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://carta.com/learn/private-funds/structures/limited-partner/">Limited Partner (LP): Responsibilities & Role in Private Funds</a></li>
<li><a href="https://faisonlawgroup.com/blog/startup-founder-control/">Founder Control During Fundraising | Faison Law Group</a></li>
<li><a href="https://www.investopedia.com/terms/l/lockup-period.asp">Decoding Lock-Up Periods: Key Insights for Investors</a></li>

</ul>
</details>

**标签**: `#AI Funding`, `#Corporate Governance`, `#DeepSeek`, `#Venture Capital`, `#China Tech`

---

<a id="item-5"></a>
## [高德发布世界模型工坊 ABot-WorldStudio，内置'时空任意门'可生成交互式 3D 世界](https://www.ithome.com/0/976/538.htm) ⭐️ 8.0/10

阿里巴巴旗下高德正式发布并开放测试通用世界模型工坊 ABot-WorldStudio，用户输入文字或图片即可生成可实时交互的 AI 世界。其核心特色是内置'时空任意门'，可在不同 3D 场景间无缝跃迁，并且该系统可在单张 RTX 5090 显卡上本地部署，官方实测连续推理超过 1 小时无崩溃和质量衰减。 此次发布意义重大，它将交互式视频生成与高保真 3D 场景创建（通过 3D 高斯泼溅技术）统一到一个可本地部署的产品中，降低了创建沉浸式 3D 内容的门槛。其超长的稳定推理能力以及底层模型的开源，有望加速具身智能仿真、游戏影视创作及文旅教育等领域的发展。 该工具的输出结果可保存为视频与 3DGS 文件，其原生的 3DGS 资产具备真实的几何结构与照片级的视觉保真度。底层的 ABot-World 系列模型已全面开源，应用场景覆盖具身智能仿真训练、游戏影视创作及文旅教育等领域。

telegram · zaihuapd · Jul 14, 12:22

**背景**: 在人工智能领域，'世界模型'是一种构建环境内部表征的系统，用于理解和预测环境动态，这对于机器人技术等领域的规划和仿真至关重要。3D 高斯泼溅（3DGS）是一种新颖的 3D 场景表示与渲染技术，它使用数百万个微小的半透明'泼溅点'从图像创建照片级真实感的场景，是传统多边形网格的替代方案。RTX 5090 是英伟达的高端消费级 GPU，拥有 32GB GDDR7 显存和强大的计算能力，适合高要求的 AI 和图形工作负载。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/World_model_(artificial_intelligence)">World model (artificial intelligence) - Wikipedia</a></li>
<li><a href="https://note.com/izutsuya/n/n45650a5fb0f4?hl=en">3D Gaussian Splatting (3DGS) File Format Complete Guide</a></li>
<li><a href="https://www.runpod.io/articles/guides/nvidia-rtx-5090">RTX 5090 Specs and VRAM: Specifications, AI Benchmarks, and LLM Guide</a></li>

</ul>
</details>

**标签**: `#AI-Generated-Content`, `#3D-Gaussian-Splatting`, `#World-Models`, `#Computer-Vision`, `#Creative-Tools`

---

<a id="item-6"></a>
## [Telegram 短链接域名 t.me 遭注册局以 serverHold 状态冻结。](https://t.me/zaihuapd/42559) ⭐️ 8.0/10

Telegram 的核心短链接域名 t.me 于 2026 年 7 月 13 日被其注册局设置为 'serverHold' 状态，导致域名被暂停使用。WHOIS 记录显示该状态更新，并附加了禁止删除、转移、续费和更新等限制，而其注册商仍为 GoDaddy。 此事影响重大，因为注册局层面的 'serverHold' 状态会将域名从全球 DNS 中移除，导致所有用于邀请、频道预览、机器人链接和共享消息的 t.me 短链接失效。这凸显了关键互联网基础设施在集中控制下的脆弱性，并引发了人们对影响主要平台的外部压力、审查或法律行动的担忧。 'serverHold' 状态由域名注册局（据报道是 .me 顶级域的管理方 Identity Digital）直接施加，而非注册商 GoDaddy，它会直接导致域名无法进行 DNS 解析。尽管域名被冻结，其在 GoDaddy 的注册有效期仍持续至 2035 年，Telegram 核心应用功能可能仍能运行，但所有依赖 t.me 链接的服务均已中断。

telegram · zaihuapd · Jul 14, 12:48

**背景**: Telegram 是一款流行的全球性即时通讯应用，以其对速度和安全的重视而闻名。t.me 域名是其官方的短链接服务，用于为分享公共频道、机器人和消息创建简洁的 URL。'serverHold' 是一种注册局层面的管理状态，它会暂停域名，将其从 DNS 中移除，导致域名在互联网上无法访问，这通常是由于法律纠纷、不合规或安全问题引起的。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://domainnamewire.com/2026/07/13/telegrams-t-me-domain-suspended-leading-to-outages/">Telegram's t.me domain suspended, leading to outages [updated] - Domain Name Wire | Domain Name News</a></li>
<li><a href="https://sidebysidedomains.com/blog/serverhold-domain-status.html">"ServerHold" Domain Status Explained: Causes & Solutions ...</a></li>
<li><a href="https://netcrook.com/written_article?slug=telegram-tme-registry-hold-domain-risk&lang=en">A Registry Hold Put Telegram’s Short Link Under Pressure</a></li>

</ul>
</details>

**标签**: `#Telegram`, `#DNS`, `#Internet Governance`, `#Infrastructure`, `#Censorship`

---

<a id="item-7"></a>
## [DeepMind CEO 呼吁美国主导成立拥有发布前评估权的全球 AI 监管机构](https://www.theverge.com/tech/965270/google-deepmind-demis-hassabis-global-ai-watchdog) ⭐️ 8.0/10

Google DeepMind 首席执行官 Demis Hassabis 公开呼吁由美国主导成立一个全球 AI 监管机构，力争在今年年底前开始运作。他提议该机构应由独立专家和开源社区代表组成，并拥有在 AI 模型发布前对其进行评估的权限，以及在风险过高时协调全行业暂停部署的权力。 这一提议意义重大，因为它代表了一位主要的行业领袖正在推动为先进 AI 建立具体、集中的全球治理机制，超越了自愿性准则。如果该机构得以成立，它将从根本上重塑前沿 AI 模型的开发和部署方式，实施强制性的安全审查，并创建一个协调暂停的机制，从而在 AI 接近通用人工智能（AGI）时减轻灾难性风险。 据报道，Hassabis 已与特朗普政府、其他 AI 实验室及欧洲官员进行了数月的沟通，并得到了'非常积极'的反馈。该提议的监管机构所拥有的强制发布前评估和协调行业暂停的权力，与 Anthropic 等其他关注安全的实体最近的呼吁相呼应，表明业界对此类措施的必要性正形成日益增长的共识。

telegram · zaihuapd · Jul 14, 14:29

**背景**: AI 治理指的是为确保 AI 系统的开发和使用符合道德、安全及法规而设计的框架与实践，通常强调公平、问责等原则。在模型发布前进行评估，即部署前评估，是识别潜在风险的关键治理实践。协调行业暂停的想法最近获得了关注，例如 Anthropic 等公司也提议在安全风险升级时暂停开发，这凸显了该行业在快速创新与风险缓解之间的内部张力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.ai21.com/knowledge/ai-governance-frameworks/">9 Key AI Governance Frameworks in 2025 | AI21</a></li>
<li><a href="https://openai.com/index/deployment-simulation/">Predicting model behavior before release by simulating deployment | OpenAI</a></li>
<li><a href="https://political.org/2026/06/04/anthropic-calls-for-coordinated-industry-plan-to-pause-ai-development-if-safety-risks-escalate/">Anthropic Calls for Coordinated Industry Plan to Pause AI ...</a></li>

</ul>
</details>

**标签**: `#AI Governance`, `#AI Safety`, `#Policy`, `#DeepMind`

---

<a id="item-8"></a>
## [白宫将召集电力公司与数据中心开发商，推动自愿承诺以应对 AI 用电成本。](https://t.me/zaihuapd/42566) ⭐️ 8.0/10

白宫计划在未来几周召集电力公司和数据中心开发商，推动一项自愿承诺，以确保人工智能带来的电力需求激增不会推高居民和企业电费。此举是在谷歌、Meta、OpenAI 等公司今年早些时候签署类似承诺的基础上，旨在将承诺范围扩大到电力公司、数据中心代建运营商以及相关州的州长。 这项举措至关重要，因为它解决了 AI 规模化发展的一个关键瓶颈——确保可持续且负担得起的能源基础设施，而无需将电网升级和新建发电设施的巨额成本转嫁给现有电力用户。这代表了一项重要的政策努力，旨在协调 AI 的快速增长与经济公平及电网可靠性，将影响整个科技行业和能源领域。 该承诺是自愿性的，建立在 2026 年初主要科技公司签署的'费率支付者保护承诺'基础之上。一个关键的技术挑战是，将新的数据中心接入电网可能需要 4-5 年，而建设新的输电线路可能需要 7-12 年，这远远超过了典型的数据中心建设周期。

telegram · zaihuapd · Jul 14, 16:00

**背景**: 由于密集的 GPU 集群和先进的冷却要求，AI 数据中心的电力和基础设施成本远高于传统设施。这些数据中心的快速扩张正给美国电网带来压力，引发了关于潜在停电和消费者电费上涨的担忧。关于谁应承担必要电网升级的成本——科技公司、电力公司还是电力用户——正在进行立法和监管层面的讨论。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.reuters.com/legal/litigation/white-house-rally-utilities-data-centers-over-ai-power-costs-2026-07-13/">White House to rally utilities, data centers for AI power ...</a></li>
<li><a href="https://verticaldata.io/data-center-grid-upgrade-costs-who-pays-for-power-in-ai-infrastructure/">Data Center Grid Upgrade Costs: Who Pays for Power in AI ...</a></li>
<li><a href="https://www.cnbc.com/2026/06/24/ai-data-centers-tech-companies-congress-energy-costs.html">Tech companies may have to pay AI data center energy costs</a></li>

</ul>
</details>

**标签**: `#AI Policy`, `#Energy Infrastructure`, `#Data Centers`, `#Sustainable AI`

---