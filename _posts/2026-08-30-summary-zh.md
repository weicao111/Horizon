---
layout: default
title: "Horizon Summary: 2026-08-30 (ZH)"
date: 2026-08-30
lang: zh
---

> From 19 items, 4 important content pieces were selected

---

1. [腾讯开源 Hy4 预览版，一个具备自我改进循环的 7700 亿参数大语言模型](#item-1) ⭐️ 8.0/10
2. [德克萨斯州通过 1 美元汽车保险费，资助了 Flock 监控摄像头的广泛部署。](#item-2) ⭐️ 8.0/10
3. [美国国土安全部利用晦涩海关法秘密获取记者与活动人士电话记录。](#item-3) ⭐️ 8.0/10
4. [索尼音乐等出版商起诉 Anthropic，指控其使用盗版歌词训练 Claude AI 模型](#item-4) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [腾讯开源 Hy4 预览版，一个具备自我改进循环的 7700 亿参数大语言模型](https://www.tencent.com/tencent-releases-and-open-sources-tencent-hy4-preview/) ⭐️ 8.0/10

腾讯发布并开源了 Hy4 预览版模型，这是一个拥有 7700 亿参数、上下文窗口超过 100 万 token 的大语言模型。值得注意的是，该模型通过一个自动化优化循环积极参与了自身的开发过程，对其训练方法、数据策略和评估框架提出了改进建议并进行了测试。 此次发布意义重大，因为它展示了一个早期阶段的递归式自我改进循环，这是迈向更自主的 AI 开发的关键一步。该模型在 OpenRouter 等平台上迅速获得高关注度，几天内处理了数万亿 token，表明了强烈的市场兴趣，并可能在定价和性能上给竞争对手带来压力。 该模型采用混合专家架构，总参数量为 7700 亿，其中活跃参数为 490 亿。它在 OpenRouter 上的定价具有竞争力，缓存成本为 5%，低于典型的 10-20% 费率，这可能促成了其快速被采用。开源版本与 Hugging Face 生态系统完全兼容。

hackernews · shenli3514 · Aug 29, 19:33 · [社区讨论](https://news.ycombinator.com/item?id=49492632)

**背景**: 像 GPT-4 这样的大语言模型是在海量文本数据上训练的 AI 系统，用于理解和生成类人文本。腾讯的混元是其大语言模型系列，类似于 OpenAI 或谷歌的模型。OpenRouter 是一个聚合了来自不同提供商的各种 AI 模型访问权限的平台，允许用户通过统一的 API 进行比较和使用。自动化优化循环指的是一个系统，其中 AI 模型可以提出、运行和评估实验，以改进其自身的设计或训练过程。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.tencent.com/tencent-releases-and-open-sources-tencent-hy4-preview/">Tencent Releases and Open - Sources Tencent Hy4 preview - Tencent</a></li>
<li><a href="https://openrouter.ai/models">Compare AI Models : Pricing, Context & Benchmarks | OpenRouter</a></li>
<li><a href="https://huggingface.co/tencent/Hunyuan-A13B-Pretrain">tencent /Hunyuan-A13B-Pretrain · Hugging Face</a></li>

</ul>
</details>

**社区讨论**: 社区讨论强调了该模型在 OpenRouter 上的快速采用，在短时间内处理的 token 数量超过了 GLM 5.3，部分原因在于其较低的 5% 缓存成本。人们对其自我改进能力表现出浓厚兴趣，一位用户将其与递归式自我改进的概念相提并论。另一位用户则提出了一个关于词汇优化权衡的哲学问题，将其比作创造一种限制性的‘新话’语言。

**标签**: `#artificial-intelligence`, `#machine-learning`, `#open-source`, `#large-language-models`, `#tencent`

---

<a id="item-2"></a>
## [德克萨斯州通过 1 美元汽车保险费，资助了 Flock 监控摄像头的广泛部署。](https://www.texastribune.org/2026/08/28/texas-flock-cameras-auto-insurance-fee-mvcpa-grants/) ⭐️ 8.0/10

2023 年，德克萨斯州立法机构一致通过了一项法律，在所有汽车保险单上增加 1 美元的费用，其收入用于资助机动车犯罪预防局（MVCPA）。该机构由一个主要由州长任命的委员会领导，已使用这些资金在全州部署了至少 3200 个 Flock 监控摄像头，名义上是为了打击催化转化器盗窃。 这为大规模监控基础设施的扩张建立了一个具体、广泛且由公共资金支持的机制，引发了关于隐私和政府越权的重大担忧。该计划在减少催化转化器盗窃方面的有效性尚未得到证实，突显了既定目标与实际结果之间可能存在的脱节。 资金由机动车犯罪预防局（MVCPA）管理，其委员会成员主要由州长任命。目前没有公开数据证实摄像头的部署是否真的降低了催化转化器盗窃率，这是社区质疑的一个关键点。

hackernews · DeepLogin · Aug 29, 23:17 · [社区讨论](https://news.ycombinator.com/item?id=49494182)

**背景**: Flock Safety 是一家制造自动车牌识别（ALPR）摄像头的公司，这些摄像头为执法目的捕获和存储车辆移动数据。催化转化器盗窃是一种普遍犯罪，因为这些汽车部件内部含有贵金属，导致车主需要支付昂贵的维修费用。机动车犯罪预防局（MVCPA）是德克萨斯州的一个机构，专注于减少与机动车相关的犯罪。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://trafficvision.live/blog/flock-cameras">Flock Cameras : What They Are & Can You Watch... | TrafficVision.Live</a></li>
<li><a href="https://dontgetflocked.com/">FlockHopper | Flock Camera Avoidance Routing</a></li>

</ul>
</details>

**社区讨论**: 讨论显示出高度的参与度和复杂的情绪，包括对政府越权和隐私侵蚀的强烈批评，有用户将其与历史上“无代表权的征税”相提并论。一个反复出现且被大量反对的问题聚焦于该计划在减少催化转化器盗窃方面未经证实的有效性。另一种观点建议使用有限责任公司（LLC）注册车辆，作为保护个人信息免受 Flock 数据收集的潜在变通方法。

**标签**: `#surveillance`, `#privacy`, `#public-policy`, `#law-enforcement`, `#data-collection`

---

<a id="item-3"></a>
## [美国国土安全部利用晦涩海关法秘密获取记者与活动人士电话记录。](https://www.theguardian.com/us-news/2026/aug/29/trump-dhs-1509-summons-records-journalists-nonprofits) ⭐️ 8.0/10

美国国土安全部一直在利用《美国法典》第 19 编第 1509 条规定的法律传唤权——一项原本用于海关检查的法律——秘密从电信公司获取记者、非营利组织和工会数月之久的电话记录。在至少一个案例中，国土安全部在未通知目标人物的情况下，获取了其六个月的电话记录，涵盖超过一万条通话和短信，直到记录在法庭上被出示时，当事人才知晓。 这种做法意味着监控权力的显著扩张，已超出其原本用途，引发了关于政府越权、滥用法律权力以及对新闻自由和公民自由产生寒蝉效应的严重担忧。它使得政府能够绕过搜查令或事先通知等标准法律保护程序，直接影响从事受宪法保护活动的个人隐私。 一个关键细节是，遵守第 1509 条传票并非强制性的；如果受到质疑，国土安全部必须诉诸法庭才能强制执行，这使得选择不加抵抗就配合的公司负有责任。此外，据报道，当在法庭上受到质疑时，国土安全部会撤回传票，这一策略被视为试图避免法院对此类做法的合法性做出裁决。

hackernews · firefax · Aug 29, 18:44 · [社区讨论](https://news.ycombinator.com/item?id=49492219)

**背景**: 《美国法典》第 19 编第 1509 条是一项美国法律，主要授予美国海关和边境保护局（CBP，国土安全部下辖机构）在与海关和税收执法相关的事务中检查记录和传唤证人的权力。一份 2017 年的国土安全部监察长报告发现，CBP 当时正在利用这些传票获取与海关或移民法无关的案件记录，这违反了其自身政策。在调查中获取电话记录的标准法律程序通常涉及传票或搜查令，与此行政传唤权相比，它们提供了不同程度的司法监督和提出异议的机会。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.oig.dhs.gov/sites/default/files/assets/Mga/2017/oig-18-18-nov17.pdf">Management Alert - CBP's Use of Examination and Summons Authority Under</a></li>
<li><a href="https://www.law.cornell.edu/uscode/text/19/1509">19 U.S. Code § 1509 - Examination of books and witnesses | U.S. Code | US Law | LII / Legal Information Institute</a></li>

</ul>
</details>

**社区讨论**: 社区评论强调了一个战略性的法律关切，指出国土安全部撤回传票的模式是为了避免法院对其合法性做出明确裁决。评论批评了像 T-Mobile 这样配合请求的公司，并与据报道进行了抵抗的谷歌形成对比。一些评论为记者提出了避免依赖中心化系统的技术解决方案，而另一些则认为针对国内威胁的监控可能是合理的，但这属于少数观点。

**标签**: `#surveillance`, `#civil-liberties`, `#government`, `#journalism`, `#privacy`

---

<a id="item-4"></a>
## [索尼音乐等出版商起诉 Anthropic，指控其使用盗版歌词训练 Claude AI 模型](https://www.musicbusinessworldwide.com/files/2026/08/COMPLAINT-in-Sony_Music_Publishing_US_LLC_e.pdf) ⭐️ 8.0/10

索尼音乐出版、华纳查佩尔音乐等多家公司已在美国加州联邦法院对 Anthropic 及其创始人提起诉讼，指控该公司为训练其 Claude AI 模型，非法下载了数百万本盗版书籍并抓取了受版权保护的歌词。起诉书特别提到了对 LibGen 和 PiLiMi 等影子图书馆的使用，并寻求每件侵权作品最高 15 万美元的法定赔偿以及永久禁令。 这起诉讼是关于使用受版权保护的材料训练生成式 AI 模型的法律斗争的重大升级，直接针对一家领先的 AI 公司，并可能带来巨额经济处罚。其结果可能为 AI 开发者如何获取训练数据树立重要先例，影响整个行业的实践，并可能导致更严格的许可要求或更高的 AI 开发成本。 诉讼指控 Anthropic 从 LibGen 和 PiLiMi 等知名盗版网站获取了超过 700 万本书籍，并且删除了歌词中的版权管理信息。起诉书提及了先前一起导致 15 亿美元和解的类似案件，这表明 Anthropic 面临的风险极高。

telegram · zaihuapd · Aug 30, 01:00

**背景**: Claude 是由 Anthropic 开发的一系列大型语言模型（LLM），于 2023 年 3 月作为聊天机器人发布。LibGen（Library Genesis）是一个知名的影子图书馆，提供对数百万篇学术文章和书籍的免费、未经授权的访问。PiLiMi（Pirate Library Mirror）是一个类似的盗版数字书籍存储库，已被法院明确认定为侵权，并与搜索引擎 Anna's Archive 有关联。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_(AI)">Claude (AI) - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Library_Genesis">Library Genesis - Wikipedia</a></li>
<li><a href="https://www.6pages.com/glossary/piratelibrarymirror(pilimi)/">Pirate Library Mirror (PiLiMi) | 6Pages</a></li>

</ul>
</details>

**标签**: `#AI Ethics`, `#Copyright Law`, `#Legal`, `#Music Industry`, `#Generative AI`

---