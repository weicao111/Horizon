---
layout: default
title: "Horizon Summary: 2026-06-18 (ZH)"
date: 2026-06-18
lang: zh
---

> From 34 items, 6 important content pieces were selected

---

1. [Midjourney 宣布一项新的医学成像计划，旨在利用 AI 实现低辐射、高分辨率断层扫描。](#item-1) ⭐️ 8.0/10
2. [RFC 10008 引入 QUERY，一种用于携带请求体的新型幂等 HTTP 方法](#item-2) ⭐️ 8.0/10
3. [GLM-5.2 成为 Artificial Analysis 基准测试中排名第一的开源权重 AI 模型。](#item-3) ⭐️ 8.0/10
4. [美国科学研究因政治契约破裂、资金削减和人才外流而陷入危机](#item-4) ⭐️ 8.0/10
5. [微软通过 Azure 销售 OpenAI 模型，在华 AI 业务快速扩张](#item-5) ⭐️ 8.0/10
6. [DeepSeek 开始试推送其图像识别功能](#item-6) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Midjourney 宣布一项新的医学成像计划，旨在利用 AI 实现低辐射、高分辨率断层扫描。](https://www.midjourney.com/medical/blogpost) ⭐️ 8.0/10

Midjourney 宣布了一项名为“Midjourney Medical”的新计划，旨在应用 AI 开发用于低辐射、高分辨率断层扫描的医学成像技术。该公告附带了一个展示假设设备概念的视频渲染。 该计划可能通过减少辐射暴露使诊断成像更安全，并通过降低成本使其更易获得，从而对医疗保健产生重大影响。如果成功，它可能实现对癌症、动脉瘤和纤维化等疾病的更早、更频繁的检测。 目前该公告仍处于概念阶段，主要依靠视频渲染来展示，尚未发布任何证据或临床数据来验证该技术的可行性或性能。社区中的一些技术讨论指出，其强调的纳米级偏转灵敏度与信号放大有关，并不直接等同于最终的图像分辨率。

hackernews · ricochet11 · Jun 18, 01:59 · [社区讨论](https://news.ycombinator.com/item?id=48579650)

**背景**: Midjourney 主要以其开发用于图像和视频生成的高级 AI 模型而闻名。在医学成像领域，计算机断层扫描（CT）是一种常见的诊断工具，它使用 X 射线生成横截面图像，但涉及具有致癌风险的离子辐射。低剂量 CT（LDCT）是一种现有技术，可减少辐射暴露，但往往以牺牲图像质量为潜在代价，AI 增强方法的目标正是改善这种权衡。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.ebme.co.uk/articles/clinical-engineering/low-radiation-dose-computed-tomography-ldct-screening-mobiles">Low radiation dose computed tomography (LDCT) screening mobiles</a></li>
<li><a href="https://pmc.ncbi.nlm.nih.gov/articles/PMC9334854/">Understanding the harm of low -dose computed tomography radiation ...</a></li>
<li><a href="https://www.midjourney.com/">Midjourney</a></li>

</ul>
</details>

**社区讨论**: 社区情绪复杂，一方面对更安全、更便宜的扫描的潜在益处持谨慎乐观态度，另一方面又因缺乏实质性证据而抱有强烈的怀疑。关键观点包括对该技术概念的兴趣、批评宣传视频不足以作为证据，以及要求提供基于证据且经过临床验证的结果才认为其有用。

**标签**: `#AI`, `#Medical Imaging`, `#Healthcare Technology`, `#Computer Vision`, `#Startups`

---

<a id="item-2"></a>
## [RFC 10008 引入 QUERY，一种用于携带请求体的新型幂等 HTTP 方法](https://www.rfc-editor.org/info/rfc10008/) ⭐️ 8.0/10

IETF 已发布 RFC 10008，正式将 QUERY 定义为一个新的 HTTP 方法。QUERY 被设计为一种安全且幂等的方法，允许携带请求体，旨在解决长期以来使用 GET 请求发送负载的问题。 这是 HTTP 协议的一次重要演进，它提供了一种标准化的、幂等的方式来发送带有请求体的复杂查询，这对于需要高级过滤、搜索或无副作用数据检索的 API 至关重要。它解决了历史上与使用 GET 携带负载相关的互操作性和缓存问题。 QUERY 与 POST 类似，但必须是幂等的，这意味着相同的请求可以安全地重复执行。一个值得注意的设计选择是请求体被包含在缓存键中，这引发了关于如何处理大型或用户控制负载的缓存键大小和管理的讨论。

hackernews · schappim · Jun 17, 10:51 · [社区讨论](https://news.ycombinator.com/item?id=48568502)

**背景**: HTTP 方法如 GET、POST、PUT 和 DELETE 定义了请求的操作。GET 被定义为幂等且安全的，但历史上不应包含请求体，这导致了使用长查询字符串等变通方案。POST 可以包含请求体，但不是幂等的，这会导致诸如浏览器重新提交警告等问题。幂等性意味着多次发出相同的请求与发出一次具有相同的效果。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.rfc-editor.org/info/rfc10008/">RFC 10008: The HTTP QUERY Method | RFC Editor</a></li>
<li><a href="https://developer.mozilla.org/en-US/docs/Glossary/Idempotent">Idempotent - Glossary | MDN</a></li>
<li><a href="https://gautamkalla.medium.com/can-we-send-payload-in-http-get-request-e9136eb9c156">Can we send payload in HTTP GET request ? | by GautamKalla | Medium</a></li>

</ul>
</details>

**社区讨论**: 社区讨论既体现了实用兴趣，也包含了对设计的批评。一些开发者质疑将请求体包含在缓存键中所带来的缓存影响，并思考 HTML 表单是否将支持此方法。另一些人则提到了历史背景，表示已使用带请求体的 GET 多年，并幽默地注意到 RFC 编号达到五位数的里程碑。

**标签**: `#http`, `#web-standards`, `#rfc`, `#networking`, `#api-design`

---

<a id="item-3"></a>
## [GLM-5.2 成为 Artificial Analysis 基准测试中排名第一的开源权重 AI 模型。](https://artificialanalysis.ai/articles/glm-5-2-is-the-new-leading-open-weights-model-on-the-artificial-analysis-intelligence-index) ⭐️ 8.0/10

由 Z.ai（原智谱 AI）开发的开源权重大语言模型 GLM-5.2 已在 Artificial Analysis Intelligence Index 上排名第一。该模型在性能上可与 Claude Opus 等顶级闭源模型竞争，尤其在长周期编码和科学推理基准测试中表现出色，同时成本显著更低。 这一进展代表了开源 AI 的重大飞跃，以极低的价格提供了接近前沿模型的性能，可能使高性能 AI 的获取更加民主化。它挑战了 Anthropic、OpenAI 和 Google 等公司的闭源模型主导地位，可能重塑 AI API 的竞争格局和定价。 这个拥有 7530 亿参数的模型相比其前身 GLM-5.1 有显著提升，包括在 CritPt 科学推理基准上提高了 16 分，并以 1524 分的成绩在 GDPval-AA v2 评分中领先。然而，一些社区测试表明，尽管其整体基准测试效率很高，但对于某些推理密集型任务，它可能速度较慢且计算成本较高。

hackernews · himata4113 · Jun 17, 09:12 · [社区讨论](https://news.ycombinator.com/item?id=48567759)

**背景**: Artificial Analysis 是一个独立的基准测试平台，用于评估 AI 模型在推理质量、速度和成本等指标上的表现，并编制如 Intelligence Index 等综合评分。'开源权重'模型，如 GLM-5.2，其模型参数是公开可用的，这与 Anthropic 的 Claude Opus 等'专有'或闭源模型不同，后者仅能通过 API 访问。这些模型的性能和成本是开发者和企业选择 AI 解决方案的关键因素。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://artificialanalysis.ai/articles/glm-5-2-is-the-new-leading-open-weights-model-on-the-artificial-analysis-intelligence-index">GLM-5.2 is the new leading open weights model on the Artificial Analysis Intelligence Index</a></li>
<li><a href="https://venturebeat.com/technology/z-ais-open-weights-glm-5-2-beats-gpt-5-5-on-multiple-long-horizon-coding-benchmarks-for-1-6th-the-cost">Z.ai’s open-weights GLM-5.2 beats GPT-5.5 on multiple long-horizon coding benchmarks for 1/6th the cost | VentureBeat</a></li>
<li><a href="https://artificialanalysis.ai/">AI Model & API Providers Analysis | Artificial Analysis</a></li>

</ul>
</details>

**社区讨论**: 社区情绪总体积极，强调了该模型令人印象深刻的性能价格比，一些用户指出第三方提供商以远低于官方 API 的价格提供该模型。然而，批评意见包括对其在实际任务中的推理速度和效率的担忧，例如有用户报告生成一个简单的代码库需要 15 分钟。此外，社区也在讨论其与 GPT-5.5 等模型在不同努力设置下的成本效益对比。

**标签**: `#artificial-intelligence`, `#open-source`, `#large-language-models`, `#machine-learning`, `#ai-apis`

---

<a id="item-4"></a>
## [美国科学研究因政治契约破裂、资金削减和人才外流而陷入危机](https://www.scientificamerican.com/article/americas-compact-between-science-and-politics-is-broken/) ⭐️ 8.0/10

近期的一篇文章和广泛的社区讨论指出，美国科学与政治之间长期存在的契约已经破裂，具体表现为前所未有的随意取消拨款、延迟发放资金以及新的签证限制。这导致了科学人才的大量外流，许多研究人员及其家庭正计划离开美国。 这场系统性危机威胁着美国科学主导地位的基础——稳定的资金和全球人才的获取——可能对创新、经济竞争力和国家安全造成长期损害。正如全球掌握特定仪器技能的研究人员数量极少所表明的，这种专业化知识的流失对国家研究能力造成了不可替代的损失。 这场危机因资金决策的政治化理由而加剧，例如禁止提及多样性、公平和包容（DEI）内容的拨款申请。社区评论揭示，即使是此前受影响较小的领域，现在也正经历严重的紧张局势，资深科学家们正在准备备选方案，有前途的博士生也选择前往其他国家。

hackernews · presspot · Jun 17, 09:54 · [社区讨论](https://news.ycombinator.com/item?id=48568058)

**背景**: 历史上，美国的科学进步依赖于一种默示的“契约”，即公共资金在最小政治干预下支持基础研究，从而培养了全球领导地位。关键机制包括来自美国国家科学基金会（NSF）和美国国立卫生研究院（NIH）等机构的竞争性拨款，以及吸引国际人才的签证项目（如 J-1、H-1B）。“人才外流”指的是一个国家或机构熟练人员和人才的大量流失，目前在美国学术界正因政策和资金压力而出现研究人员离开的现象。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.scientificamerican.com/article/americas-compact-between-science-and-politics-is-broken/">America’s compact between science and politics is broken</a></li>
<li><a href="https://cen.acs.org/policy/us-visa-restriction-stem-research-innovation-patent/104/web/2026/05">As visa rules tighten, impacts to researchers and US science escalate</a></li>
<li><a href="https://theweek.com/education/united-states-trump-higher-education-losing-educators">How US policies are fueling a new academic brain drain | The Week</a></li>

</ul>
</details>

**社区讨论**: 讨论反映出一种绝望和紧迫感，研究人员分享了资金枯竭、计划招聘因签证问题受阻以及个人决定离开美国的第一手经历。普遍情绪表明，大家广泛认同科研环境已变得充满敌意，正迫使早期职业和资深科学家离开学术界或美国，并将基本的科学事实视为党派议题。

**标签**: `#science-policy`, `#research-funding`, `#academia`, `#brain-drain`, `#immigration`

---

<a id="item-5"></a>
## [微软通过 Azure 销售 OpenAI 模型，在华 AI 业务快速扩张](https://www.bloomberg.com/news/articles/2026-06-17/microsoft-s-china-ai-business-grows-on-openai-model-sales) ⭐️ 8.0/10

微软正通过其 Azure 云平台向中国主要科技公司销售 OpenAI 模型，从而快速扩张其在中国的 AI 业务。知情人士称，字节跳动是其最大客户，每年在微软 AI 和云服务上的投入预计超 10 亿美元；蚂蚁集团、美团、腾讯也是重要客户，推动 Azure 在华 AI 收入增速一度成为全球最快。 此次扩张凸显了全球商业与地缘政治的复杂交织，微软在服务庞大市场的同时，也面临着美国对技术转让和国家安全风险的审查。这一重要的收入来源也表明，尽管中国持续努力发展国产替代方案，但其对西方尖端 AI 模型仍存在巨大依赖，这可能影响全球 AI 竞争格局。 微软强调其只向成熟企业而非个人开发者销售模型，且模型托管在境外的数据中心，客户需通过互联网进行访问。OpenAI 曾私下向微软抱怨，称其未充分阻止中国公司通过'蒸馏'技术提取其模型知识，这是一种将大模型知识转移到小模型的技术。

telegram · zaihuapd · Jun 18, 01:06

**背景**: Azure AI Foundry 是微软的一个平台，允许企业通过 API 和 Web 门户发现、部署和管理 AI 模型，包括来自 OpenAI 的模型。模型蒸馏，或称知识蒸馏，是一种机器学习技术，通过训练一个较小的'学生'模型来模仿更大、更复杂的'教师'模型的行为，从而有可能以更少的资源复制核心能力。微软的 Azure 为全球公司提供了访问先进 AI 模型的基础设施和合规框架，同时试图管理数据治理和使用策略。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://learn.microsoft.com/en-us/rest/api/aifoundry/modelinference/">Azure AI Model Inference REST API | Microsoft Learn</a></li>
<li><a href="https://en.wikipedia.org/wiki/Knowledge_distillation">Knowledge distillation - Wikipedia</a></li>
<li><a href="https://learn.microsoft.com/en-us/azure/ai-foundry/openai/use-your-data-quickstart">Use your own data with Azure OpenAI in Azure AI Foundry Models ...</a></li>

</ul>
</details>

**标签**: `#AI Ethics & Policy`, `#Cloud Computing`, `#Geopolitics`, `#Business Strategy`, `#Microsoft`

---

<a id="item-6"></a>
## [DeepSeek 开始试推送其图像识别功能](https://t.me/zaihuapd/42026) ⭐️ 8.0/10

根据 Telegram 频道的公告，DeepSeek 已开始对其图像识别功能进行试推送。这标志着该 AI 模型一项新的多模态能力的初始部署阶段。 此次推送意义重大，因为它将 DeepSeek 从纯文本模型扩展为多模态 AI，增强了其与其他具备视觉能力的大型语言模型的竞争力。这使得 AI 能够理解和分析视觉内容，从而在内容分析、自动化等领域拓宽了模型的实用性。 该功能目前处于试用阶段，表明正在向部分用户进行可控发布，以进行初步测试和收集反馈。相关技术资料显示，DeepSeek 的图像识别采用了结合卷积神经网络（CNN）和视觉变换器（ViT）的深度学习架构。

telegram · zaihuapd · Jun 18, 04:50

**背景**: DeepSeek 是一个知名的大型语言模型（LLM），以其在文本任务上的强大性能而著称。图像识别，或称计算机视觉，是 AI 的一个领域，旨在让机器能够解释和理解来自世界的视觉信息。为 LLM 添加视觉能力可创建一个多模态模型，使其能够跨文本和图像进行处理和推理，这是推动 AI 向更通用智能发展的关键趋势。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://deepseekimage.org/features/image-recognition">DeepSeek Image Recognition | DeepSeek Image</a></li>
<li><a href="https://edrawmind.wondershare.com/ai-features/deepseek-for-image-analysis.html">Quick Tutorial for DeepSeek Image Analysis</a></li>
<li><a href="https://launchdarkly.com/blog/ai-model-deployment/">AI model deployment: Best practices for production environments | LaunchDarkly</a></li>

</ul>
</details>

**标签**: `#DeepSeek`, `#Computer Vision`, `#AI Features`, `#Model Updates`

---