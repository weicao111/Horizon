---
layout: default
title: "Horizon Summary: 2026-08-31 (ZH)"
date: 2026-08-31
lang: zh
---

> From 24 items, 3 important content pieces were selected

---

1. [苹果发布首款 2 纳米制程的 M6 芯片及采用四芯片架构的 M5 Ultra。](#item-1) ⭐️ 9.0/10
2. [QubesOS 安全公告 QSB-118：通过复制到虚拟机错误报告在 Dom0 中执行任意代码的漏洞](#item-2) ⭐️ 8.0/10
3. [Claude 共享对话链接遭搜索引擎索引，导致用户隐私大规模泄露。](#item-3) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [苹果发布首款 2 纳米制程的 M6 芯片及采用四芯片架构的 M5 Ultra。](https://t.me/zaihuapd/43505) ⭐️ 9.0/10

据报道，苹果发布了其首款采用 2 纳米制程的 M6 芯片，以及采用全新四芯片架构的 M5 Ultra 芯片。M6 芯片在新款 Mac mini 中首发，配备 12 核 CPU 和 12 核 GPU；而 M5 Ultra 则随新款 Mac Studio 推出，最高拥有 36 核 CPU、80 核 GPU，以及高达 1.2TB/s 的统一内存带宽。 这标志着苹果在半导体技术上的一次重大飞跃，转向 2 纳米制程有望带来显著的性能和能效提升。同时，M5 Ultra 的四芯片架构也标志着苹果芯片在扩展能力上的新突破，有望为专业工作负载和 AI 应用提供前所未有的计算能力。 据报道，M6 芯片的统一内存带宽最高可达 170GB/s。M5 Ultra 的 1.2TB/s 内存带宽据称比 M3 Ultra 高出 50%，并支持高达 512GB 的统一内存，这得益于苹果的 UltraFusion 互连技术。

telegram · zaihuapd · Aug 30, 16:41

**背景**: 在半导体制造中，“2 纳米制程”指的是继 3 纳米之后的主要技术节点，能提供更高的晶体管密度和能效，但这个术语是一个营销名称，并不直接对应物理尺寸。苹果的“Ultra”芯片（如 M1 Ultra）传统上采用多芯片架构（UltraFusion），将两个 Max 芯片组合成一个更强大的片上系统（SoC）。统一内存是苹果芯片的一项关键特性，CPU、GPU 和神经网络引擎共享一个高带宽内存池，消除了数据复制开销，对 AI 和图形工作负载有益。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/2_nm_process">2 nm process - Wikipedia</a></li>
<li><a href="https://www.pcmag.com/news/apple-m5-ultra-and-m6-silicon-explained">Apple M5 Ultra and M6 Silicon Explained: 2nm Tech, Quad-Die ...</a></li>
<li><a href="https://llmcheck.net/blog/apple-silicon-memory-bandwidth-llm/">Apple Silicon Memory Bandwidth & LLM Speed... — LLM Check</a></li>

</ul>
</details>

**标签**: `#Semiconductors`, `#Apple Silicon`, `#Hardware`, `#Computer Architecture`, `#Performance`

---

<a id="item-2"></a>
## [QubesOS 安全公告 QSB-118：通过复制到虚拟机错误报告在 Dom0 中执行任意代码的漏洞](https://www.qubes-os.org/news/2026/08/29/qsb-118/) ⭐️ 8.0/10

QubesOS 项目于 2026 年 8 月 29 日发布了安全公告 QSB-118，详细说明了从 Dom0 使用 `qvm-copy-to-vm` 工具时存在的一个任意代码执行漏洞。该漏洞源于 Dom0 版本工具中的错误报告函数使用了不安全的 `system()` 调用，这可能允许攻击者执行任意命令。 这是一个严重的漏洞，因为它允许在 QubesOS 中权限最高、安全最关键的域 Dom0 中执行任意代码。由于 QubesOS 是一个专注于安全、旨在实现强隔离的操作系统，Dom0 的失陷可能危及整个系统的安全模型，影响依赖它进行高安全性任务的用户。 该漏洞仅影响从 Dom0 调用的 `qvm-copy-to-vm` 命令；虚拟机到虚拟机的变体不受影响。该问题已通过将易受攻击的 `system()` 调用替换为更安全的错误报告方法得到修复。建议用户及时将系统更新到已修补的版本。

hackernews · vntok · Aug 30, 08:51 · [社区讨论](https://news.ycombinator.com/item?id=49496918)

**背景**: QubesOS 是一个面向安全的操作系统，它使用虚拟化技术（通过 Xen 虚拟机管理程序）将应用程序和系统组件隔离到不同的虚拟机中。Dom0 是初始的、具有特权的管理域，负责控制虚拟机管理程序和其他虚拟机。`qvm-copy-to-vm` 工具用于在域之间（例如从 Dom0 到虚拟机）复制文件。任意代码执行是一种安全漏洞，攻击者可以在目标系统上运行他们选择的任何代码，通常会导致系统完全被攻陷。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://doc.qubes-os.org/en/latest/user/how-to-guides/how-to-copy-from-dom0.html">How to copy from dom0 — Qubes OS Documentation</a></li>
<li><a href="https://www.qubes-os.org/news/2026/08/29/qsb-118/">QSB-118: Dom0 arbitrary code execution in qvm-copy-to-vm error reporting</a></li>
<li><a href="https://en.wikipedia.org/wiki/Arbitrary_code_execution">Arbitrary code execution - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 社区讨论承认该漏洞的严重性，同时指出其攻击面仅限于不鼓励用于常规工作的 Dom0 操作。一些评论反思了 QubesOS 的整体安全记录以及硬件加速等实际采用挑战。一个离题的讨论将 QubesOS 的安全模型与 BSD Jails 进行了比较，对其基础设计选择提出了疑问。

**标签**: `#security`, `#vulnerability`, `#qubesos`, `#operating-systems`

---

<a id="item-3"></a>
## [Claude 共享对话链接遭搜索引擎索引，导致用户隐私大规模泄露。](https://t.me/zaihuapd/43511) ⭐️ 8.0/10

Claude 的共享对话功能存在严重隐私漏洞，用户通过该功能生成的公开链接被 Google 等搜索引擎索引，导致敏感数据泄露。泄露的信息包括 API 密钥、加密货币钱包、个人简历、律师咨询记录、公司内部项目资料及社会安全号码等。 这一事件对一家主流 AI 平台构成了严重的信任危机，将高度敏感的个人和财务信息暴露在公共互联网上。它凸显了 AI 聊天应用中反复出现的安全疏忽（约一年前 ChatGPT 曾发生同类问题），引发了业界对数据处理实践的紧迫担忧。 根本原因是共享页面上缺少 `noindex` 元标签或类似指令，未能指示搜索引擎爬虫避免索引。截至报道时，Anthropic 尚未修复该漏洞，建议用户立即前往设置中的“共享对话”管理页面，手动删除涉及隐私或财务的聊天记录。

telegram · zaihuapd · Aug 31, 03:22

**背景**: Claude.ai 包含一项功能，允许用户生成一个公开链接来与他人分享特定的对话。搜索引擎索引是指 Google 等搜索引擎发现、分析并存储网页以将其纳入搜索结果的过程。`noindex` 元标签是一种标准方法，用于请求搜索引擎不要索引特定网页，通常用于私密或临时性内容。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Noindex">noindex - Wikipedia</a></li>
<li><a href="https://developers.google.com/search/docs/crawling-indexing/block-indexing">Block Search Indexing with noindex | Google Search Central ...</a></li>
<li><a href="https://www.guideflow.com/tutorial/how-to-share-a-chat-publicly-in-claudeai">How to share a chat publicly in Claude.ai - Guideflow Tutorials</a></li>

</ul>
</details>

**标签**: `#AI Safety`, `#Privacy`, `#Security Vulnerability`, `#Claude`, `#Data Leak`

---