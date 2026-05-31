---
layout: default
title: "Horizon Summary: 2026-05-31 (ZH)"
date: 2026-05-31
lang: zh
---

> From 31 items, 4 important content pieces were selected

---

1. [微软计划将永久许可的 Office 降级为仅查看模式，以推动订阅服务。](#item-1) ⭐️ 8.0/10
2. [Zig 0.16.0 发布，重构构建系统并引入新 IO 机制](#item-2) ⭐️ 8.0/10
3. [教宗利奥首份通谕抨击技术救世主思想。](#item-3) ⭐️ 8.0/10
4. [OpenAI Codex 现已支持跨设备远程控制并增强桌面自动化功能](#item-4) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [微软计划将永久许可的 Office 降级为仅查看模式，以推动订阅服务。](https://consumerrights.wiki/w/Microsoft_Office_2019_and_2021_for_Mac_view-only_conversion_(2026)) ⭐️ 8.0/10

据报道，微软计划对永久许可的离线版 Office（如 Office 2019 和 2021 for Mac）进行功能降级，强制其转换为仅查看模式，从而阻止编辑功能。这一变更计划于 2026 年实施，旨在推动用户转向其基于订阅的 Microsoft 365 服务。 此举代表了软件许可模式的重大转变，它破坏了“拥有”软件的传统概念，并迫使用户接受持续付费模式。这引发了关于消费者权利、已购软件使用寿命以及整个行业从永久许可转向软件即服务（SaaS）趋势的重大问题。 据报道，此次变更专门针对 Office 2019 和 2021 for Mac，仅查看模式的转换计划在 2026 年进行。社区的一个关键推测是，如此激进的时限可能是由于 AI 实验室使用单个永久许可为多个 AI 智能体提供支持，而微软希望对此进行单独收费。

hackernews · antipurist · May 30, 23:26 · [社区讨论](https://news.ycombinator.com/item?id=48341578)

**背景**: 永久软件许可是一个传统模式，客户支付一次性费用以获得无限期使用该特定版本软件的权利，但通常不包括持续的更新或支持。相比之下，软件即服务（SaaS）或订阅模式（如 Microsoft 365）需要持续付费以获得访问权限，这包括更新和云服务。“仅查看”或“只读”模式是 Microsoft Office 等应用程序中的一种受限状态，允许打开和查看文件，但不能进行编辑。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://cpl.thalesgroup.com/software-monetization/perpetual-license">What is a Perpetual Software License</a></li>
<li><a href="https://sequoialegal.com/blog/saas-vs-perpetual-license">SaaS vs . Perpetual License : Which Is Right? | Software Licensing ...</a></li>
<li><a href="https://learn.microsoft.com/en-us/answers/questions/5722181/word-documents-view-only">Word documents View Only - Microsoft Q&A</a></li>

</ul>
</details>

**社区讨论**: 社区情绪非常负面，用户谴责此举是反消费者且违背信任的行为。关键观点包括根据消费者保护法（特别是在澳大利亚）提出法律挑战，推测 AI 智能体的使用加速了微软的计划，以及呼吁放弃微软产品，转而使用 LibreOffice 等开源替代品。

**标签**: `#microsoft`, `#software-licensing`, `#consumer-rights`, `#saas`, `#open-source`

---

<a id="item-2"></a>
## [Zig 0.16.0 发布，重构构建系统并引入新 IO 机制](https://ziglang.org/devlog/2026/#2026-05-26) ⭐️ 8.0/10

Zig 0.16.0 于 2026 年 4 月 18 日发布，引入了重大重构的构建系统和一个新的标准库 IO 机制。新的 `std.Io` 接口允许同一份代码无需重新编译，即可在单线程、多线程或事件驱动等不同并发模型下高效运行。 此次发布标志着 Zig 语言成熟度的重要一步，其重点从增加语言特性转向改进基础开发者工具和运行时性能。对快速、灵活的构建系统以及统一 IO 抽象的重视，直接解决了系统编程中的痛点，可能使 Zig 成为对性能要求高、工具链复杂的项目中更具吸引力的选择。 重构后的构建系统基于可并发执行的步骤有向无环图（DAG），提供了更高级的项目配置能力。新的 IO 机制利用 `io_uring` 和纤程（fibers）来提供高效的异步 I/O，而无需 `async/await` 关键字的语法负担，从而避免了其他语言中常见的'函数着色'问题。

hackernews · tosh · May 30, 08:38 · [社区讨论](https://news.ycombinator.com/item?id=48334048)

**背景**: Zig 是一种通用、静态类型的系统编程语言，旨在作为 C 语言的现代替代品，注重简洁性、性能和强大的工具链。其构建系统通过项目根目录的 `build.zig` 文件定义，一直是管理项目依赖和编译步骤的核心功能。'函数着色'概念指的是同步函数与异步函数在语法和语义上的割裂，Zig 的新 IO 设计旨在统一这两者。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://ziglang.org/download/0.16.0/release-notes.html">0.16.0 Release Notes ⚡ The Zig Programming Language</a></li>
<li><a href="https://daily.dev/blog/zig-async-io-io-uring-zig-0-16-rethinks-concurrent-programming/">Zig Async I/O with io_uring: How Zig 0.16 Rethinks...</a></li>
<li><a href="https://ziglang.org/learn/build-system/">Zig Build System Zig Programming Language</a></li>

</ul>
</details>

**社区讨论**: 社区反馈非常积极，用户赞扬了其对开发者体验和工具链关注度的实际改进。一位用户指出，这些改动虽然广泛，但为语言奠定了'光明的未来'，尤其赞赏新 IO 机制的灵活性。其他人则提到 Zig 作为快速原型开发的'工具语言'的优势，以及其专注于快速编译和反馈循环，而非增加新语法。

**标签**: `#programming-languages`, `#systems-programming`, `#developer-tools`, `#zig`

---

<a id="item-3"></a>
## [教宗利奥首份通谕抨击技术救世主思想。](https://www.economist.com/europe/2026/05/28/leos-first-encyclical-attacks-technological-messianism) ⭐️ 8.0/10

教宗利奥发布了他的首份通谕，这份正式教义文件直接批评了'技术弥赛亚主义'——即认为技术（尤其是人工智能）具有拯救人类根本问题的准宗教信念。这份于 2026 年 5 月下旬发布的文件，引发了关于 AI 治理和伦理的广泛讨论。 此事意义重大，因为它将一个重要的宗教和哲学声音引入了关于强大技术的局限性与治理的全球辩论中，挑战了部分科技领袖所宣扬的叙事。它将讨论从纯粹的技术或监管框架，提升到了涉及人类目的、伦理以及混淆技术进步与救赎之危险的根本性问题。 这份通谕特别提及了像 Sam Altman 和 Dario Amodei 这样的知名 AI 行业领袖的言论和抱负，他们曾使用'创造宗教'或'建造上帝'等宗教隐喻。它进入了一个由 IBM、Databricks 等组织提出的、专注于伦理、安全和公平的现有 AI 治理框架的拥挤领域，但提供了一个独特的神学视角。

hackernews · 1vuio0pswjnm7 · May 30, 10:30 · [社区讨论](https://news.ycombinator.com/item?id=48334710)

**背景**: 教宗通谕是教宗为向天主教会及更广泛的世界传达关于信仰、道德或教义的教导而发布的正式信函。'技术弥赛亚主义'指的是相信技术进步（而非精神或政治变革）是实现人类乌托邦或救赎状态的主要手段。在 AI 语境下，这通常表现为相信人工通用智能（AGI）将能单独解决复杂的全球性问题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://fiveable.me/introduction-christianity/key-terms/papal-encyclicals">Papal encyclicals Definition for Intro to Christianity |.</a></li>
<li><a href="https://www.catholicity.com/commentary/shea/02282.html">Mark Shea: Technological Messianism</a></li>
<li><a href="https://www.ibm.com/think/topics/ai-governance">What is AI Governance? | IBM</a></li>

</ul>
</details>

**社区讨论**: 社区评论反映出对通谕批评的认同以及对控制权更广泛的担忧。一些用户批评 AI 公司 CEO 患有'AI 精神病'并夸大了当前大语言模型的能力，而另一些人则将这场辩论视为关于谁应控制变革性技术——技术专家、用户、政府，或如今包括宗教权威——的更广泛权力斗争的一部分。

**标签**: `#AI Ethics`, `#Technology Governance`, `#Philosophy of Technology`, `#Societal Impact`

---

<a id="item-4"></a>
## [OpenAI Codex 现已支持跨设备远程控制并增强桌面自动化功能](https://developers.openai.com/codex/changelog#codex-2026-05-28-app) ⭐️ 8.0/10

OpenAI 的 Codex 应用现已支持跨设备远程控制，允许用户从 iOS、Android 或 Mac 设备远程启动并实时查看 Windows 端的 Codex 任务进度。此次更新还使 Codex 能在 Windows 前台运行以直接操作桌面应用，推出了展示详细使用统计与词元活动的新版个人资料页面，并将历史讨论的搜索范围扩大至对话内容与 Git 分支名称。 此次更新极大地增强了 Codex 作为协作式、一体化 AI 编程助手的能力，打破了设备壁垒，实现了跨平台的无缝工作流管理。这标志着 AI 驱动的工作流自动化迈出了重要一步，使开发者和团队能更灵活地协调任务、更快地获取上下文，从而提升复杂软件项目的开发效率。 远程控制功能可实时运行，并提供来自目标 Windows 机器的实时进度更新。本地项目中增强的线程协调功能允许添加独立的后台线程，从而为多任务处理提供更精细的控制。

telegram · zaihuapd · May 30, 10:37

**背景**: OpenAI Codex 是一个轻量级的编程智能体，通常通过命令行界面或专用桌面应用在用户本地计算机上运行，以协助完成编码任务。工作流自动化和编排工具旨在自动协调跨人员和系统的工作，减少软件开发等流程中的手动操作和错误。词元活动追踪是 AI 助手中的常见功能，用于提供与大型语言模型交互相关的使用模式和成本洞察。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developers.openai.com/codex/app">App – Codex | OpenAI Developers</a></li>
<li><a href="https://www.domo.com/glossary/workflow-orchestration">Workflow Orchestration: How It Works and Why It Matters</a></li>

</ul>
</details>

**标签**: `#AI-Assistants`, `#Developer-Tools`, `#Workflow-Automation`, `#OpenAI`, `#Cross-Platform`

---