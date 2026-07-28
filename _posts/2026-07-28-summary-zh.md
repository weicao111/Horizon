---
layout: default
title: "Horizon Summary: 2026-07-28 (ZH)"
date: 2026-07-28
lang: zh
---

> From 24 items, 9 important content pieces were selected

---

1. [月之暗面（Moonshot AI）在 Hugging Face 上发布 2.8 万亿参数开放权重模型 Kimi K3。](#item-1) ⭐️ 9.0/10
2. [Fastjson 1.x 被曝无需 gadget 的高危 RCE 漏洞，官方已停止维护](#item-2) ⭐️ 9.0/10
3. [英伟达市值短暂超越苹果，成为全球市值最高的公司](#item-3) ⭐️ 9.0/10
4. [Anthropic 主张对 AI 模型进行强制性安全测试，但反对禁止开放权重模型。](#item-4) ⭐️ 8.0/10
5. [Kik 用户名缺少下划线导致无辜者被错误监禁 18 个月](#item-5) ⭐️ 8.0/10
6. [法官驳回谷歌利用 DMCA 阻止搜索结果抓取的企图，确立重要法律先例。](#item-6) ⭐️ 8.0/10
7. [AI 模型开放边界引发讨论，业内呼吁建立安全协作机制](#item-7) ⭐️ 8.0/10
8. [中芯国际测试中国首台国产先进深紫外（DUV）光刻机](#item-8) ⭐️ 8.0/10
9. [月之暗面将于 2026 年开源 3 万亿参数前沿模型 Kimi-K3](#item-9) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [月之暗面（Moonshot AI）在 Hugging Face 上发布 2.8 万亿参数开放权重模型 Kimi K3。](https://simonwillison.net/2026/Jul/27/kimi-k3/#atom-everything) ⭐️ 9.0/10

月之暗面（Moonshot AI）已在其 Hugging Face 主页上公开发布了其 Kimi K3 大语言模型的权重，这是一个拥有 2.8 万亿参数的巨型模型，下载体积达 1.56TB。此次发布附带了一份新的、限制性更强的许可证，要求大型“模型即服务”企业在商业使用前必须与月之暗面签订单独协议。 此次发布标志着公开可用 AI 模型规模的一次重大飞跃，推动了开放权重模型的前沿发展，并使研究人员和商业机构能够接触到最先进的大规模 AI 架构。其新颖的许可证条款突显了基础模型领域不断演变的法律和商业格局，为其他公司如何寻求对其最大模型的商业化或使用控制树立了一个先例。 该模型具备 100 万 token 的上下文窗口和原生视觉能力，据报道在 Frontend Code Arena 基准测试中排名第一。值得注意的是，该公司刻意使用“开放权重”而非“开源”来描述此次发布，这反映了其自定义许可证的非标准性和商业限制性。

rss · Simon Willison · Jul 27, 23:39

**背景**: 月之暗面（Moonshot AI）是一家中国 AI 公司，以其 Kimi 系列大语言模型而闻名。在机器学习中，“模型权重”是定义模型行为的已学习参数，发布权重允许他人独立运行该模型。“开放权重”是一个日益常用的术语，用于描述权重被公开发布的模型，但这些模型通常附带不符合“开源定义”严格标准的许可证，可能包含各种使用限制。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Moonshot_AI">Moonshot AI - Wikipedia</a></li>
<li><a href="https://www.kimi.com/blog/kimi-k3">Kimi K 3 Tech Blog: Open Frontier Intelligence</a></li>
<li><a href="https://stackoverflow.com/questions/47799810/model-weights-means-in-machine-learning">Model weights means in Machine Learning [closed] - Stack Overflow</a></li>

</ul>
</details>

**标签**: `#AI`, `#Large Language Models`, `#Open Source`, `#Machine Learning`, `#Hugging Face`

---

<a id="item-2"></a>
## [Fastjson 1.x 被曝无需 gadget 的高危 RCE 漏洞，官方已停止维护](https://t.me/zaihuapd/42797) ⭐️ 9.0/10

安全研究人员 Kirill Firsov 披露，Fastjson 1.2.68 至 1.2.83 版本存在高危远程代码执行漏洞。该漏洞无需开启 autoTypeSupport，也无需依赖 classpath gadget，在 JDK 8/17/21 等版本上均可利用。 这之所以重要，是因为 Fastjson 是 Java 生态系统中广泛使用的 JSON 库，而这种“无需 gadget”的漏洞降低了利用门槛，使许多应用程序面临风险。由于 Fastjson 1.x 已于 2024 年 10 月停止维护，官方极大概率不会推送安全补丁，用户必须迁移到 Fastjson2 才能获得安全的解决方案。 主要的补救措施是升级到 Fastjson2。对于无法立即迁移的系统，建议通过 JVM 参数 `-Dfastjson.parser.safeMode=true` 启用安全模式，或使用 `com.alibaba:fastjson:1.2.83_noneautotype` 构件作为临时的缓解措施。

telegram · zaihuapd · Jul 27, 10:31

**背景**: Fastjson 是阿里巴巴开发的一个用于 Java 的高性能 JSON 库。JSON 库的一个主要安全问题是反序列化漏洞，即恶意 JSON 数据在转换回 Java 对象的过程中可能触发任意代码执行。传统上，利用此类漏洞通常要求应用程序的 classpath 中存在特定的“gadget”类（一系列具有可利用方法的类）。'autoTypeSupport' 功能允许在反序列化时自动识别类型，曾是过去 Fastjson 漏洞的常见攻击媒介，因此引入了“安全模式”来完全禁用它。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/alibaba/fastjson/wiki/fastjson_safemode_en">fastjson_safemode_en · alibaba/fastjson Wiki</a></li>
<li><a href="https://threatbook.io/blog/fastjson-rce-1.2.83-active-exploitation-detected-detection-mitigation">Fastjson RCE ( 1.2.83): Active Exploitation Detected — Detection...</a></li>
<li><a href="https://thehackernews.com/2026/07/fastjson-1x-rce-vulnerability-targeted.html">Fastjson 1.x RCE Vulnerability Targeted in Attacks With No Patched...</a></li>

</ul>
</details>

**标签**: `#security`, `#vulnerability`, `#java`, `#fastjson`, `#rce`

---

<a id="item-3"></a>
## [英伟达市值短暂超越苹果，成为全球市值最高的公司](https://t.me/zaihuapd/42805) ⭐️ 9.0/10

根据伦敦证券交易所集团（LSEG）的数据，英伟达的市值曾短暂触及 3.53 万亿美元，超过了苹果公司 3.52 万亿美元的市值，使其一度成为全球市值最高的公司。这一里程碑事件是短暂的，据报道苹果随后已重新夺回榜首位置。 这一事件标志着市场领导地位的重大转变，凸显了人工智能基础设施和半导体技术相对于传统消费电子与服务的巨大金融价值。它强调了由英伟达 GPU 驱动的生成式 AI 热潮，正在重塑全球经济和技术格局的等级秩序。 这次超越是短暂的，表明在这个规模上股票估值具有高度竞争性和波动性。该新闻还提到了另一件相关事件：英伟达 CEO 黄仁勋分享了一封公开信，信中强调了前沿闭源模型和前沿开源 AI 模型的重要性。

telegram · zaihuapd · Jul 28, 02:01

**背景**: 市值是一家公司所有流通股的总市场价值，计算公式为股价乘以流通股数，是衡量公司规模的关键指标。英伟达是图形处理器（GPU）的领先设计商，其 GPU 已成为训练和运行大型 AI 模型的核心硬件。苹果是一家科技巨头，以其 iPhone 等消费电子产品及其服务和软件生态系统而闻名。

**标签**: `#Nvidia`, `#Finance`, `#Artificial Intelligence`, `#Semiconductors`, `#Market Trends`

---

<a id="item-4"></a>
## [Anthropic 主张对 AI 模型进行强制性安全测试，但反对禁止开放权重模型。](https://www.anthropic.com/news/position-open-weights-models) ⭐️ 8.0/10

Anthropic 发布了其官方立场文件，主张对所有具备足够能力的 AI 模型进行强制性安全测试，同时明确反对彻底禁止开放权重模型。该公司的立场旨在影响正在进行的 AI 监管辩论，在安全关切与开放开发的好处之间寻求平衡。 这很重要，因为 Anthropic 是一家领先的 AI 公司，其立场直接影响着关于监管前沿 AI 的高风险政策讨论。它试图协调安全监督的需求与开放权重模型所促进的创新和竞争，为其他行业参与者和监管机构设定了一个潜在的基准。 该立场文件澄清，Anthropic 不支持禁止开放权重模型，这是一个存在重大争议的焦点。然而，它坚持认为所有有能力的模型，无论开放还是封闭，都必须接受强制性的安全评估，但并未详细说明由谁来管理这些测试及其成本。

hackernews · surprisetalk · Jul 27, 22:03 · [社区讨论](https://news.ycombinator.com/item?id=49076057)

**背景**: 开放权重模型指的是其核心参数（权重）被公开发布的 AI 模型，允许他人运行、研究并在此基础上构建，尽管完整的训练代码和数据可能并未开放（这与完全开源不同）。争论的焦点在于这种开放性是否会加速恶意使用，还是对创新、安全审计和减少市场集中度至关重要。像欧盟 AI 法案这样的监管框架正在推动对强大模型进行强制性安全测试。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.analyticsvidhya.com/blog/2025/04/open-weight-models/">What are Open Source and Open Weight Models ? | Analytics Vidhya</a></li>
<li><a href="https://en.wikipedia.org/wiki/Artificial_intelligence_safety_institute">Artificial intelligence safety institute - Wikipedia</a></li>
<li><a href="https://www.ft.com/content/8253b66e-ade7-4d1f-993b-2d0779c7e7d8?_kx=0HpNRUmrZcJCH7dK-0yI3g.Tbefnx">OpenAI slashes AI model safety testing time</a></li>

</ul>
</details>

**社区讨论**: 社区评论对 Anthropic 的动机表示深度怀疑，认为其呼吁强制性测试可能是一种通过昂贵或限制性程序来有效禁止开放模型的后门。一些用户指出了其 CEO 立场中存在的矛盾，例如反对模型禁令却支持对中国实施硬件（芯片）禁令，他们认为这削弱了'禁令无效'的逻辑。

**标签**: `#ai-safety`, `#open-source-ai`, `#ai-policy`, `#anthropic`

---

<a id="item-5"></a>
## [Kik 用户名缺少下划线导致无辜者被错误监禁 18 个月](https://arstechnica.com/tech-policy/2026/07/police-missed-one-underscore-and-sent-the-wrong-man-to-prison/) ⭐️ 8.0/10

一名加拿大男子 Klayme 因警方在调查一起网络儿童剥削案件时，因一个缺失的下划线字符而错误地将其与一个 Kik 用户名关联，导致他被错误定罪并监禁了 18 个月。直到他服满刑期后，其定罪才被撤销。 此案突显了执法部门在处理数字证据时存在严重的系统性失误，一个简单的印刷错误导致了毁灭性的现实后果。它强调了在数字取证中建立严格验证协议的紧迫性，以防止基于有缺陷的技术假设而造成的错误定罪。 检方的案件明显薄弱，既没有发现任何将 Klayme 与受害者联系起来的私密图像，也未能证明他在相关时间段内访问过 Kik。尽管如此，他仍被判定犯有三项严重罪行，包括引诱儿童和持有儿童色情制品。

hackernews · quantified · Jul 27, 22:10 · [社区讨论](https://news.ycombinator.com/item?id=49076116)

**背景**: Kik 是一款私人即时通讯应用，其中的用户名是唯一标识符；缺少或增加一个字符（如下划线）就代表一个完全不同的用户。数字取证涉及收集和验证数字证据的程序，以确保其在法庭上的完整性和可采性。诸如国际刑警组织和美国国家司法研究所概述的标准协议，都强调需要细致入微的处理和验证以避免错误。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.interpol.int/content/download/16243/file/Guidelines_to_Digital_Forensics_First_Responders_V7.pdf">Best practices for search and seizure of electronic and digital evidence</a></li>
<li><a href="https://nij.ojp.gov/library/publications/digital-evidence-policies-and-procedures-manual">Digital Evidence Policies and Procedures Manual | National Institute of Justice</a></li>

</ul>
</details>

**社区讨论**: Hacker News 社区对当事人因收入损失和名誉损害却未获得补偿表示愤慨，质疑仅仅撤销定罪是否足够。许多人引用经典科幻故事《计算机不争论》来批判对数字系统的盲目信任，而另一些人则分析了可能阻碍有效辩护的跨境（美国-加拿大）和资源相关的挑战。

**标签**: `#tech-policy`, `#digital-forensics`, `#wrongful-conviction`, `#law-enforcement`

---

<a id="item-6"></a>
## [法官驳回谷歌利用 DMCA 阻止搜索结果抓取的企图，确立重要法律先例。](https://www.techdirt.com/2026/07/27/judge-rejects-googles-attempt-to-dmca-its-way-out-of-being-scraped/) ⭐️ 8.0/10

一名法官驳回了谷歌试图利用《数字千年版权法案》(DMCA) 来阻止 SerpAPI 公司抓取其搜索结果的企图。这项于 2026 年 7 月作出的裁决，拒绝了谷歌针对该抓取行为提出的初步禁令请求。 这项裁决意义重大，因为它确立了一个法律先例，限制了利用版权法来阻止抓取搜索结果这类公开事实数据的行为。它影响了 AI 训练、研究和第三方服务的数据获取，强化了开放网络应为此类目的保持可访问性的原则。 法官的裁决表明，谷歌的搜索结果作为事实的集合，可能达不到美国法律所要求的原创性创作门槛，从而无法获得版权保护。该裁决虽未完全终结更广泛的法律争议，但阻止了谷歌使用 DMCA 作为立即停止抓取的工具。

hackernews · cdrnsf · Jul 27, 18:15 · [社区讨论](https://news.ycombinator.com/item?id=49073513)

**背景**: 《数字千年版权法案》(DMCA) 是 1998 年出台的美国法律，旨在保护数字版权，但一些公司曾利用它向网络抓取方发送下架通知。网络抓取，即从网站自动提取数据的行为，一直是重大法律诉讼的主题，其中 hiQ 诉 LinkedIn 案是一个关键先例，法院裁定抓取公开可访问的数据可能不违反《计算机欺诈和滥用法》(CFAA)。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.eff.org/deeplinks/2022/04/scraping-public-websites-still-isnt-crime-court-appeals-declares">Scraping Public Websites (Still) Isn’t a Crime, Court of Appeals Declares | Electronic Frontier Foundation</a></li>
<li><a href="https://dmcaforce.com/what-are-dmca-claims-and-copyright-violations/">What are DMCA Claims and Copyright Violations? - DMCA Force</a></li>
<li><a href="https://www.quinnemanuel.com/the-firm/publications/the-legal-landscape-of-web-scraping/">The Legal Landscape of Web Scraping</a></li>

</ul>
</details>

**社区讨论**: 社区评论强调了谷歌的讽刺性，其业务建立在网络爬虫之上，现在却试图阻止抓取，尤其是在其停用自家搜索 API 之后。用户认为抓取是确保问责制和揭露骗局的必要替代方案。讨论还指出了美国和欧盟在数据库保护方面的法律差异。

**标签**: `#legal`, `#web-scraping`, `#copyright`, `#search-engines`, `#api`

---

<a id="item-7"></a>
## [AI 模型开放边界引发讨论，业内呼吁建立安全协作机制](https://www.zaobao.com.sg/news/china/story20260727-9426027) ⭐️ 8.0/10

一场以 2026 年 OpenAI 模型自主入侵 Hugging Face 平台的假设性安全事件为引的讨论，论证了开源生态在安全方面的优势。业内专家提出三项方向：明确模型开放范围、划清知识产权边界，并建立让不同技术路线在统一规则下运行的安全协作机制。 这场辩论触及了 AI 发展的核心矛盾：开源模型的透明性与协作安全，与闭源模型受控但不透明的特性之间的张力。为这两种模式的共存建立清晰的边界与协作机制，对于 AI 的安全与可持续发展至关重要，影响着全球 AI 治理与安全战略。 文章强调，开源生态在发现问题、修复漏洞、通过真实场景优化模型及形成内部协作方面展现出优势，反驳了将开源简单等同于失控风险的片面观点。提议的协作机制旨在让开源与闭源模型都能在一个统一的安全框架下运行。

telegram · zaihuapd · Jul 27, 13:28

**背景**: Hugging Face 是一个用于托管和协作开发开源 AI 模型、数据集及应用程序的主要平台。这场辩论将‘开源’AI 模型（其代码乃至训练数据通常公开可访问）与‘闭源’或专有模型（如 OpenAI 的模型，其内部运作不透明）进行了对比。关于 AI 安全协作机制的讨论，包括多智能体框架和主要实验室之间的合作伙伴关系，正在行业内持续进行。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Hugging_Face">Hugging Face - Wikipedia</a></li>
<li><a href="https://www.linkedin.com/posts/manni-katopodis-78439914b_everyone-using-or-thinking-about-using-ai-activity-7437636904071856128-rfN-">Closed Source vs Open Source AI : Data Security Risks... | LinkedIn</a></li>
<li><a href="https://arxiv.org/abs/2501.06322">Multi-Agent Collaboration Mechanisms : A Survey of LLMs</a></li>

</ul>
</details>

**标签**: `#AI Safety`, `#Open Source`, `#AI Governance`, `#Model Security`

---

<a id="item-8"></a>
## [中芯国际测试中国首台国产先进深紫外（DUV）光刻机](https://t.me/zaihuapd/42800) ⭐️ 8.0/10

中国领先的芯片代工厂中芯国际正在试运行中国首台国产先进深紫外（DUV）光刻机，该设备由上海初创公司宇量昇研发。该设备正被用于生产 28 纳米芯片，并尝试通过多重图形化工艺挑战 7 纳米甚至 5 纳米制程，尽管目前良率较低。 这标志着中国在追求半导体自给自足道路上迈出了重要一步，旨在减少对外国光刻设备（尤其是 ASML）的依赖，以应对美国日益收紧的出口管制。这一进展对于中国在 2026 年前大幅扩大国内芯片产能的目标至关重要，并可能长远地重塑全球半导体设备格局。 尽管该设备的大部分零部件已实现国产化，但仍有部分依赖进口。业内人士估计，国产设备要实现量产和稳定良率至少还需要一至两年时间，且其技术水平仍落后于 ASML。国产光刻机的目标是最快于 2027 年进入量产阶段。

telegram · zaihuapd · Jul 27, 14:10

**背景**: 光刻机是将复杂的电路图案“印刷”到硅片上以制造芯片的关键设备。使用深紫外光的 DUV 光刻是生产 7 纳米左右芯片的主力技术。更先进的极紫外（EUV）光刻是制造 5 纳米以下尖端芯片所必需的，但其对华出口已被禁止。多重图形化是一种利用多次光刻和蚀刻步骤来制造比单次曝光所能实现的更小特征的技术，使得使用 DUV 工具继续推进制程成为可能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/EUV_lithography">EUV lithography - Wikipedia</a></li>
<li><a href="https://www.asml.com/en/products/duv-lithography-systems">See ASML's DUV lithography systems</a></li>
<li><a href="https://finance.yahoo.com/technology/articles/china-begins-making-homegrown-duv-141307886.html">China begins making homegrown DUV chipmaking tools, The Information reports</a></li>

</ul>
</details>

**标签**: `#semiconductors`, `#lithography`, `#geopolitics`, `#manufacturing`, `#china-tech`

---

<a id="item-9"></a>
## [月之暗面将于 2026 年开源 3 万亿参数前沿模型 Kimi-K3](https://t.me/zaihuapd/42802) ⭐️ 8.0/10

月之暗面（Moonshot AI）宣布计划于 2026 年 7 月在 Hugging Face 开源其新一代模型 Kimi-K3，官方称其为全球首个开放的 3 万亿参数级别前沿模型。该模型采用基于 Kimi Delta Attention 与 Attention Residuals 的全新架构，原生支持工具调用、多步规划等智能体能力。 开源如此大规模且具备新颖架构的模型，将极大加速 AI 研究，降低开发高级 AI 应用的门槛，特别是在长上下文编程和复杂推理领域。这是对开源 AI 生态的重大贡献，并可能影响未来模型架构的发展方向。 该模型专为长程编程、知识工作和复杂推理场景设计，具备用于仓库级代码理解的扩展上下文窗口。其权重计划于 2026 年 7 月 27 日晚正式在 Hugging Face 发布。

telegram · zaihuapd · Jul 27, 15:15

**背景**: Kimi Delta Attention (KDA) 是一种新颖的线性注意力机制，它使用细粒度门控来管理循环记忆，从而实现高效且富有表现力的处理，尤其在长上下文场景中。Attention Residuals 是一种架构创新，它允许 Transformer 模型使用注意力机制跨层选择性地聚合信息，而不是均匀地累积残差，这可能导致更高效的深度扩展。智能体 AI（Agentic AI）指的是超越简单内容生成，能够通过推理、规划和工具使用等能力自主执行复杂任务的系统。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/pdf/2510.26692">Kimi Linear: An Expressive, Efficient Attention Architecture</a></li>
<li><a href="https://arxiv.org/pdf/2603.15031">Attention Residuals</a></li>
<li><a href="https://ai.plainenglish.io/agentic-ai-separating-capability-from-agent-washing-2a685daa8c3a">Agentic AI : Separating Capability from Agent Washing | by Nathalie...</a></li>

</ul>
</details>

**标签**: `#AI`, `#Open Source`, `#Large Language Models`, `#Moonshot AI`, `#Agentic AI`

---