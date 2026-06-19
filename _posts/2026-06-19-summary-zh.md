---
layout: default
title: "Horizon Summary: 2026-06-19 (ZH)"
date: 2026-06-19
lang: zh
---

> From 36 items, 5 important content pieces were selected

---

1. [安全研究员发现一万个分发木马的 GitHub 仓库，主要针对 AI 智能体](#item-1) ⭐️ 8.0/10
2. [医院与高校合作以低至原价 10%的成本进行药物再利用。](#item-2) ⭐️ 8.0/10
3. [苹果与英特尔达成初步芯片代工协议，据报道有美国政府推动。](#item-3) ⭐️ 8.0/10
4. [美国向 ASML 施压，称其顶级 EUV 光刻机可能已流入中国](#item-4) ⭐️ 8.0/10
5. [Midjourney 宣布进军医疗技术领域，推出超声波全身扫描仪及水疗中心](#item-5) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [安全研究员发现一万个分发木马的 GitHub 仓库，主要针对 AI 智能体](https://orchidfiles.com/github-repositories-distributing-malware/) ⭐️ 8.0/10

一位安全研究员报告称，发现了大约一万个分发木马恶意软件的 GitHub 仓库。该攻击专门针对自动化的 AI 智能体和搜索依赖项的开发者，通过创建新仓库并频繁更新以出现在搜索结果中来实现。 这代表了软件供应链攻击的一次重大演变，它利用了人们对开源平台的信任以及 AI 智能体的自动化行为。这对依赖自动化工具进行依赖管理的开发者和组织构成了直接威胁，可能导致广泛的安全漏洞。 攻击者专注于克隆新的、不太流行的仓库，而非成熟的仓库，并且他们频繁地删除和推送新提交以操纵“最后更新”时间戳。这种策略旨在规避人工审查，同时增加被自动化智能体搜索选中的机会。

hackernews · theorchid · Jun 18, 11:45 · [社区讨论](https://news.ycombinator.com/item?id=48583928)

**背景**: 软件供应链攻击是指通过破坏软件更新、构建过程或源代码来分发恶意软件，通常针对广泛使用的开源组件。自动化 AI 智能体是能够执行任务（如搜索和集成代码依赖项）且几乎无需人工监督的程序。GitHub 是托管开源代码的核心平台，这使其成为攻击者试图渗透开发工作流程的主要目标。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.comparitech.com/software-supply-chain-attacks/">Worldwide software supply chain attacks tracker (updated daily)</a></li>
<li><a href="https://futurehumanism.co/articles/ai-agent-security-vulnerabilities-2026/">AI Agent Security : Vulnerabilities That Could... | Future Humanism</a></li>
<li><a href="https://docs.github.com/en/code-security/dependabot/dependabot-alerts">Identifying vulnerabilities in your project's dependencies with Dependabot alerts - GitHub Docs</a></li>

</ul>
</details>

**社区讨论**: 社区成员分析了攻击机制，指出其目标是自动化智能体而非人类。一位开发者分享了其姓名和项目被冒用的亲身经历。其他人则讨论了现实世界的后果，将这一问题与对 AI 智能体安全性以及恶意代码易于伪装成合法代码的更广泛担忧联系起来。

**标签**: `#security`, `#software-supply-chain`, `#github`, `#malware`, `#ai-agents`

---

<a id="item-2"></a>
## [医院与高校合作以低至原价 10%的成本进行药物再利用。](https://www.kcl.ac.uk/news/hospitals-and-universities-repurposing-drugs-at-90-lower-cost) ⭐️ 8.0/10

医院和大学正在合作，系统地识别和测试现有药物的新治疗用途，与开发新药相比，成本可降低高达 90%。这种做法凸显了传统药物开发和定价模式中存在的重大系统性低效问题。 这很重要，因为它为开发新疗法提供了一条更快、更便宜的途径，有可能满足未竟的医疗需求，特别是对于那些对传统制药公司无利可图的罕见病和被忽视的疾病。它也挑战了高成本的药物开发模式，指向更可持续和可及的医疗解决方案。 一个具体例子是使用抗癌药贝伐珠单抗（Avastin，约 50 美元/剂）来治疗黄斑变性（导致失明的主要原因），而不是使用分子结构相似但经过特殊包装的雷珠单抗（Lucentis，约 1500 美元/剂）。然而，一个关键限制是，在没有原制造商同意的情况下，缺乏明确的监管途径来正式批准现有药物的新用途。

hackernews · giuliomagnifico · Jun 18, 10:33 · [社区讨论](https://news.ycombinator.com/item?id=48583386)

**背景**: 药物再利用（或重新定位）是指为现有的、已获批的药物寻找新治疗用途的过程。这种方法可以显著减少与传统从头药物发现相关的时间（从 10-17 年）、成本和失败风险。制药行业面临系统性低效问题，包括漫长的开发周期和高昂成本，这往往导致其优先开发“重磅炸弹”药物，而非针对罕见病或被忽视的热带病等利润较低疾病的疗法。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://pmc.ncbi.nlm.nih.gov/articles/PMC12926256/">Recent advances in drug repositioning and rediscovery for different...</a></li>
<li><a href="https://www.iqvia.com/blogs/2022/05/drug-repurposing-basics">Drug Repurposing Basics | IQVIA</a></li>
<li><a href="https://pmc.ncbi.nlm.nih.gov/articles/PMC12277471/">Rethinking pharmaceutical development: A not-for-profit model to address global health inequities - PMC</a></li>

</ul>
</details>

**社区讨论**: 社区评论提供了具体例子，验证了文章的前提。一位用户详述了治疗黄斑变性时使用 Avastin 与 Lucentis 的案例，强调了本质相同的药物之间巨大的价格差异。其他人分享了与资助罕见病药物再利用的非营利组织的个人联系，并批评了不良的激励机制，例如为轻微修饰的分子（如艾氯胺酮）申请专利，而不是使用更有效但已过专利期的版本（如氯胺酮）。提出的一个关键担忧是，在没有制造商参与的情况下，正式批准新用途存在监管障碍。

**标签**: `#healthcare`, `#pharmaceuticals`, `#drug-repurposing`, `#economics`, `#public-health`

---

<a id="item-3"></a>
## [苹果与英特尔达成初步芯片代工协议，据报道有美国政府推动。](https://t.me/zaihuapd/42031) ⭐️ 8.0/10

据报道，经过一年多的谈判，苹果与英特尔已达成初步协议，由英特尔为部分苹果设备代工生产芯片，双方在近几个月敲定了正式合同。此次合作据称由美国政府深度推动。 这标志着苹果供应链的重大转变，可能减少其对台积电的依赖，并使其先进芯片制造基地多元化。这对英特尔的代工业务（IFS）也是一次重大胜利，提升了其行业信誉，并与美国加强本土半导体生产的地缘政治目标相契合。 目前尚不明确英特尔将具体为 iPhone、iPad 或 Mac 中的哪类产品线代工芯片。随着与苹果协议的达成，英特尔代工服务目前已与英伟达、SpaceX 和苹果三家公司均建立了制造合作伙伴关系。

telegram · zaihuapd · Jun 18, 09:19

**背景**: 半导体代工厂（或纯代工厂）是指为其他公司设计的芯片进行制造的公司，台积电是这种商业模式的代表。英特尔传统上是一家集成设备制造商（IDM），自行设计和制造芯片；作为其 IDM 2.0 战略的一部分，英特尔于 2021 年推出了英特尔代工服务（IFS），旨在为外部客户提供制造服务。地缘政治紧张局势和供应链担忧正在推动全球半导体制造业重组，美国政府等正积极激励本土生产。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.esmchina.com/news/11503.html">官宣！Intel Foundry来了-国际电子商情</a></li>
<li><a href="https://omdia.tech.informa.com/blogs/2025/sep/the-great-decoupling-how-geopolitics-is-reshaping-semiconductor-supply-chains">The great decoupling: how geopolitics is reshaping ...</a></li>

</ul>
</details>

**标签**: `#semiconductors`, `#apple`, `#intel`, `#supply-chain`, `#geopolitics`

---

<a id="item-4"></a>
## [美国向 ASML 施压，称其顶级 EUV 光刻机可能已流入中国](https://www.bloomberg.com/news/articles/2026-06-19/us-tells-asml-it-s-concerned-china-may-have-top-chip-tool) ⭐️ 8.0/10

美国商务部长卢特尼克近期向荷兰芯片设备巨头 ASML 高管表示，怀疑一台顶级极紫外光刻机（EUV）可能已流入中国，违反美方主导的出口管制。ASML 坚决否认，强调从未向中国出口 EUV 整机，且全球运行的 314 台设备都不在中国。 如果这一指控被证实，将构成对国际制裁的重大违反，并可能严重削弱美国主导的限制中国获取先进半导体制造技术努力的有效性。此事加剧了美欧在芯片管制上的紧张关系，也可能影响美国国会正在推动的更严格的对华设备限制法案。 美方高级官员声称掌握 ASML 未善意行事的证据，包括对华出口 EUV 相关运输设备，但拒绝出示。ASML 已散发文件自证清白，并反驳称从未出口任何 EUV 专用组件。

telegram · zaihuapd · Jun 19, 03:09

**背景**: 极紫外（EUV）光刻是制造全球最先进半导体的关键技术，它使用 13.5 纳米波长的光在晶圆上刻印复杂的电路图案。荷兰公司 ASML 是全球唯一的商用 EUV 光刻系统生产商。美国以国家安全为由，实施了一系列出口管制措施，旨在限制先进半导体技术及制造设备流向中国。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Extreme_ultraviolet_lithography">Extreme ultraviolet lithography - Wikipedia</a></li>
<li><a href="https://www.congress.gov/crs_external_products/R/PDF/R48642/R48642.6.pdf">U.S. Export Controls and China: Advanced Semiconductors</a></li>

</ul>
</details>

**标签**: `#semiconductors`, `#geopolitics`, `#export-controls`, `#ASML`, `#hardware-security`

---

<a id="item-5"></a>
## [Midjourney 宣布进军医疗技术领域，推出超声波全身扫描仪及水疗中心](https://www.midjourney.com/medical/blogpost) ⭐️ 8.0/10

Midjourney 宣布正在开发一款超声波全身扫描仪，用户走入浅水池后，约 60 秒即可生成高精度 3D 身体图像，速度据称可达 MRI 的近百倍。公司计划于 2027 年在旧金山开设首个配套水疗中心，并目标在 2031 年前在全球部署超过 5 万台扫描仪。 这标志着一家领先的 AI 公司向硬件和医疗保健领域的重大战略转型，有望普及快速、非侵入性的全身成像。如果成功，它可能颠覆传统的诊断影像市场，并为预防性健康和保健创建一个新的面向消费者的模式。 该扫描仪在浅水池中使用一个由约 50 万个微型传感器组成的环。初期仅提供身体成分图，后续计划向 FDA 提交结果以申请更多诊断功能。其目标是到 2031 年在全球部署超过 5 万台设备，实现每月 10 亿次的扫描容量。

telegram · zaihuapd · Jun 19, 04:00

**背景**: Midjourney 主要以其 AI 驱动的图像生成平台而闻名。超声波成像利用高频声波创建身体内部结构的图像，通常比磁共振成像（MRI）更快且成本更低。美国食品药品监督管理局（FDA）负责监管美国的医疗器械，任何声称具有诊断功能的设备通常都需要获得 FDA 的许可或批准，这一过程的复杂程度取决于设备的风险分类。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.theverge.com/ai-artificial-intelligence/952011/midjourney-medical-ai-ultrasound-scan">Midjourney Medical goes from AI image generation to full - body ...</a></li>
<li><a href="https://www.fda.gov/patients/device-development-process/step-3-pathway-approval">Step 3: Pathway to Approval | FDA</a></li>

</ul>
</details>

**标签**: `#AI`, `#Medical Technology`, `#Hardware`, `#Company Strategy`, `#Health Diagnostics`

---