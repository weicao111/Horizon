---
layout: default
title: "Horizon Summary: 2026-06-17 (ZH)"
date: 2026-06-17
lang: zh
---

> From 36 items, 10 important content pieces were selected

---

1. [SpaceX 将以 600 亿美元收购 AI 代码编辑器 Cursor。](#item-1) ⭐️ 9.0/10
2. [Android 17 正式发布：强制要求自适应大屏支持，通过 AppFunctions 集成 AI，并转向 Jetpack Compose](#item-2) ⭐️ 9.0/10
3. [本地运行大语言模型已成为一个实用且具优势的选择。](#item-3) ⭐️ 8.0/10
4. [争议性技术文章反对在浏览器会话中使用 JWT，列举安全与复杂性隐患](#item-4) ⭐️ 8.0/10
5. [交互式文章通过手写代码动画拆解机械手表工作原理](#item-5) ⭐️ 8.0/10
6. [针对 Claude Fable 5 的出口管制被批损害美国网络防御能力](#item-6) ⭐️ 8.0/10
7. [中国交付首台国产 ArF 浸没式光刻机，可支撑 7 纳米芯片制造](#item-7) ⭐️ 8.0/10
8. [智谱 AI 全量开放 GLM-5.2 模型，并宣布将基于 MIT 协议开源。](#item-8) ⭐️ 8.0/10
9. [哪吒监控探针存在高危路径穿越漏洞（CVE-2026-53519，CVSS 9.1）](#item-9) ⭐️ 8.0/10
10. [GitHub Copilot 将于 2026 年 6 月改为按使用量计费，调用 GPT-5.5 的成本乘数高达 57 倍。](#item-10) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [SpaceX 将以 600 亿美元收购 AI 代码编辑器 Cursor。](https://www.reuters.com/legal/transactional/spacex-buy-anysphere-60-billion-2026-06-16/) ⭐️ 9.0/10

SpaceX 宣布已达成协议，将以价值 600 亿美元的股票收购 AI 驱动的代码编辑器公司 Cursor，交易预计在 2026 年第三季度完成。这是一家领先的航空航天公司对软件开发工具的一次巨额收购。 此次收购因其巨大的规模而意义重大，标志着 SpaceX 从航空航天领域向先进软件工具领域的一次重大战略转向。这表明 SpaceX 相信 AI 产品拥有巨大的可寻址市场，并可能从根本上重塑开发者工具和 AI 辅助编程的格局。 这笔交易估值为 600 亿美元，采用股票交易形式。据报道，由 25 岁的 CEO Michael Truell 领导的 Cursor 公司，在约两年内将年经常性收入从 100 万美元增长到 20 亿美元，使其成为增长最快的 SaaS 公司之一。

hackernews · itsmarcelg · Jun 16, 10:44 · [社区讨论](https://news.ycombinator.com/item?id=48553224)

**背景**: Cursor 是一款 AI 驱动的代码编辑器，也被称为 AI 编程助手或 AI IDE。与主要提供编写、测试和调试代码工作环境的传统集成开发环境不同，像 Cursor 这样的 AI 驱动编辑器使用大语言模型，能根据自然语言指令主动协助完成代码生成、补全和理解整个代码库等任务。SpaceX 主要是一家由埃隆·马斯克创立的私营航空航天制造商和太空运输服务公司。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Cursor_(code_editor)">Cursor (code editor)</a></li>
<li><a href="https://fortune.com/article/who-is-michael-truell-cursor-ceo-spacex-acquisition/">Who is Michael Truell? Meet Cursor's 25-year-old CEO who cemented a $60 billion deal with SpaceX | Fortune</a></li>
<li><a href="https://www.wsj.com/business/spacex-agrees-to-buy-ai-coding-agent-cursor-for-60-billion-7a473340">SpaceX's $60 Billion Deal to Buy Cursor Gives It More AI Coding Power - WSJ</a></li>

</ul>
</details>

**社区讨论**: 社区情绪复杂，一些人对交易的逻辑和估值表示怀疑。主要观点包括：质疑一家太空公司为何要对一款软件工具进行如此大规模的投资；将 600 亿美元的估值与《我的世界》等其他收购案进行不利比较；以及分享个人偏好，认为其他 AI 编程工作流优于 Cursor。还有一条评论强调了 SpaceX 据称认为 AI 产品拥有 26 万亿美元可寻址市场的观点。

**标签**: `#acquisitions`, `#spacex`, `#developer-tools`, `#artificial-intelligence`, `#industry-news`

---

<a id="item-2"></a>
## [Android 17 正式发布：强制要求自适应大屏支持，通过 AppFunctions 集成 AI，并转向 Jetpack Compose](https://android-developers.googleblog.com/2026/06/Android-17.html) ⭐️ 9.0/10

Android 17 已正式发布，强制要求应用必须支持自适应大屏布局，移除了开发者锁定设备方向和尺寸的规避选项。该版本通过新的 AppFunctions API 集成了 AI 能力，允许 Google Gemini 等 AI 助手直接调用应用内功能，并正式宣布 Android 开发全面转向 Jetpack Compose，传统 View 组件进入维护模式。 此次发布标志着 Android 生态的一次重大转变，推动开发者为日益增长的折叠屏、平板和大屏设备市场打造无缝适配的应用。通过 AppFunctions 实现的深度 AI 集成为更主动、更具代理能力的应用体验铺平了道路，而向 Jetpack Compose 的全面过渡则标准化并现代化了 UI 开发工具包。 强制性的自适应支持意味着 `resizeableActivity=false` 标志在大屏设备上将不再生效，应用必须原生支持自由窗口。AppFunctions API 充当设备端的 MCP（模型上下文协议）服务器，允许应用向 AI 代理暴露自描述的函数。新的隐私控制包括临时权限和联系人选择器，以限制应用获取完整的通讯录。

telegram · zaihuapd · Jun 17, 01:02

**背景**: Jetpack Compose 是一个现代的、声明式的 Android UI 工具包，旨在比旧的基于 XML 的 View 系统更简化、更快速地开发 UI。自适应布局设计是一套创建能在不同屏幕尺寸和设备形态上良好工作的 UI 的原则，随着折叠屏手机和平板电脑的兴起，这变得至关重要。AppFunctions 是一个平台 API 和 Jetpack 库，它使 Android 应用能够通过将其功能暴露为可被发现和调用的工具，来与 AI 代理集成。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developer.android.com/ai/appfunctions">Overview of AppFunctions | AI | Android Developers</a></li>
<li><a href="https://developer.android.com/codelabs/adaptive-material-guidance">Design an Adaptive Layout with Material Design | Android Developers</a></li>
<li><a href="https://medium.com/@appdevinsights/difference-between-compose-ui-vs-android-view-048460959231">Difference between Compose UI vs Android View? | by App Dev Insights - Medium</a></li>

</ul>
</details>

**标签**: `#Android`, `#Mobile Development`, `#AI Integration`, `#Jetpack Compose`, `#Platform Updates`

---

<a id="item-3"></a>
## [本地运行大语言模型已成为一个实用且具优势的选择。](https://vickiboykis.com/2026/06/15/running-local-models-is-good-now/) ⭐️ 8.0/10

文章指出，在本地运行大语言模型已达到可行的程度，为基于云的服务提供了一个实用的替代方案。这一转变得益于 Ollama、LM Studio 和 LocalAI 等工具，它们简化了模型的部署和管理。 这很重要，因为它赋予用户更强的数据隐私性，降低了长期成本，并减少了对云服务提供商的依赖。这代表了人工智能行业的一个重要拐点，可能压低商业 API 提供商的收费上限，并促进强大 AI 技术的民主化访问。 关键的促成因素包括 GPTQ 和 GGUF 等量化技术以减少模型大小，以及 Qwen、Gemma 等强大开源模型的可用性。然而，也存在权衡，例如需要强大的本地硬件（尤其是内存）、量化可能导致的性能下降，以及在工具调用可靠性方面与最先进的云模型相比仍存在局限性。

hackernews · jfb · Jun 16, 14:36 · [社区讨论](https://news.ycombinator.com/item?id=48555993)

**背景**: 大语言模型是在海量文本上训练、用于生成类人语言的 AI 系统。传统上，访问最强大的 LLM 需要使用 OpenAI 或 Anthropic 等公司提供的基于云的 API。本地运行模型涉及下载模型权重并使用软件框架在个人硬件上执行推理，由于计算和内存需求，这在历史上一直具有挑战性。Ollama、LM Studio 和 LocalAI 等工具已经出现，通过提供用户友好的界面和用于本地部署的 OpenAI 兼容 API 来简化这一过程。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://ollama.com/">Ollama</a></li>
<li><a href="https://lmstudio.ai/">LM Studio - Local AI on your computer</a></li>
<li><a href="https://localai.io/">LocalAI</a></li>

</ul>
</details>

**社区讨论**: 社区情绪复杂但参与度高，突显了本地与云端辩论中的权衡。一些用户对本地模型当前的局限性表示失望，指出了速度、准确性（尤其是对于混合专家模型）以及量化后工具调用可靠性等问题。另一些用户则强烈偏好特定本地模型的体验胜过商业云服务，认为其不必要的观点更少，交互风格更令人舒适。一个关键观点是，本地模型可行性的提高对 Anthropic 等云 API 提供商的定价能力构成了长期的竞争威胁。

**标签**: `#local-ai`, `#llm`, `#open-source`, `#model-deployment`, `#cloud-vs-local`

---

<a id="item-4"></a>
## [争议性技术文章反对在浏览器会话中使用 JWT，列举安全与复杂性隐患](https://gist.github.com/samsch/0d1f3d3b4745d778f78b230cf6061452) ⭐️ 8.0/10

一位开发者发布了一篇名为《Stop Using JWTs》的技术文章，明确指出由于安全风险和实现复杂性，应避免使用 JSON Web Tokens 来管理基于浏览器的用户会话。这篇文章在 Hacker News 上引发了广泛讨论，产生了 175 条包含详细技术反驳的评论。 这场辩论很重要，因为 JWT 在 Web 身份验证中应用广泛，而这一强烈批评挑战了常见实践，迫使开发者重新评估无状态 JWT 与有状态会话 Cookie 之间的权衡。讨论凸显了身份验证机制的选择对安全性、可扩展性和系统复杂性（尤其在基于浏览器的应用中）具有深远影响。 该批评特别针对浏览器会话，同时承认 JWT 在服务间通信中仍有其价值。主要担忧包括无法即时撤销单个令牌，以及被盗令牌在过期前一直有效等风险。不过，反对意见指出，采用短期令牌配合刷新机制和撤销列表可以缓解这些问题。

hackernews · dzonga · Jun 16, 16:49 · [社区讨论](https://news.ycombinator.com/item?id=48558147)

**背景**: JSON Web Tokens (JWT) 是一种紧凑、自包含的标准，用于在双方之间安全地传输信息（如用户身份），通常用于身份验证和授权。它常与传统的基于会话的身份验证进行对比，后者由服务器存储会话状态并向客户端发放会话标识符（通常存储在 Cookie 中）。在无状态的 JWT 和有状态的会话之间进行选择，需要在可扩展性、安全攻击面（例如 CSRF 与令牌盗窃）以及对即时撤销的需求等方面进行权衡。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://medium.com/@VisheshV/jwt-vs-session-cookies-picking-the-right-weapon-for-authentication-c41f2c95e804">JWT vs Session Cookies : Picking the Right Weapon for... | Medium</a></li>
<li><a href="https://bytepane.com/blog/jwt-vs-session-cookies-authentication/">JWT vs Session Cookies in 2026: Security, APIs & SPAs</a></li>
<li><a href="https://www.devx.com/web-development-zone/understanding-jwts-and-when-not-to-use-them/">Understanding JWTs (and When Not to Use Them) - DevX</a></li>

</ul>
</details>

**社区讨论**: 社区讨论显示，对于该文章一概而论的谴责存在显著反对意见，许多人认为其批评过于宽泛。主要观点包括：JWT 对于服务间通信是安全且合适的；采用短期令牌配合刷新令牌可以解决撤销问题；并且这种比较常常忽略了基于会话的系统同样存在扩展和存储开销。一些评论者认为原文混淆了 JWT 的通用用途与在浏览器环境中的特定误用。

**标签**: `#authentication`, `#security`, `#jwt`, `#web-development`, `#api-security`

---

<a id="item-5"></a>
## [交互式文章通过手写代码动画拆解机械手表工作原理](https://ciechanow.ski/mechanical-watch/) ⭐️ 8.0/10

2022 年，Bartosz Ciechanowski 发表了一篇深入的交互式文章，通过逐步动画和清晰的解释，直观地阐述了机械手表的复杂工作原理。整个体验完全使用手写的原生 HTML、CSS 和 JavaScript 构建，确保了广泛的兼容性。 这项工作之所以重要，是因为它为网络交互式技术教育树立了高标准，让复杂的工程学主题变得易于广大受众理解。它展示了基础网络技术的持久生命力，能够在不依赖现代框架的情况下，创建丰富、高性能且普遍可访问的教育内容。 这篇文章的技术实现值得注意，它完全采用手写代码，没有使用外部库，这使得它即使在 iPhone 7 等旧设备上也能完美运行。虽然深入探讨了钟表学这一小众主题，但它已经激发了现实世界的项目，例如一位社区成员构建了一个手表机芯的实体爆炸视图。

hackernews · razin · Jun 16, 11:26 · [社区讨论](https://news.ycombinator.com/item?id=48553550)

**背景**: 钟表学是测量时间和制造计时设备的科学与艺术，专注于手表和时钟等机械仪器。机械手表由主发条提供动力，主发条储存的能量通过一系列齿轮释放。这种能量的受控释放由一个称为擒纵机构的关键部件控制，它为摆轮提供周期性脉冲，从而以恒定速率推进指针。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Horology">Horology</a></li>
<li><a href="https://en.wikipedia.org/wiki/Escapement">Escapement - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Mainspring">Mainspring - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 社区赞扬了这篇文章卓越的教育清晰度以及使用原生手写代码实现广泛兼容性的技术成就。评论指出，解释的简洁性掩盖了这项任务的难度，一位用户受到启发，基于这些概念创建了一个物理模型。社区也对作者谦逊的变现方式表示赞赏。

**标签**: `#mechanical-engineering`, `#interactive-education`, `#web-development`, `#horology`, `#visualization`

---

<a id="item-6"></a>
## [针对 Claude Fable 5 的出口管制被批损害美国网络防御能力](https://simonwillison.net/2026/Jun/16/fable-5-export-controls/#atom-everything) ⭐️ 8.0/10

网络安全专家 Kate Moussouris 证实，导致 Anthropic 的 Claude Fable 5 AI 模型受到出口管制的所谓'越狱'行为，仅仅是向包含漏洞的软件代码发出了'修复此代码'的提示。Simon Willison 引述批评指出，这种基于模型修复安全漏洞能力而采取的监管行动，正在损害防御性网络安全工作。 此事意义重大，因为它代表了一个重大的政策失误：旨在防止 AI 辅助网络攻击的出口管制，反而削弱了一种关键的防御工具。如果能够修复安全漏洞的模型受到限制，就会削弱防御者快速发现和修补漏洞的能力，使美国处于安全劣势。 研究人员使用了带有已知 CVE 的开源代码和植入了漏洞的新代码，先是要求模型'审查代码中的安全问题'（Fable 5 拒绝了此请求），然后要求'修复此代码'。Moussouris 认为，这种'发现、修复和测试'的能力是防御性安全的核心，如果削弱此能力，模型修复漏洞的效用就会大打折扣。

rss · Simon Willison · Jun 16, 05:20

**背景**: Claude Fable 5 是 Anthropic 公司公开可用的'Mythos 级'AI 模型，以 3D 设计等能力闻名。Claude Mythos 是 Anthropic 公司一个更强大、未公开发布的模型级别，以其在网络安全和生物学领域涌现的能力而著称。CVE（通用漏洞披露）是对公众已知安全漏洞的标准标识符。针对 AI 模型的出口管制一直存在争议，焦点在于那些可能自动化网络攻击的模型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/news/claude-fable-5-mythos-5">Claude Fable 5 and Claude Mythos 5 \ Anthropic</a></li>
<li><a href="https://en.wikipedia.org/wiki/Mythos_(model)">Mythos (model)</a></li>
<li><a href="https://en.wikipedia.org/wiki/Common_Vulnerabilities_and_Exposures">Common Vulnerabilities and Exposures - Wikipedia</a></li>

</ul>
</details>

**标签**: `#AI Policy`, `#Cybersecurity`, `#Export Controls`, `#AI Safety`

---

<a id="item-7"></a>
## [中国交付首台国产 ArF 浸没式光刻机，可支撑 7 纳米芯片制造](https://news.tongji.edu.cn/info/1002/94903.htm) ⭐️ 8.0/10

2025 年 5 月，由贺荣明团队自主研发的首台氟化氩（ArF）浸没式光刻机正式交付中芯国际。该设备搭配多重曝光工艺，可稳定支撑 7 纳米及以上芯片制程的生产。 此举打破了国外在高端前道光刻设备领域的长期垄断，这是中国半导体产业的一个关键瓶颈。这标志着中国在先进芯片制造领域迈向更大自主性的重要一步，对国家的技术和经济安全至关重要。 该设备支撑 7 纳米制程的能力依赖于多重曝光工艺，这是一种会增加制造步骤和成本的复杂技术。该研发团队自上世纪 80 年代起扎根上海张江，其研发的先进封装光刻机此前已在国内市场占有率超 80%，全球占比 33%。

telegram · zaihuapd · Jun 16, 16:34

**背景**: ArF 浸没式光刻是制造先进半导体节点的关键技术。它使用 193 纳米波长的氟化氩激光光源，并在镜头和晶圆之间增加一层液体（通常是水）以提高分辨率。对于 7 纳米等节点，仅靠浸没式光刻的分辨率仍不足，需要采用多重曝光技术，即使用不同的掩模版对同一芯片层进行多次曝光以形成更精细的图形。前道光刻设备负责在晶圆上绘制最小的晶体管特征。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Immersion_lithography">Immersion lithography - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Multiple_patterning">Multiple patterning - Wikipedia</a></li>
<li><a href="https://www.ccsinsight.com/blog/chinese-chipmakers-look-inward-for-equipment-suppliers/">Chinese Chipmakers Look Inward for Equipment ... - CCS Insight</a></li>

</ul>
</details>

**标签**: `#semiconductors`, `#lithography`, `#china-tech`, `#manufacturing`, `#innovation`

---

<a id="item-8"></a>
## [智谱 AI 全量开放 GLM-5.2 模型，并宣布将基于 MIT 协议开源。](https://t.me/zaihuapd/41997) ⭐️ 8.0/10

智谱 AI 宣布，其能力最强的开源模型 GLM-5.2 现已面向 GLM Coding Plan 全量用户开放，并计划于下周以 MIT 协议开源。该模型支持 100 万 token 的上下文长度，并被定位为国产最强的编程模型。 在其他前沿模型突然变得不可用的背景下，此次发布提供了一个强大且开源的选择，可能加速全球 AI，特别是编程领域的发展和应用。宽松的 MIT 许可证允许广泛的商业和研究使用，没有互惠性（copyleft）的限制要求。 GLM-5.2 是一个拥有 7440 亿参数的混合专家模型，每 token 激活约 400 亿参数，基于 DeepSeek 稀疏注意力架构实现高效的 100 万 token 上下文。该模型完全在华为昇腾 910B 芯片上使用 MindSpore 框架训练，减少了对 NVIDIA 硬件的依赖。

telegram · zaihuapd · Jun 16, 19:29

**背景**: 像 GLM-5.2 这样的大语言模型是在海量文本上训练的 AI 系统，用于理解和生成人类语言。模型的“上下文窗口”指的是它在处理输入时一次性能考虑的最大 token 数量，这对于需要处理长文档或对话的任务至关重要。MIT 许可证是一种宽松的自由软件许可证，允许几乎无限制的使用、修改和分发，只要求保留原始的版权声明。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.aimadetools.com/blog/glm-5-2-complete-guide">GLM-5.2 Complete Guide — 1M Context, MIT License, Setup (2026)</a></li>
<li><a href="https://awesomeagents.ai/models/glm-5-2/">GLM-5.2 | Awesome Agents</a></li>
<li><a href="https://fossa.com/blog/open-source-licenses-101-mit-license/">Open Source Software Licenses 101: The MIT License | FOSSA Blog</a></li>

</ul>
</details>

**标签**: `#Open-Source AI`, `#Large Language Models`, `#Machine Learning`, `#Programming Assistants`

---

<a id="item-9"></a>
## [哪吒监控探针存在高危路径穿越漏洞（CVE-2026-53519，CVSS 9.1）](https://t.me/zaihuapd/42001) ⭐️ 8.0/10

哪吒监控（Nezha）v2.0.13 以下版本存在一个严重的未授权路径穿越漏洞，编号为 CVE-2026-53519，CVSS 评分为 9.1。攻击者通过构造特定的 GET 请求（例如 /dashboard../data/config.yaml）即可读取配置文件并获取其中的 JWT 密钥。 该漏洞危害性极高，因为它允许未经授权的攻击者访问敏感的服务器配置，可能危及被监控服务器的整个身份验证系统。鉴于哪吒监控在服务器监控领域的广泛使用，这对众多 DevOps 和基础设施环境构成了重大风险，需要立即修补。 该漏洞可通过构造类似 `/dashboard../data/config.yaml` 的 GET 请求路径进行利用。获取的 JWT 密钥可能使攻击者能够伪造身份验证令牌。所有 v2.0.13 以下的版本均受影响，用户必须升级到 v2.0.13 或更高版本来规避风险。

telegram · zaihuapd · Jun 17, 01:25

**背景**: 路径穿越漏洞发生在应用程序未能正确清理用于文件操作的用户输入时，使得攻击者能够访问预期范围之外的文件和目录。通用漏洞评分系统（CVSS）是一个用于评估安全漏洞严重程度的标准化框架，9.1 分属于高危级别。JWT（JSON Web Token）密钥用于对令牌进行加密签名；一旦泄露，攻击者可以冒充合法用户或服务。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Path_traversal_vulnerability">Path traversal vulnerability</a></li>
<li><a href="https://en.wikipedia.org/wiki/Common_Vulnerability_Scoring_System">Common Vulnerability Scoring System - Wikipedia</a></li>
<li><a href="https://jwt.io/introduction">JSON Web Token Introduction - jwt.io</a></li>

</ul>
</details>

**标签**: `#security`, `#vulnerability`, `#devops`, `#monitoring`, `#cve`

---

<a id="item-10"></a>
## [GitHub Copilot 将于 2026 年 6 月改为按使用量计费，调用 GPT-5.5 的成本乘数高达 57 倍。](https://t.me/zaihuapd/42003) ⭐️ 8.0/10

GitHub 宣布，从 2026 年 6 月 1 日起，Copilot 的主要计费方式将从固定费率订阅切换为按用量计费，费用根据 Token 消耗计算，并提供每月 GitHub AI Credits 额度。最新公布的模型乘数表显示，使用 GPT-5.5 模型的单次请求计费乘数设定为 57 倍。 这一变化标志着开发者支付 AI 辅助编程费用的根本性转变，从可预测的订阅费转向可变的使用量计费，这可能显著增加重度用户或使用 GPT-5.5 等高级模型的开发者的成本。这反映了 AI 服务向基于 Token 计费的行业大趋势，迫使开发团队必须监控和优化其 AI 使用以控制成本。 对于仍处于传统年度计划中的老用户，官方允许其继续沿用旧版计费模式直到计划到期。GPT-5.5 模型高达 57 倍的乘数表明，与标准模型相比，使用这种更先进、更高智能的模型需要支付高昂的溢价。

telegram · zaihuapd · Jun 17, 03:16

**背景**: GitHub Copilot 是一款广泛使用的 AI 驱动的代码补全工具，集成在开发环境中。基于 Token 的计费是 AI 服务的常见定价模式，费用根据模型处理的输入和输出 Token（文本的基本单位）数量计算。GitHub AI Credits 是该计费体系下的新消费单位，不同订阅等级每月提供一定额度的积分，这些积分会根据所使用的模型和处理的 Token 数量被消耗。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arstechnica.com/ai/2026/06/ai-costs-how-much-github-copilot-users-react-to-new-usage-based-pricing-system/">AI costs how much? GitHub Copilot users react to new... - Ars Technica</a></li>
<li><a href="https://tech.xebia.ms/ai/videos/github-copilot-token-based-billing">Token - based billing : from premium request units to AI ... - Tech Hub</a></li>
<li><a href="https://openai.com/index/introducing-gpt-5-5/">Introducing GPT - 5 . 5 | OpenAI</a></li>

</ul>
</details>

**标签**: `#GitHub Copilot`, `#AI Pricing`, `#Developer Tools`, `#GPT-5.5`

---