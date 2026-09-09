---
layout: default
title: "Horizon Summary: 2026-09-09 (ZH)"
date: 2026-09-09
lang: zh
---

> From 36 items, 8 important content pieces were selected

---

1. [数学家指控 OpenAI 在其 Navier-Stokes 突破性声明中不当使用其研究成果。](#item-1) ⭐️ 9.0/10
2. [DeepMind 发布 AlphaGenome Atlas，一个预测人类基因组中所有可能单字母 DNA 变化的图谱。](#item-2) ⭐️ 9.0/10
3. [OpenAI 发布 ChatGPT Images 2.0，强化文本渲染、逻辑推理与多图一致性。](#item-3) ⭐️ 9.0/10
4. [陶哲轩警告：AI 正在将开放性数学问题作为不可再生资源进行不可持续的“开采”。](#item-4) ⭐️ 8.0/10
5. [Anthropic 员工因担忧 AI 存在性风险而公开辞职](#item-5) ⭐️ 8.0/10
6. [陶哲轩警告：AI 驱动的研究开采正在耗尽开放问题，威胁开放科学传统。](#item-6) ⭐️ 8.0/10
7. [美国指控六家中国 AI 公司通过模型蒸馏技术大规模窃取知识产权](#item-7) ⭐️ 8.0/10
8. [美英立法者提出法案，旨在禁止超级智能 AI 并监管其前体系统。](#item-8) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [数学家指控 OpenAI 在其 Navier-Stokes 突破性声明中不当使用其研究成果。](https://cims.nyu.edu/~tristanb/statement.pdf) ⭐️ 9.0/10

数学家 Tristan Buckmaster 发布声明，指控 OpenAI 在得知他与 Levent Alpöge 在相关数学问题上取得进展后，迅速利用其 AI 模型宣称在 Navier-Stokes 存在性与光滑性问题上取得突破。Buckmaster 进一步指控 OpenAI 试图胁迫他接受一项有利于该公司的延迟发布计划，并对其职业生涯进行了威胁。 这一事件引发了关于研究伦理、知识产权以及大型 AI 公司与学术研究者之间权力动态的深刻问题。如果指控属实，可能会破坏人们对 AI 驱动科学发现的信任，并为公司侵占学术成果开创危险的先例。 Buckmaster 和 Alpöge 于 8 月 15 日发布的工作，证明了相关流体方程（多孔介质、Boussinesq、3D Euler）的有限时间爆破，但并非针对百万美元千禧年大奖的 Navier-Stokes 问题的证明。OpenAI 于 2026 年 9 月 8 日宣称的证明，据称建立在与数学家工作类似的方法之上，并在 Lean 证明助手中进行了形式化，但尚未得到外部专家的验证。

hackernews · procedurecall · Sep 8, 05:42 · [社区讨论](https://news.ycombinator.com/item?id=49605915)

**背景**: Navier-Stokes 存在性与光滑性问题是数学界七大著名的千禧年大奖难题之一，解决者可获得 100 万美元奖金。这些方程描述了流体运动，证明三维空间中光滑解是否始终存在是数学物理学中一个尚未解决的基本问题。OpenAI 是一家领先的 AI 研究公司，最近已开始应用大语言模型来辅助数学发现。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Navier-Stokes_existence_and_smoothness_problem">Navier-Stokes existence and smoothness problem</a></li>
<li><a href="https://fortune.com/2026/09/08/openai-says-it-cracked-navier-stokes-math-grand-challenge-buckmaster-accusation-cheating-intimidation-tao-lament/">OpenAI says it cracked Navier-Stokes, one of math's grand ...</a></li>
<li><a href="https://www.scientificamerican.com/article/openai-claims-blockbuster-math-breakthrough-amid-swirl-of-controversy/">OpenAI claims blockbuster math breakthrough amid swirl of controversy | Scientific American</a></li>

</ul>
</details>

**社区讨论**: 社区讨论突出了 OpenAI 自身声明中指出的核心模糊性，即其“不能排除”使用了包含研究者交互在内的去标识化用户数据。许多评论对涉嫌窃取研究成果和恐吓手段表示愤怒，将其视为公司权力与学术诚信之间的尖锐冲突。舆论普遍批评 OpenAI 的行为，用户将其与历史上因新技术而加速的科学优先权争议案例相提并论。

**标签**: `#mathematics`, `#ai-ethics`, `#openai`, `#academic-research`, `#navier-stokes`

---

<a id="item-2"></a>
## [DeepMind 发布 AlphaGenome Atlas，一个预测人类基因组中所有可能单字母 DNA 变化的图谱。](https://blog.google/innovation-and-ai/models-and-research/google-deepmind/alphagenome-atlas/) ⭐️ 9.0/10

Google DeepMind 推出了 AlphaGenome Atlas 平台，该平台预先计算并预测了人类基因组中每一个可能的单核苷酸变体（约 90 亿个）的分子影响。 这是计算生物学领域的一项重大进展，提供了一个高分辨率的资源，可以加速理解遗传变异在健康和疾病中的作用，有望推动医学研究和变异解读。 该图谱也能预测非编码 DNA 区域的影响，其模型架构结合了用于识别局部模式的卷积层和用于处理长距离序列上下文的 Transformer。可通过网页界面访问，据报道数据集大小约为 1PB。

hackernews · utiiiD · Sep 8, 14:55 · [社区讨论](https://news.ycombinator.com/item?id=49611251)

**背景**: 人类基因组由四种核苷酸碱基（A、T、C、G）的序列组成。单核苷酸变异（SNV）是指其中一个字母的改变，有时会影响基因功能并导致疾病。预测这些变异的功能影响，尤其是在广阔的非编码区域，是基因组学的一大挑战。像 AlphaGenome 这样的计算模型旨在通过学习生物学数据来预测分子表型，从而解决这一问题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://deepmind.google/blog/alphagenome-atlas-a-predictive-map-of-every-possible-dna-letter-change-in-the-human-genome/">AlphaGenome Atlas: Molecular predictions for 9 Billion human DNA ...</a></li>
<li><a href="https://deepmind.google/blog/alphagenome-ai-for-better-understanding-the-genome/">AlphaGenome: AI for better understanding the genome — Google DeepMind</a></li>

</ul>
</details>

**社区讨论**: 社区评论强调了实际访问细节，指出无需正式机构 affiliation 即可访问该图谱。有评论提出了关于其对启动子序列的适用性，以及其与 23andMe 等消费级基因数据结合用于发现致病性突变的潜力。有人分享了一个对病毒进行突变的相关实验研究链接，提供了一个现实世界的比较点。

**标签**: `#genomics`, `#deep-learning`, `#bioinformatics`, `#ai-research`, `#computational-biology`

---

<a id="item-3"></a>
## [OpenAI 发布 ChatGPT Images 2.0，强化文本渲染、逻辑推理与多图一致性。](https://t.me/zaihuapd/43693) ⭐️ 9.0/10

OpenAI 推出了新一代图像生成模型 ChatGPT Images 2.0，该模型引入了逻辑推理与联网搜索能力，能够根据单一提示词生成多达 8 张保持视觉一致性的连续图像，并解决了长期困扰 AI 绘图的中文、日语等非拉丁语系的文本拼写难题。 此次发布通过将类似大语言模型的逻辑推理能力注入图像生成过程，标志着一个范式转变。它将极大推动漫画、UI 设计和营销素材等复杂、多图内容的创作，使 AI 从生成单张图像迈向连贯的视觉叙事。 该模型最高可生成 2K 分辨率的图像，并能创作漫画、UI 元素等复杂构图。一个关键细节是，它在中文、日语等东亚语言的文本渲染准确性上取得了显著提升，这是以往 AI 图像生成器的长期短板。

telegram · zaihuapd · Sep 8, 18:45

**背景**: AI 图像生成中的文本渲染，指的是模型在图像内生成准确、清晰可读文字的能力，这对于创建海报、标签和营销材料至关重要。之前的模型如 DALL-E 3 等在此方面常常表现不佳，尤其是对于非拉丁语系文字。同时，在由 AI 生成的多张图像序列中保持视觉一致性，对创作者来说也一直是一个重大的技术挑战。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/index/introducing-chatgpt-images-2-0/">Introducing ChatGPT Images 2.0 - OpenAI</a></li>
<li><a href="https://www.imagine.art/blogs/text-rendering-ai">What is Text Rendering in AI Image Generation? - imagine.art</a></li>
<li><a href="https://reelmind.ai/blog/mastering-consistency-multi-image-fusion-for-cohesive-ai-character-sequences">Mastering Consistency: Multi-Image Fusion for Cohesive AI ...</a></li>

</ul>
</details>

**社区讨论**: 社区反馈强调了模型生成速度的显著提升，有用户报告延迟从约 104 秒降至 35-40 秒。其他用户对将其用于书籍场景可视化等创意项目感到兴奋，但也有人指出复杂构图中的微小细节（如精确的手指位置）仍可能不完美。该模型在 LM Arena 排行榜上的高分也被视为其能力的重要指标。

**标签**: `#OpenAI`, `#Image Generation`, `#AI Models`, `#Multimodal AI`, `#GPT`

---

<a id="item-4"></a>
## [陶哲轩警告：AI 正在将开放性数学问题作为不可再生资源进行不可持续的“开采”。](https://mathstodon.xyz/@tao/117237320796901560) ⭐️ 8.0/10

著名数学家陶哲轩在 Mathstodon 上发帖，指出数学界面临一个新挑战：识别有前景的开放性问题已成为一种稀缺资源。他警告称，甚至关于某人正在研究某个特定问题的传言，都可能引发大规模 AI 算力介入并率先“解决”它，这可能耗尽这一资源，却无法产生维持进步所需的人类洞见。 这一点很重要，因为它凸显了数学和科学发现领域一个潜在的生存性风险：AI 的暴力解题可能会耗尽由人类提出的、有限的开放问题库，却无法培养出传统上推动长期进步所需的深刻理解和新技术。这迫使人们重新评估 AI 如何融入研究，将焦点从单纯的解决方案提取转向更具创造性的问题提出任务。 陶哲轩的类比将开放性问题视为一种正在被“露天开采”的“不可再生资源”，通过 AI 解决它们的行为（尤其是不揭示底层推理时）可能会抢占并使传统人类主导的研究工作贬值。这种担忧不仅关乎“抢先”获得奖项，更关乎更广泛的生态系统：没有洞见的解决方案无助于提出下一代问题所需的基础知识。

hackernews · _alternator_ · Sep 8, 21:00 · [社区讨论](https://news.ycombinator.com/item?id=49616968)

**背景**: 在数学和理论科学中，“开放性问题”是指那些定义明确、尚未解决的问题，它们指导着研究并启发新理论和方法的产生。经济学中的“不可再生资源”概念指的是随着使用而耗尽的有限存量，如矿物或化石燃料。AI 的最新进展，特别是大语言模型和神经符号系统，已展现出自主解决运筹学、理论物理学等领域中一些长期存在的开放性问题的能力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://panews.io/articles/01a083c5-6d5a-7384-be70-d9eee539859c">Terence Tao Warns: AI Is Unsustainably 'Mining' Open ...</a></li>
<li><a href="https://www.machucavalley.tech/blog/terence-tao-ai-math-non-renewable-resource/">The Great Math Mine: Is AI Exhausting the World's Open Problems?</a></li>
<li><a href="https://www.cs.cmu.edu/news/2026/ai-solves-open-math-problems">Researchers Channel AI To Solve Open Mathematical Problems</a></li>

</ul>
</details>

**社区讨论**: 社区讨论反映了对陶哲轩核心论点的参与，一些人将其与艾萨克·阿西莫夫关于提出有意义问题之困难的科幻作品相提并论。关键观点包括：争论没有洞见的解决方案是否真的阻碍知识进步；建议 AI 的下一个前沿应该是提出具有挑战性的问题，而不仅仅是解决问题；同时也认识到，识别有前景的问题现在已成为稀缺资源。

**标签**: `#artificial-intelligence`, `#mathematics`, `#philosophy-of-science`, `#research-methodology`, `#machine-learning`

---

<a id="item-5"></a>
## [Anthropic 员工因担忧 AI 存在性风险而公开辞职](https://twitter.com/hilbertspaess/status/2097476196791709843#m) ⭐️ 8.0/10

一位名叫 Jacob 的员工今日公开宣布从 AI 实验室 Anthropic 辞职，其引用的主要原因是出于对 AI 安全性和存在性风险的担忧。这一辞职声明在公开平台发布，引发了社区内的广泛讨论。 这一事件突显了领先 AI 公司内部日益增长的伦理张力，注重安全的员工正在权衡其持续参与和感知到的风险。它将关于 AI 存在性威胁的、通常是理论性的辩论，带入了职业选择和企业责任的实践领域，可能影响人才流动和公众对行业的看法。 辞职员工明确表示，没有其他人类活动能构成与先进 AI 同等级别的危险，并将其定性为前所未有的存在性风险。此次辞职的公开性质，以及分享的详细理由，旨在提高认知并引发行动，而非一次私人的职业变动。

hackernews · yurivish · Sep 9, 00:40 · [社区讨论](https://news.ycombinator.com/item?id=49619227)

**背景**: Anthropic 是一家知名的 AI 研究与安全公司，以开发 Claude AI 助手和强调负责任的 AI 发展而闻名。来自人工通用智能（AGI）的存在性风险，指的是一个超级智能 AI 系统可能导致人类灭绝或不可逆转的全球性灾难的假设性场景。围绕 AI 安全的辩论，将关注灾难性后果的担忧与关注近期可衡量的危害及 AI 潜在益处的论点对立起来。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/company">Company \ Anthropic</a></li>
<li><a href="https://en.wikipedia.org/wiki/Existential_risk_from_artificial_general_intelligence">Existential risk from artificial intelligence - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 社区情绪存在分歧，部分评论者赞扬这一基于原则的立场和行动，认为其可能激发更广泛的运动。另一些人则表现出强烈的怀疑，质疑将 AI 风险与核武器或气候变化等威胁相提并论，并就假设的 AI 末日场景的机制和可能性进行辩论。

**标签**: `#AI Safety`, `#AI Ethics`, `#Career`, `#Existential Risk`, `#Industry News`

---

<a id="item-6"></a>
## [陶哲轩警告：AI 驱动的研究开采正在耗尽开放问题，威胁开放科学传统。](https://simonwillison.net/2026/Sep/9/terence-tao/) ⭐️ 8.0/10

著名数学家陶哲轩指出，数学领域富有成果的开放问题集合正被“以不可再生的方式开采”，并可能变得稀缺。他特别警告，即使是关于某人正在研究某个问题的传言，也可能引发大规模的 AI 驱动努力，在该问题尚未充分发展前就将其“解决”，从而促使研究人员不再分享有前景的研究方向。 这突显了一个关键的新兴结构性风险：AI 工具可能加速学术研究中的“公地悲剧”，耗尽未解决问题这一至关重要的共享资源。如果研究人员感到不得不隐藏想法，可能会逆转数个世纪的开放科学传统，损害数学、理论物理等领域的长期进步与合作。 陶哲轩的担忧集中在 AI 增强研究的速度和规模上，它可能在最初由人类主导、可能更具洞察力的研究项目充分发挥潜力之前，就将问题“解决”。这一警告并非针对 AI 解决问题本身，而是针对其在竞争性、传言驱动的环境中使用，如何改变了科学发现的基本激励和社会动态。

rss · Simon Willison · Sep 9, 00:20

**背景**: 在数学和科学中，“开放问题”是指那些定义明确、尚未解决的、能指导研究的问题，例如“千禧年大奖难题”。“开放科学”的传统涉及分享想法、问题和部分结果以促进合作进步，这一实践可追溯到 17 世纪学术期刊的建立。如今，像 Elicit 这样的 AI 驱动研究工具可以快速分析海量文献并生成见解，可能加速这些开放问题的解决。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Open_problems_in_mathematics">Open problems in mathematics</a></li>
<li><a href="https://en.wikipedia.org/wiki/Open_science">Open science - Wikipedia</a></li>
<li><a href="https://elicit.com/">Elicit: AI for scientific research</a></li>

</ul>
</details>

**标签**: `#ai-ethics`, `#open-science`, `#mathematics`, `#research-culture`, `#ai-impact`

---

<a id="item-7"></a>
## [美国指控六家中国 AI 公司通过模型蒸馏技术大规模窃取知识产权](https://www.reuters.com/technology/us-accuses-chinese-ai-firms-industrial-scale-theft-ai-technology-2026-09-08/) ⭐️ 8.0/10

美国政府于 9 月 8 日正式指控包括深度求索（DeepSeek）、月之暗面（Moonshot AI）和阿里巴巴在内的六家中国 AI 公司大规模窃取知识产权。美方指控称，这些公司通过“蒸馏”技术复制了来自 Anthropic、OpenAI、谷歌和 SpaceX 等美国企业的 AI 模型，并暗示相关行为“很可能在中国政府知情下进行”。 这一指控将 AI 技术提升至中美战略竞争的核心议题，直接影响国家安全、贸易政策和全球 AI 创新格局。指控恰逢高层访问计划及中美 AI 安全对话前夕，可能破坏外交努力，并引发针对中国科技行业更严格的出口管制或制裁。 美方声称，所谓的窃取行为不仅降低了中国企业的研发成本，还增强了中国的军事和网络攻击能力。指控中提及的具体技术是“模型蒸馏”，这是一种将知识从大型“教师”模型转移到更小“学生”模型的合法 AI 训练方法。

telegram · zaihuapd · Sep 9, 01:43

**背景**: 模型蒸馏是一种常见的 AI 技术，用于创建更小、更高效的模型，以模仿更大、更复杂模型的性能。Anthropic 是一家由 OpenAI 前成员创立的知名 AI 安全与研究公司。月之暗面（Moonshot AI）是一家领先的中国 AI 公司，以其庞大的开源权重模型“Kimi”而闻名。“AI Tigers”（AI 独角兽）指的是中国顶级的 AI 初创企业。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://kingy.ai/blog/ai-model-distillation-explained/">AI Model Distillation Explained: Technical Guide | Kingy AI</a></li>
<li><a href="https://en.wikipedia.org/wiki/Anthropic">Anthropic - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Moonshot_AI">Moonshot AI - Wikipedia</a></li>

</ul>
</details>

**标签**: `#AI Ethics`, `#Geopolitics`, `#Intellectual Property`, `#US-China Relations`, `#Industry News`

---

<a id="item-8"></a>
## [美英立法者提出法案，旨在禁止超级智能 AI 并监管其前体系统。](https://time.com/article/2026/09/08/ban-superintelligence-ai-uk-us-lawmakers/) ⭐️ 8.0/10

美国参议员伯尼·桑德斯宣布将提出《禁止人工超级智能法案》，旨在禁止开发比人类更聪明的 AI，并暂停其他先进 AI 研究。与此同时，英国议员安德鲁·索贝尔在下议院提出了据称是 G7 议会中首份相关法案，要求赋予政府监控和限制超级智能'前体'系统的权力。 这标志着针对前沿 AI 存在性风险的立法努力显著升级，从自愿的安全承诺转向了提议的法律禁令。如果这些法案获得通过，可能会从根本上重塑全球 AI 发展格局，并为国际监管树立先例，有可能暂停或改变大型企业和国家的 AI 项目方向。 两份法案都要求各自政府推动关于超级智能 AI 的全球条约，但外界普遍认为它们在近期通过的前景渺茫。这些提案得到了专家警告的支持，例如加州大学伯克利分校的斯图尔特·罗素教授，他将潜在风险比作可能协同破坏金融、通信或电网系统的'切尔诺贝利级灾难'。

telegram · zaihuapd · Sep 9, 03:06

**背景**: 人工超级智能（ASI）指的是一种假想的、在所有领域都超越人类智能的 AI，如果其目标与人类价值观不一致，可能会带来存在性风险。'AI 存在性风险'是一些研究人员和行业领袖的主要关切，他们警告超级智能 AI 可能变得无法控制。为此，要求政府监管的呼声日益高涨，包括 2025 年由数百名专家和前官员签署的一份声明，呼吁禁止超级智能的开发。此处的'前体系统'很可能指的是被视为通往超级智能之路的垫脚石或必要技术基础的先进 AI 模型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/AI_existential_risk">AI existential risk</a></li>
<li><a href="https://en.wikipedia.org/wiki/Existential_risk_from_artificial_intelligence">Existential risk from artificial intelligence - Wikipedia</a></li>

</ul>
</details>

**标签**: `#AI Policy`, `#AI Safety`, `#Regulation`, `#Superintelligence`, `#Existential Risk`

---