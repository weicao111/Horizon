---
layout: default
title: "Horizon Summary: 2026-07-08 (ZH)"
date: 2026-07-08
lang: zh
---

> From 32 items, 5 important content pieces were selected

---

1. [欧盟《聊天控制》立法提案要求扫描私人信息，威胁端到端加密。](#item-1) ⭐️ 9.0/10
2. [Januscape 漏洞：潜伏 16 年的 KVM 缺陷，允许虚拟机逃逸至 Intel 和 AMD 宿主机](#item-2) ⭐️ 9.0/10
3. [Anthropic 发布 Claude Sonnet 5，一款具备更强代理能力的新模型。](#item-3) ⭐️ 8.0/10
4. [深度求索（DeepSeek）正在自研 AI 推理芯片，以减少对英伟达和华为的依赖。](#item-4) ⭐️ 8.0/10
5. [中国商务部考虑限制国产顶尖 AI 模型对外出口](#item-5) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [欧盟《聊天控制》立法提案要求扫描私人信息，威胁端到端加密。](https://fightchatcontrol.eu/chat-control-overview) ⭐️ 9.0/10

欧盟提出了名为《聊天控制》的立法提案，其正式名称为《防止和打击儿童性虐待条例》（CSAR），该法案要求对私人数字通信内容进行扫描以查找非法材料。这包括一个允许自愿扫描的“临时减损条款”（聊天控制 1.0），以及一个正在谈判中的、可能强制要求此类扫描的更广泛的永久性法规（聊天控制 2.0）。 这项立法体现了公共安全目标与数字隐私之间的根本性冲突，因为它可能实际上强制要求在端到端加密服务中设置后门或进行客户端扫描。该法案若通过，将为大规模监控私人通信开创全球先例，影响欧盟数百万用户，并影响全球技术标准。 一个关键的技术影响是，合规性很可能要求要么通过一个“中间人”机构来破坏端到端加密，要么实施类似于苹果公司有争议的 CSAM 检测系统的设备端扫描（客户端扫描）。此外，谷歌和 Meta 等主要服务提供商已表示，即使在临时的法律依据到期后，它们也可能继续扫描。

hackernews · gasull · Jul 7, 14:23 · [社区讨论](https://news.ycombinator.com/item?id=48818311)

**背景**: 端到端加密（E2EE）是一种安全方法，只有通信双方可以读取信息，从而防止服务提供商或第三方访问加密密钥。欧盟拥有强大的数字隐私框架，特别是《通用数据保护条例》（GDPR），而这项提案可能与 GDPR 相冲突。客户端扫描是指在加密之前或之后，在用户设备上将数据与已知非法内容数据库进行比对检查。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Chat_Control">Chat Control - Wikipedia</a></li>
<li><a href="https://www.eff.org/deeplinks/2019/11/why-adding-client-side-scanning-breaks-end-end-encryption">Why Adding Client-Side Scanning Breaks End-To-End Encryption | Electronic Frontier Foundation</a></li>
<li><a href="https://en.wikipedia.org/wiki/General_Data_Protection_Regulation">General Data Protection Regulation - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 社区情绪 overwhelmingly 持批评态度，认为该法律是越权行为，利用高尚的目标（打击儿童性虐待）来为大规模监控辩护。关键观点包括：对其在不破坏加密情况下的技术可行性表示怀疑；担心这是“授予独裁权力”的把戏；并指出大型科技公司计划无论法律状态如何都进行扫描。一条评论还强调了政治影响，将反对该法律与可能禁止政党联系起来。

**标签**: `#privacy`, `#encryption`, `#surveillance`, `#eu-policy`, `#digital-rights`

---

<a id="item-2"></a>
## [Januscape 漏洞：潜伏 16 年的 KVM 缺陷，允许虚拟机逃逸至 Intel 和 AMD 宿主机](https://github.com/V4bel/Januscape) ⭐️ 9.0/10

安全研究人员公开了 Januscape 漏洞（CVE-2026-53359），这是 Linux 内核虚拟机（KVM）影子 MMU 中的一个释放后重用漏洞，允许客户虚拟机逃逸并破坏宿主机内核。该漏洞潜伏了约 16 年，是首个能在 Intel 和 AMD 平台上触发的 KVM/x86 虚拟机逃逸漏洞。 该漏洞直接威胁到多租户 KVM 宿主机（如公有云中使用的）的隔离边界，允许恶意客户机获得对宿主机的控制权。其漫长的潜伏期和跨平台特性使其对云基础设施安全构成重大威胁，可能使受影响系统（如 RHEL）上的本地普通用户提权至 root。 该漏洞存在于影子 MMU 模拟中，仅通过客户机内部操作即可触发，从而破坏宿主机的影子页状态。概念验证代码已发布，可导致宿主机内核崩溃，且该漏洞此前曾被用作 Google kvmCTF 挑战赛中的 0-day 攻击。

telegram · zaihuapd · Jul 7, 10:14

**背景**: KVM（基于内核的虚拟机）是 Linux 内核中的一个虚拟化模块，允许内核充当虚拟机监控程序（Hypervisor）。影子 MMU 是 KVM 中的一个组件，当未使用或需要模拟硬件辅助虚拟化功能（如 Intel 的 EPT 或 AMD 的 NPT）时，它负责管理客户机物理地址到宿主机物理地址的转换。释放后重用漏洞发生在程序在指针所指向的内存被释放后继续使用该指针时，这可能导致崩溃或代码执行。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thehackernews.com/2026/07/16-year-old-linux-kvm-flaw-lets-guest.html">16-Year-Old Linux KVM Flaw Lets Guest VMs Escape to Host on Intel and AMD x86 Systems</a></li>
<li><a href="https://docs.kernel.org/virt/kvm/x86/mmu.html">The x86 kvm shadow mmu — The Linux Kernel documentation</a></li>
<li><a href="https://learn.snyk.io/lesson/use-after-free/">Use after free vulnerability | Tutorial & Examples | Snyk Learn</a></li>

</ul>
</details>

**标签**: `#security`, `#virtualization`, `#linux-kernel`, `#vulnerability`, `#cloud-computing`

---

<a id="item-3"></a>
## [Anthropic 发布 Claude Sonnet 5，一款具备更强代理能力的新模型。](https://t.me/zaihuapd/42404) ⭐️ 8.0/10

Anthropic 发布了 Claude Sonnet 5，称其是迄今为止代理能力最强的 Sonnet 模型，具备更强的规划能力，并能自主使用浏览器和终端等工具。该模型在推理、工具使用、编码和知识工作方面的性能超越了 Sonnet 4.6，并接近顶级模型 Opus 4.8 的水平，同时价格更低。 此次发布极大地提升了高级 AI 代理能力的可及性，以更实惠的价格提供了接近顶级模型的性能。这使得更多开发者和企业能够构建和部署用于涉及规划与工具交互的复杂任务的、更精密的自主代理。 Claude Sonnet 5 现已面向所有套餐用户开放，并成为 Free 和 Pro 用户的默认模型。在 Claude Platform 上，其限时促销价格为每百万输入 token 2 美元、每百万输出 token 10 美元，有效期至 2026 年 8 月 31 日。

telegram · zaihuapd · Jul 7, 09:02

**背景**: Anthropic 的 Claude 模型家族包含不同层级：Haiku（速度最快）、Sonnet（性能均衡）和 Opus（能力最强）。'代理能力'指的是 AI 能够自主规划多步骤任务，并使用外部工具（如 API、浏览器或代码解释器）来实现目标，这超越了简单的问答功能。Sonnet 系列被定位为性价比高的中间选择，而此次新发布旨在将顶级的代理性能带入这个更易获取的层级。

**标签**: `#AI`, `#LLM`, `#Anthropic`, `#Claude`, `#Model Release`

---

<a id="item-4"></a>
## [深度求索（DeepSeek）正在自研 AI 推理芯片，以减少对英伟达和华为的依赖。](https://www.reuters.com/world/china/chinas-deepseek-developing-its-own-ai-chip-sources-say-2026-07-07/) ⭐️ 8.0/10

据路透社报道，中国 AI 公司深度求索（DeepSeek）已开始开发自己的 AI 芯片，该芯片专注于推理阶段，该项目始于约一年前，目前仍处于早期阶段。该公司已开始私下大量招募芯片设计工程师，并与芯片设计、代工和存储公司接洽。 这是头部 AI 公司为获得硬件独立性而采取的重大战略举措，直接影响全球 AI 供应链，并降低因美国出口管制等地缘政治限制带来的脆弱性。这也凸显了 AI 推理阶段日益增长的重要性和经济潜力，该阶段是 AI 服务的主要成本和收入驱动因素。 该芯片专为推理而非训练设计，这与为用户提供 AI 服务所需的大规模部署需求相符。深度求索此前依赖英伟达的 H800 和华为的昇腾芯片，其创始人梁文锋在 2024 年的一次采访中承认，芯片管制是公司面临的挑战。

telegram · zaihuapd · Jul 7, 11:08

**背景**: AI 芯片是专门用于人工智能工作负载的硬件。该过程主要分为两个阶段：训练（使用海量数据集教导模型）和推理（使用训练好的模型为用户生成答案）。虽然训练需要像 GPU 这样的强大芯片，但推理阶段通常需要大规模部署数量庞大的芯片来处理用户请求，这使其成为一个关键且成本高昂的运营阶段。英伟达和华为等公司是该市场的主要供应商。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.datacenterknowledge.com/data-center-chips/inference-becomes-the-next-ai-chip-battleground">Inference Becomes the Next AI Chip Battleground</a></li>
<li><a href="https://lenovopress.lenovo.com/lp1814-thinksystem-nvidia-h800-pcie-gen5-gpu">ThinkSystem NVIDIA H800 PCIe Gen5 GPUs Product Guide (withdrawn product) > Lenovo Press</a></li>

</ul>
</details>

**标签**: `#AI Hardware`, `#Semiconductors`, `#DeepSeek`, `#Supply Chain`, `#AI Inference`

---

<a id="item-5"></a>
## [中国商务部考虑限制国产顶尖 AI 模型对外出口](https://www.reuters.com/world/beijing-is-looking-curbing-overseas-access-chinas-top-ai-models-sources-say-2026-07-07/) ⭐️ 8.0/10

根据路透社的独家报道，中国商务部在过去一个月内已召集阿里巴巴、字节跳动及初创公司智谱 AI 等企业开会，讨论限制最先进的国产 AI 模型向海外提供访问，包括尚未发布的模型。会议还讨论了将 AI 核心技术泄露或窃取纳入国家安全法治罪，并考虑限制境外资本投资国内 AI 初创企业。 这一潜在的政策转变意味着一个主要 AI 大国开始将先进 AI 模型视为战略资产，这与全球技术民族主义和 AI 治理的趋势相符。它可能重塑全球 AI 竞争格局，影响国际研究合作，并冲击流入中国活跃的 AI 初创企业生态的外国投资。 限制的具体范围仍在商讨中，可能仅适用于未来发布的新模型，目前尚不确定这些措施最终是否会落地实施。报道提及的讨论方 specifically 涉及中国头部科技巨头和一家知名的 AI 初创公司，这表明政策焦点在于尖端能力。

telegram · zaihuapd · Jul 7, 11:42

**背景**: 先进的 AI 模型，特别是大语言模型（LLMs），被视为具有民用和潜在军用用途的两用技术，这导致各国从国家安全视角审视它们。中国一直在发展强大的国内 AI 产业，阿里巴巴、百度、腾讯等公司以及智谱 AI 等初创企业都在开发具有竞争力的模型。对敏感技术实施出口管制是各国用于维持战略优势、防范潜在威胁的常见工具。

**标签**: `#AI Regulation`, `#Geopolitics`, `#Technology Policy`, `#China Tech`, `#Export Controls`

---