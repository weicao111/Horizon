---
layout: default
title: "Horizon Summary: 2026-07-19 (ZH)"
date: 2026-07-19
lang: zh
---

> From 27 items, 5 important content pieces were selected

---

1. [据报道，GPT-5.6 被用于填补凸优化复杂性理论中一个长达 30 年的空白。](#item-1) ⭐️ 8.0/10
2. [LG 显示器通过 Windows Update 在未经用户同意的情况下自动安装软件](#item-2) ⭐️ 8.0/10
3. [台积电宣布下一代 A14 制程技术将于 2028 年投产。](#item-3) ⭐️ 8.0/10
4. [旧金山责令苹果和谷歌下架 AI'脱衣'应用。](#item-4) ⭐️ 8.0/10
5. [荣耀发布 Agentic OS 技术框架，旨在将手机操作系统从应用中心转向意图中心](#item-5) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [据报道，GPT-5.6 被用于填补凸优化复杂性理论中一个长达 30 年的空白。](https://old.reddit.com/r/math/comments/1uxj3cy/after_openais_cdc_proof_announcement_gpt56_used_a/) ⭐️ 8.0/10

一名研究人员使用 GPT-5.6（具体是 Sol Pro 版本）证明了一个关于在球面上优化 Lipschitz 凸函数计算复杂性的猜想，该问题已悬而未决约三十年。据称，在与 AI 交互了 148 分钟后得出了解决方案，而此前已用更早的模型尝试了一年。 这展示了先进 AI 作为数学发现协作者的一种新颖且可能具有变革性的应用，特别是在理论计算机科学和优化领域。它表明 AI 可以加速解决长期存在的、小众的理论问题，可能重塑这些领域的研究方式。 这项工作具体针对的是在球域上优化 Lipschitz 凸函数的复杂性，这是优化理论中的一个标准设定。来自社区的批判性背景指出，'148 分钟'的说法是有细微差别的，因为它是在使用 GPT-5.4/5.5 进行了一年的人工引导尝试之后才实现的，并且提供给 Sol Pro 的最终提示可能包含了关键的解决技术。

hackernews · mbustamanter · Jul 18, 13:00 · [社区讨论](https://news.ycombinator.com/item?id=48957779)

**背景**: 凸优化是数学优化的一个子领域，专注于在凸集上最小化凸函数，许多问题都存在高效（多项式时间）算法。复杂性理论中的一个关键问题是，对于具有特定性质（如凸性和 Lipschitz 连续性）的函数，确立其优化所需时间或查询次数的基本下界。所解决的猜想就与在球面等有界域上定义的函数的这些基本极限有关。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Convex_optimization">Convex optimization - Wikipedia</a></li>
<li><a href="https://proceedings.mlr.press/v65/balkanski17a/balkanski17a.pdf">The Sample Complexity of Optimizing a Convex Function</a></li>

</ul>
</details>

**社区讨论**: 讨论中既有认可也有怀疑。评论者虽然承认这是一个真正的贡献，但也批判性地审视了这一说法的表述，指出在 AI 那 148 分钟的会话之前，已有大量的人力前期工作（使用更早的 GPT 版本工作了一年）。此外，还讨论了不同 AI 模型（Sol Pro 与 Ultra）的具体能力，以及对数学研究更广泛的影响，并将其与 AI 处理'低垂果实'的软件开发趋势进行了比较。

**标签**: `#artificial-intelligence`, `#mathematics`, `#optimization`, `#machine-learning`, `#complexity-theory`

---

<a id="item-2"></a>
## [LG 显示器通过 Windows Update 在未经用户同意的情况下自动安装软件](https://videocardz.com/newz/lg-monitors-silently-install-software-through-windows-update-without-user-consent) ⭐️ 8.0/10

LG 显示器被发现一旦通过 HDMI 接口连接，就会触发 Windows Update 机制自动安装 LG 的 OnScreen Control 软件，整个过程无需用户交互或同意。对于已连接的老款 LG 显示器，在 Windows Update 扫描时也会发生同样的情况。 这种做法绕过了标准的安全和隐私预期，使得硬件厂商能够在全球超过十亿台 Windows PC 上静默安装可能不需要的软件，且该软件拥有完整的系统与网络访问权限。这严重削弱了用户控制权，并创造了一个新的攻击途径——任何拥有微软签名驱动的设备都可能被用来部署恶意软件。 被安装的软件是 LG 的 OnScreen Control 应用程序，根据微软规则它被归类为'手动'驱动更新，但却被自动分发。用户可以通过在 Windows 设备安装设置中禁用'自动下载设备制造商提供的应用'来规避此问题。

hackernews · baranul · Jul 18, 10:21 · [社区讨论](https://news.ycombinator.com/item?id=48956688)

**背景**: Windows Update 可以自动分发驱动程序包，以实现硬件的即插即用功能。像 LG 这样的制造商可以向微软提交其驱动程序和相关软件，然后微软通过其受信任的更新渠道进行分发。该系统旨在无需用户提示即可安装'自动'驱动更新以确保硬件兼容性，但供应商可以控制其软件包的分发类型（自动、手动等）。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://learn.microsoft.com/en-us/windows-hardware/drivers/dashboard/understanding-windows-update-automatic-and-optional-rules-for-driver-distribution">Understanding Windows Update rules for driver distribution - Windows drivers | Microsoft Learn</a></li>
<li><a href="https://learn.microsoft.com/en-us/windows-hardware/drivers/develop/distributing-a-driver-package">Distributing a Driver Package - Windows drivers | Microsoft Learn</a></li>
<li><a href="https://www.lg.com/levant_en/support/product-help/CT40011533-20155181426844">Help Library: Help Library: How to download the LG OnScreen ...</a></li>

</ul>
</details>

**社区讨论**: 社区情绪高度批判，认为这种自动安装行为类似'恶意软件'，赋予了不需要的软件完整的系统访问权限。评论者强调，仅插入显示器就触发这种静默的、具备网络访问能力的安装，具有严重的安全隐患。讨论还提供了使用组策略或系统设置的实际解决方法，并辩论了微软在监管供应商通过其更新系统推送软件方面的责任。

**标签**: `#security`, `#privacy`, `#windows`, `#hardware`, `#malware`

---

<a id="item-3"></a>
## [台积电宣布下一代 A14 制程技术将于 2028 年投产。](https://t.me/zaihuapd/42643) ⭐️ 8.0/10

台积电宣布计划在 2028 年开始生产 A14 制程技术，并将其定位为即将量产的 N2 节点的后继者。该公司宣称，与 N2 相比，A14 将在相同功耗下提升高达 15%的性能，或在相同性能下降低达 30%的功耗，同时逻辑密度提高 20%以上。 这一公告意义重大，它勾勒出台积电为保持其在先进半导体制造领域的领先地位而制定的积极路线图，这对于驱动未来的人工智能、高性能计算和消费电子至关重要。A14 预计带来的性能和能效提升，将直接影响苹果、AMD 和英伟达等主要科技公司设计的芯片的性能与能耗。 台积电还计划在 2026 年末推出中间的 A16 制程，这表明其新节点推出的节奏正在加快。A14 节点预计将采用第二代环绕栅极（GAAFET）晶体管架构，通常被称为 1.4 纳米级技术。

telegram · zaihuapd · Jul 18, 05:00

**背景**: 在半导体制造中，“制程节点”（如 N2 或 A14）指的是特定一代的制造技术，纳米数越小通常意味着芯片更先进、密度更高、能效更好。“逻辑密度”衡量的是在给定面积的硅片上能容纳多少晶体管（基本开关单元）；更高的密度允许制造更复杂、更强大的芯片。台积电的 N2 是其即将推出的 2 纳米级节点，而更先进的 A14 节点将接替它，延续行业对摩尔定律的不懈追求。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.tsmc.com/english/dedicatedFoundry/technology/logic/l_A14">A14 Technology - Taiwan Semiconductor Manufacturing Company Limited</a></li>
<li><a href="https://semiwiki.com/wikis/industry-wikis/tsmc-a14-process-technology-wiki/">TSMC A14 Process Technology Wiki - Semiwiki</a></li>
<li><a href="https://anysilicon.com/tsmc-to-break-ground-on-1-4nm-a14-fab-on-november-5/">TSMC to Break Ground on 1.4nm “A14” Fab on November 5 - AnySilicon</a></li>

</ul>
</details>

**标签**: `#semiconductors`, `#tsmc`, `#process-node`, `#roadmap`, `#hardware`

---

<a id="item-4"></a>
## [旧金山责令苹果和谷歌下架 AI'脱衣'应用。](https://techcrunch.com/2026/07/17/apple-and-google-ordered-to-purge-nudify-apps-from-app-stores/) ⭐️ 8.0/10

旧金山市检察长邱信福已责令苹果和谷歌从其应用商店中下架数十款'nudify'应用，这些应用利用 AI 技术通过数字方式移除照片中的衣物，生成非自愿的亲密深度伪造图像。该命令指出，在科技透明项目今年早些时候发出警告后，两家公司可能已从中获利数百万美元却未及时采取行动。 此举标志着在追究主要科技平台托管助长数字性虐待的有害 AI 应用的责任方面，出现了重大升级。它为地方政府执行内容审核设定了一个潜在的法律先例，并可能迫使全球应用商店主动监管 AI 生成的非自愿亲密图像。 苹果公司表示已下架三款应用并终止了相关开发者账户，而谷歌则表示已从 Play 商店暂停了被点名的五款应用。市检察长的信件指控这两家公司因允许这些收费应用运营而可能面临民事处罚，并可能从中获利。

telegram · zaihuapd · Jul 18, 08:45

**背景**: 'Nudify'应用是一种利用生成式 AI 和深度伪造技术，在通常未经本人同意的情况下，创建个人的合成裸体或亲密图像的应用程序。这属于更广泛的非自愿亲密深度伪造范畴，是一种数字性虐待形式，在英国和美国多个州等司法管辖区已被定为刑事犯罪。科技透明项目是一个非营利组织，负责调查和报告主要科技公司的行为。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Nudify_apps">Nudify apps</a></li>
<li><a href="https://airiskaware.com/insights/ai-deepfakes-your-rights">AI Deepfakes and Your Rights: What to Do If Your Image | AIRiskAware</a></li>
<li><a href="https://www.techtransparencyproject.org/">Tech Transparency Project</a></li>

</ul>
</details>

**标签**: `#AI Ethics`, `#Platform Regulation`, `#Deepfakes`, `#Content Moderation`

---

<a id="item-5"></a>
## [荣耀发布 Agentic OS 技术框架，旨在将手机操作系统从应用中心转向意图中心](https://wallstreetcn.com/articles/3777328) ⭐️ 8.0/10

在 2026 世界人工智能大会期间，荣耀发布了其 Agentic OS 技术框架，旨在重构手机操作系统，使其从以应用为中心转向以用户的“意图”和“任务”为中心。荣耀还与阿里巴巴千问合作，开发针对手机场景的终端大模型解决方案，并展示了能够通过自然语言发起并自动执行跨应用任务的“Robot Phone”。 此举标志着移动操作系统架构的一次重大概念性转变，将智能手机定位为基于用户目标主动编排任务的 AI 智能体中枢。如果成功，它可能从根本上改变人机交互模式，超越传统的以应用为中心的模式，并加速全行业向终端侧、意图驱动的 AI 助手发展的趋势。 该框架是由荣耀首席 AI 科学家黄非宣布的一项技术愿景，其实现依赖于与阿里巴巴合作开发一个强大的终端侧大模型。所展示的“Robot Phone”概念表明，自然语言有潜力直接编排跨不同应用的复杂多步骤任务，而无需人工干预。

telegram · zaihuapd · Jul 19, 02:06

**背景**: “智能体操作系统”（Agentic OS）是一个新兴概念，指的是一个使 AI 智能体能够理解目标、规划并执行任务的协调层。它代表了传统操作系统服务之上的一个抽象层，专注于编排 AI 能力。行业正在探索终端侧 AI 智能体，例如谷歌和三星推出的产品，它们从系统菜单处理任务，旨在提供更主动、更私密的辅助。正如一些机器人研究所展示的，使用自然语言指令系统是实现这一向意图计算转变的关键推动力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://helpforsoul.com/agentic-operating-system/">Agentic Operating System : Why the Next AI Battle... - helpforsoul.com</a></li>
<li><a href="https://www.nexairi.com/article/Technology/on-device-ai-agents-google-samsung/">On - Device AI Agents Are Quietly Reshaping Your ... | Nexairi</a></li>
<li><a href="https://link.springer.com/chapter/10.1007/978-3-032-02106-9_1">Towards Using Natural Language to Perform Robotic Tasks</a></li>

</ul>
</details>

**标签**: `#Mobile OS`, `#AI Agents`, `#Human-Computer Interaction`, `#On-Device AI`, `#Operating Systems`

---