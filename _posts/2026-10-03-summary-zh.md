---
layout: default
title: "Horizon Summary: 2026-10-03 (ZH)"
date: 2026-10-03
lang: zh
---

> From 28 items, 5 important content pieces were selected

---

1. [Google Research 公布 Cogentic，一个用于自动发现数学证明的多智能体系统](#item-1) ⭐️ 9.0/10
2. [2025 年诺贝尔生理学或医学奖授予外周免疫耐受领域的发现者。](#item-2) ⭐️ 9.0/10
3. [AI 凭借样本高效算法击败世界最强 Stratego 玩家，攻克长期存在的隐藏信息难题。](#item-3) ⭐️ 8.0/10
4. [Redis 创始人发布 DwarfStar (ds4)，一款新的高效本地大语言模型推理引擎。](#item-4) ⭐️ 8.0/10
5. [OpenAI 发布 GPT-6.1 Sol，性能接近 Astra 但价格仅为五分之一。](#item-5) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Google Research 公布 Cogentic，一个用于自动发现数学证明的多智能体系统](https://arxiv.org/abs/2609.40324v1) ⭐️ 9.0/10

Google Research 推出了 Cogentic，这是一个新颖的多智能体系统，它通过一个“证明-验证”循环来自动发现和验证数学证明。该系统已经在在线学习、拍卖理论等成熟领域的五个开放问题上产出了新的、经过领域专家独立验证的结果。 这代表了自动定理证明领域的一次重大进展，展示了人工智能在成熟研究领域生成新颖、可验证数学知识的能力。它可以加速数学发现，增强软件和硬件的形式化验证，并成为研究人员的强大工具。 该系统基于 Gemini 大语言模型构建，并采用去中心化方法，让多个独立的证明器智能体探索不同的证明方向。其一个关键组件是“验证账本”，它可持续地存储已确认的结果以供未来使用。

telegram · zaihuapd · Oct 2, 12:04

**背景**: 自动定理证明是人工智能的一个子领域，旨在使用计算机自动证明数学定理。用于证明搜索的多智能体系统（例如最近开源的 QED）将证明过程分解为规划、证明、验证等专门角色，以克服单次查询方法的局限性。形式化验证是通过数学方法证明系统设计或代码符合其规范的过程，这一概念也应用于智能合约安全等领域。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/html/2604.24021v1">QED: An Open-Source Multi-Agent System for Generating</a></li>
<li><a href="https://en.wikipedia.org/wiki/Formal_verification">Formal verification - Wikipedia</a></li>

</ul>
</details>

**标签**: `#AI Research`, `#Automated Theorem Proving`, `#Multi-Agent Systems`, `#Google Research`, `#Formal Verification`

---

<a id="item-2"></a>
## [2025 年诺贝尔生理学或医学奖授予外周免疫耐受领域的发现者。](https://t.me/zaihuapd/44174) ⭐️ 9.0/10

2025 年诺贝尔生理学或医学奖授予了玛丽·E·布伦科、弗雷德·拉姆斯德尔和坂口志文，以表彰他们在外周免疫耐受方面作出的开创性发现。 该奖项表彰了阐明免疫系统如何避免攻击自身组织的基础性研究，这一机制的失效会导致自身免疫性疾病。他们的工作对开发治疗多发性硬化症、1 型糖尿病和类风湿性关节炎等疾病的新疗法具有深远意义。 获奖者的研究具体阐明了维持外周耐受的关键机制，例如调节性 T 细胞（Tregs）的作用。弗雷德·拉姆斯德尔对 Foxp3 基因的鉴定是一项关键发现，将该基因与 Tregs 的发育和功能联系起来。

telegram · zaihuapd · Oct 2, 14:15

**背景**: 免疫耐受是免疫系统区分自身与非自身、防止攻击自身细胞的能力。中枢耐受发生在胸腺等初级淋巴器官，许多自身反应性免疫细胞在此被清除。外周耐受是第二道防线，在淋巴结和组织中发挥作用，主要通过克隆删除、失能以及调节性 T 细胞（Tregs）的作用来控制那些逃逸了中枢耐受的自身反应性细胞。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Peripheral_immune_tolerance">Peripheral immune tolerance</a></li>
<li><a href="https://en.wikipedia.org/wiki/Fred_Ramsdell">Fred Ramsdell - Wikipedia</a></li>

</ul>
</details>

**标签**: `#Nobel Prize`, `#Immunology`, `#Medical Research`, `#Physiology`, `#Science News`

---

<a id="item-3"></a>
## [AI 凭借样本高效算法击败世界最强 Stratego 玩家，攻克长期存在的隐藏信息难题。](https://arstechnica.com/science/2026/10/ai-finally-beat-the-best-stratego-player-in-history-and-did-it-on-a-budget/) ⭐️ 8.0/10

由卡内基梅隆大学、MIT、纽约大学和斯坦福大学的研究人员开发的 AI 系统 Ataraxos，以 15 胜 4 平 1 负的战绩，决定性击败了被广泛认为是史上最强的 Stratego 玩家 Pim Niemeijer。这一突破是通过一种新颖的、样本高效的算法实现的，该算法仅需 16 块 GPU 进行训练，且所需的训练对局数比之前的顶尖 Stratego AI 减少了约 34 倍。 这一成就标志着 AI 在处理复杂的不完美信息博弈方面取得了重大里程碑，这一领域长期以来一直是强化学习和战略推理的主要挑战。开发出样本高效且计算成本可控的解决方案，为将类似技术应用于涉及隐藏信息的现实世界问题（如谈判、网络安全和金融市场）铺平了道路。 AI 系统 Ataraxos 为强化学习和搜索建立了一种新的设计模式，该模式在大量隐藏信息下依然有效。其训练成本相对较低，仅需几千美元和 16 块 GPU，与之前的大型 AI 项目相比，这是一项更易于实现的突破。

hackernews · PaulHoule · Oct 2, 14:11 · [社区讨论](https://news.ycombinator.com/item?id=49933740)

**背景**: Stratego 是一款经典的双人棋盘游戏，每位玩家秘密布置一支由 40 个棋子组成的军队，棋子有不同的军衔、炸弹和一面军旗。对 AI 的核心挑战在于游戏的“不完美信息”——玩家在开始时无法看到对手棋子的身份和布局，这需要基于概率、虚张声势和长期策略进行推理。此前 AI 在象棋和围棋等游戏中的成功涉及的是“完美信息”（所有棋子都可见），这使得 Stratego 成为一个更难解决的问题，直到现在才被 AI 以超人类水平攻克。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://deepmind.google/blog/mastering-stratego-the-classic-game-of-imperfect-information/">Mastering Stratego , the classic game of imperfect information</a></li>
<li><a href="https://www.nature.com/articles/s41586-026-11036-y?error=cookies_not_supported&code=99150def-d132-4ca6-8dde-5d145b1e2185">Scalable decision-making for games of imperfect information | Nature</a></li>

</ul>
</details>

**社区讨论**: 社区成员对 Stratego（一些人认为它相对简单）竟然对 AI 构成如此艰巨的挑战表示惊讶。讨论的一个关键点是算法样本效率的重要性，一位评论者指出这是在隐藏信息背景下取得成功的关键因素。其他人则强调了所使用的相对适中的计算资源（16 块 GPU），并将其与之前的大规模 AI 项目进行了对比。

**标签**: `#artificial-intelligence`, `#game-ai`, `#reinforcement-learning`, `#imperfect-information`, `#research`

---

<a id="item-4"></a>
## [Redis 创始人发布 DwarfStar (ds4)，一款新的高效本地大语言模型推理引擎。](https://dwarfstar.sh/) ⭐️ 8.0/10

Redis 的创始人 Salvatore Sanfilippo (antirez) 发布了 DwarfStar 4 (ds4)，这是一个新的、专用的 C 语言推理引擎，专门针对在配备大内存的 Mac、CUDA 和 ROCm 系统上本地运行 DeepSeek V4.1 Flash 和 Qwen3.8 Flash Next 等特定大语言模型进行了优化。 这很重要，因为它由一位著名的系统程序员推出了一款高性能、自包含的推理引擎，与 llama.cpp 或 Ollama 等更通用的解决方案相比，它可能为本地运行前沿模型提供更高的效率和更简洁的技术栈。 Ds4 的设计理念是专用而非通用，它不是一个通用的 GGUF 运行器，而是一个完全自包含的引擎，并非对其他运行时的封装。它支持文本和视觉模型，并在一个单一的技术栈内集成了命令行界面、本地 API 和原生智能体框架。

hackernews · fibo · Oct 2, 18:01 · [社区讨论](https://news.ycombinator.com/item?id=49936575)

**背景**: 像 llama.cpp 和 Ollama 这样的本地大语言模型推理引擎，允许用户在自己的硬件上运行语言模型，而无需依赖云 API。一个关键挑战是通过量化等技术，高效管理模型权重和内存（如 KV 缓存），以克服内存带宽瓶颈。这些引擎的侧重点各不相同，有的广泛支持多种模型，有的则为特定硬件或用例进行性能优化。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://dwarfstar.sh/">DwarfStar 4 (ds4): Local DeepSeek V4.1, Qwen and GLM</a></li>
<li><a href="https://github.com/stefandsl/DwarfStar">GitHub - stefandsl/DwarfStar: DeepSeek 4 Flash and PRO local ...</a></li>
<li><a href="https://developers.redhat.com/articles/2026/06/15/llamacpp-vs-vllm-choosing-right-local-llm-inference-engine">llama.cpp vs. vLLM: Choosing the right local LLM inference engine</a></li>

</ul>
</details>

**社区讨论**: 社区讨论凸显了围绕 ds4 的活跃开发，包括用于共享库和语言绑定的分支（例如 ds4go），以及针对特定硬件的适配（如 Intel Xe-LP 版本）。用户报告了在高端 Apple Silicon 上使用其速度和上下文长度的积极体验，同时也讨论了替代工具并分享了实际的使用设置。

**标签**: `#llm`, `#inference`, `#local-ai`, `#systems-programming`, `#rust`

---

<a id="item-5"></a>
## [OpenAI 发布 GPT-6.1 Sol，性能接近 Astra 但价格仅为五分之一。](https://t.me/zaihuapd/44177) ⭐️ 8.0/10

OpenAI 发布了 GPT-6 Sol 的升级版 GPT-6.1 Sol，该模型在智能体编程、计算机操作和专业任务上的性能接近 GPT-6 Astra。其输入/输出价格仅为 Astra 标准价的五分之一，缓存输入每百万 token 价格为 0.10 美元。 此次发布大幅降低了获取高性能 AI 的成本门槛，使开发者和企业能更经济地使用先进功能。这体现了 OpenAI 提供分级定价和专用模型的战略，有望加速 AI 在专业及编程工作流中的普及。 该模型目前仅向 Plus、Pro、Business、Enterprise 和 Edu 用户开放，可在 ChatGPT Work 和 Codex 中使用，但尚未进入标准的 Chat 界面。开发者可通过 API 调用 'gpt-6.1-sol' 模型端点来使用它。

telegram · zaihuapd · Oct 2, 16:21

**背景**: GPT-6 Astra 是 OpenAI 于 2026 年 9 月发布的旗舰大型语言模型（LLM），以其高智能和对齐性著称。ChatGPT Work 是 ChatGPT 中的一个智能体界面，专为复杂的多步骤项目设计，与对话式的 'Chat' 模式不同。Codex 是 OpenAI 的 AI 编程助手，可集成到各种编辑器和终端中，其 API 使用和计费通常与标准 ChatGPT 订阅分开。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/GPT-6_Astra">GPT - 6 Astra - Wikipedia</a></li>
<li><a href="https://help.openai.com/en/articles/20001275-chatgpt-work-and-codex">ChatGPT Work and Codex - OpenAI Help Center</a></li>
<li><a href="https://openai.com/codex/">Codex | AI Coding Partner from OpenAI | OpenAI</a></li>

</ul>
</details>

**标签**: `#OpenAI`, `#LLM`, `#AI-Pricing`, `#GPT-6`, `#API`

---