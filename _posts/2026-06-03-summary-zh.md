---
layout: default
title: "Horizon Summary: 2026-06-03 (ZH)"
date: 2026-06-03
lang: zh
---

> From 33 items, 5 important content pieces were selected

---

1. [VSCode Web 编辑器关键漏洞允许一键窃取 GitHub 令牌](#item-1) ⭐️ 9.0/10
2. [特朗普签署行政命令，建立人工智能模型网络安全自愿审查框架](#item-2) ⭐️ 8.0/10
3. [OpenAI 推出 Sites 功能：Codex 可将想法直接转为交互式网页应用](#item-3) ⭐️ 8.0/10
4. [谷歌出资向 Play Store 开发者购买私有代码以训练其 AI 模型。](#item-4) ⭐️ 8.0/10
5. [微软发布第二代 Majorana 2 量子芯片，将商用量子计算机目标提前至 2029 年。](#item-5) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [VSCode Web 编辑器关键漏洞允许一键窃取 GitHub 令牌](https://blog.ammaraskar.com/github-token-stealing/) ⭐️ 9.0/10

一名研究人员披露了 Visual Studio Code 网页编辑器(vscode.dev)中的一个关键漏洞，攻击者只需诱骗用户点击一个恶意链接，即可窃取其 GitHub OAuth 令牌。该漏洞绕过了跨域保护机制，已向微软报告并得到修复。 该漏洞后果严重，因为被窃取的 GitHub 令牌可能让攻击者访问私有代码库和敏感代码，甚至可能通过其他 Webview 漏洞导致供应链攻击或完全远程代码执行(RCE)。它突显了将功能强大且经过身份验证的开发工具直接嵌入浏览器所带来的重大安全风险。 该漏洞之所以能成功利用，是因为 VSCode 网页编辑器的身份验证状态可以从嵌入的 iframe 中访问，这违反了跨域隔离原则。虽然具体漏洞已修复，但网页环境中编辑器登录高权限账户这一根本性的架构风险，仍然是安全研究人员关注的问题。

hackernews · ammar2 · Jun 2, 15:29 · [社区讨论](https://news.ycombinator.com/item?id=48371562)

**背景**: Visual Studio Code 的网页编辑器(vscode.dev)是这款流行 IDE 的浏览器版本。它使用 Webview（本质上是隔离的 iframe）来渲染自定义界面。GitHub OAuth 令牌用于验证用户身份，并授予应用程序访问 GitHub 资源（如代码库）的权限。跨域隔离是一项关键的 Web 安全机制，用于防止网站之间相互干扰；一旦被破坏，就可能导致数据窃取。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://deepwiki.com/microsoft/vscode/5.4-webview-and-custom-editors">Webview and Custom Editors | microsoft/vscode | DeepWiki</a></li>
<li><a href="https://docs.github.com/en/apps/oauth-apps/building-oauth-apps/scopes-for-oauth-apps">Scopes for OAuth apps - GitHub Docs</a></li>
<li><a href="https://aszx87410.github.io/beyond-xss/en/ch4/cors-attack/">Cross - Origin Security Issues | Beyond XSS</a></li>

</ul>
</details>

**社区讨论**: 社区情绪证实了该问题的严重性，用户分享了令牌被盗的个人经历，并批评微软的安全响应流程缓慢且不透明。一个关键的讨论点是基于网页的编辑器登录高权限账户的根本性风险，有人将其比作将高权限令牌以明文形式存储。尽管与厂商沟通体验不佳，仍有用户感谢研究人员进行了负责任的披露。

**标签**: `#security`, `#vscode`, `#github`, `#vulnerability`, `#web-security`

---

<a id="item-2"></a>
## [特朗普签署行政命令，建立人工智能模型网络安全自愿审查框架](https://www.whitehouse.gov/presidential-actions/2026/06/promoting-advanced-artificial-intelligence-innovation-and-security/) ⭐️ 8.0/10

美国总统特朗普于 6 月 2 日签署了一项行政命令，建立了一个自愿性框架，邀请 AI 开发商在发布“受保护的尖端模型”前 30 天，将其提交政府进行网络安全审查。该命令还要求组建一个跨机构的 AI 网络安全清算所，以协调软件漏洞的扫描与修复。 这项行政命令标志着美国在人工智能治理上的一个重要转变，旨在平衡国家安全需求与轻监管承诺，以维持其创新领导地位。它可能为政府如何与私营部门在 AI 安全，尤其是关键基础设施所用模型的安全上进行合作，树立一个先例。 最终确定的 30 天审查期是从最初提议的 90 天缩短而来的，这反映了行业压力和白宫内部的分歧。该命令明确禁止建立强制性的政府许可或预审机制，强调通过公私合作来解决问题。

telegram · zaihuapd · Jun 2, 16:44

**背景**: AI 安全涉及保护人工智能系统免受损害其完整性和可靠性的威胁。在此命令发布前，针对 AI 模型的联邦自愿测试机制已经存在，OpenAI 等公司曾提交模型接受审查。跨机构清算所是一个协调机构，旨在在不同政府部门间共享信息，例如安全漏洞信息。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://tradersunion.com/news/financial-news/show/2211532-trump-ai-model-cybersecurity-tests/">Trump administration seeks voluntary AI model cybersecurity tests in the U.S.</a></li>
<li><a href="https://govciomedia.com/white-house-order-creates-voluntary-ai-framework-for-developers/">White House Order Creates Voluntary AI Framework for Developers | GovCIO Media & Research</a></li>
<li><a href="https://www.axios.com/2026/05/26/cisa-white-house-cybersecurity-ai">Trump hobbled top cyber agency just as AI learned to hack</a></li>

</ul>
</details>

**标签**: `#AI Policy`, `#Cybersecurity`, `#Government Regulation`, `#Artificial Intelligence`

---

<a id="item-3"></a>
## [OpenAI 推出 Sites 功能：Codex 可将想法直接转为交互式网页应用](https://x.com/OpenAI/status/2061845949170045346) ⭐️ 8.0/10

OpenAI 宣布推出名为 Sites 的新功能，该功能允许其 Codex AI 智能体将工作内容、想法和计划直接转换为可通过 URL 访问、使用和分享的交互式网页应用。该功能目前率先向 Business 和 Enterprise 层级用户开放，后续将扩大覆盖范围。 这标志着 AI 辅助开发迈出了重要一步，它使得无需传统编码即可快速创建原型和应用成为可能，有望加速企业内部工具的开发，并在组织内部实现软件开发的民主化。此举将 OpenAI 的 Codex 定位为不断增长的 AI 增强型低代码/无代码平台市场的直接竞争者。 生成的应用是交互式的，可通过简单的 URL 分享，强调了协作的便捷性。一个关键的限制是，目前该功能仅面向 OpenAI 的高阶 Business 和 Enterprise 客户开放，普通公众或个人订阅者尚无法使用。

telegram · zaihuapd · Jun 2, 17:29

**背景**: OpenAI Codex 是一套旨在自动化软件工程任务的 AI 驱动型编程智能体。低代码开发平台（LCDP）通常提供图形化界面环境，使得只需编写极少量的代码即可进行应用开发，从而加速交付并允许非开发人员参与。Sites 的发布将 Codex 的 AI 能力整合到了这种低代码范式之中。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://grokipedia.com/page/OpenAI_Codex">OpenAI Codex</a></li>
<li><a href="https://en.wikipedia.org/wiki/Low-code_development_platform">Low-code development platform</a></li>

</ul>
</details>

**标签**: `#OpenAI`, `#Codex`, `#Low-Code Development`, `#AI Applications`, `#Productivity Tools`

---

<a id="item-4"></a>
## [谷歌出资向 Play Store 开发者购买私有代码以训练其 AI 模型。](https://www.neowin.net/reports/google-wants-to-pay-play-store-developers-for-code-to-train-its-ai/) ⭐️ 8.0/10

谷歌正私下联系 Android 应用开发者，提议付费获取其私有代码库的非独家使用权，用于训练 AI 和改进开发工具。开发者保留 100% 的知识产权，并可通过此授权获得额外收入。 此举是谷歌为获取高质量、现实世界训练数据以缩小其 Gemini AI 与 GitHub Copilot、Claude Code 等竞品在代码生成能力上差距的战略举措。它标志着大型科技公司可能以更符合伦理的方式获取专有代码用于 AI 训练，这可能会重塑开发者工具生态系统和 AI 辅助编程领域的竞争格局。 这一举措是谷歌更广泛推动计划的一部分，近期发布的 Gemini 3.5 Flash 模型和 Antigravity 2.0 智能体优先开发平台即是明证，旨在增强其 AI 驱动的开发者产品。授权模式是非独家的，这意味着开发者可以将同一代码授权给其他方，而谷歌的访问权专门用于训练其 AI 模型。

telegram · zaihuapd · Jun 3, 02:47

**背景**: 谷歌的 Gemini 是一个大型语言模型（LLM）家族，在 AI 编程助手领域参与竞争，而 GitHub Copilot（由 OpenAI 模型驱动）等工具是当前的领先者。有效训练这些模型需要大量高质量、多样化的代码，这些代码通常是专有的，并不像 GitHub 上的仓库那样公开可用。非独家授权允许版权所有者（开发者）授予被许可方（谷歌）使用权，同时保留将相同权利授予其他方的能力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://deepmind.google/models/gemini/flash/">Gemini 3 . 5 Flash — Google DeepMind</a></li>
<li><a href="https://antigravity.google/">Google Antigravity - Build the new way</a></li>
<li><a href="https://copyrightalliance.org/faqs/exclusive-vs-nonexclusive-licenses/">Exclusive vs Non-Exclusive Licenses | Copyright Alliance</a></li>

</ul>
</details>

**标签**: `#AI Training Data`, `#Google`, `#Android Development`, `#Code Generation`, `#Industry Strategy`

---

<a id="item-5"></a>
## [微软发布第二代 Majorana 2 量子芯片，将商用量子计算机目标提前至 2029 年。](https://news.microsoft.com/source/features/innovation/majorana-2-microsoft-discovery-agentic-ai/) ⭐️ 8.0/10

微软正式发布了第二代拓扑量子芯片 Majorana 2，通过采用铅超导体材料，声称将量子比特的可靠性提升了 1000 倍，使其平均寿命从毫秒级大幅延长至 20 秒，部分实例最高可达一分钟。同时，该公司将其构建商用量子计算机的目标时间提前了一半，定为 2029 年。 这一进展标志着在创造具有内在稳定性、容错的量子比特方面可能取得突破，而这是实现实用量子计算的主要障碍。如果成功，微软加速的时间线可能会重塑量子计算行业的竞争格局，挑战目前依赖更成熟但易出错超导量子比特架构的领先者。 此次研发得到了微软 AI 平台 Microsoft Discovery 的协助，该平台目前已正式对外开放。尽管微软声称取得了进展，但其拓扑量子计算路线的底层物理学原理在科学界仍存在争议，不过微软表示其研发过程正接受美国国防高级研究计划局（DARPA）的持续审计以确保可靠性。

telegram · zaihuapd · Jun 3, 04:17

**背景**: 拓扑量子计算是一种利用称为马约拉纳费米子的准粒子来创建“拓扑量子比特”的方法。与传统的超导量子比特不同，拓扑量子比特非局域地存储信息，理论上使其更能抵抗局部干扰和错误，这对于构建可扩展、容错的量子计算机至关重要。微软在这一具有长期高潜力的路线上押下重注，而 IBM 和谷歌等公司则致力于利用超导量子比特取得更近期的进展。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Majorana_fermion">Majorana fermion - Wikipedia</a></li>
<li><a href="https://blog.bervice.com/superconducting-vs-topological-quantum-computers/">Superconducting vs Topological Quantum Computers - blog | bervice</a></li>
<li><a href="https://anes-rezig.github.io/Majorana1/">Majorana : Microsoft’s Quantum Leap</a></li>

</ul>
</details>

**标签**: `#quantum-computing`, `#microsoft`, `#hardware`, `#artificial-intelligence`, `#research`

---