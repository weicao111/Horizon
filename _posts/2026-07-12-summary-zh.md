---
layout: default
title: "Horizon Summary: 2026-07-12 (ZH)"
date: 2026-07-12
lang: zh
---

> From 20 items, 5 important content pieces were selected

---

1. [vLLM v0.25.0 将 Model Runner V2 设为默认引擎，移除旧版 PagedAttention，并带来重大性能升级。](#item-1) ⭐️ 8.0/10
2. [英伟达、CoreWeave 与 Nebius：GPU 热潮背后的循环融资内幕](#item-2) ⭐️ 8.0/10
3. [智谱 AI 创始人唐杰启动'摸高计划'，攻坚四大 AGI 核心挑战](#item-3) ⭐️ 8.0/10
4. [上海计划 2027 年前实现高质量脑控，推动半侵入式脑机接口临床应用并取得侵入式技术突破。](#item-4) ⭐️ 8.0/10
5. [苹果起诉 OpenAI，指控其系统性窃取商业机密以推进硬件业务](#item-5) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [vLLM v0.25.0 将 Model Runner V2 设为默认引擎，移除旧版 PagedAttention，并带来重大性能升级。](https://github.com/vllm-project/vllm/releases/tag/v0.25.0) ⭐️ 8.0/10

vLLM 项目发布了 0.25.0 版本，这是一个重大更新，将 Model Runner V2 (MRv2) 设为所有密集模型的默认执行路径，并完全移除了旧版的 PagedAttention 实现。此版本还引入了新的流式解析器引擎、支持异构词汇表的通用推测解码，并增加了对 LLaVA-OneVision-2 和 GLM-5 等新模型的支持。 此次发布标志着高性能 LLM 推理生态系统中一个核心组件的重大架构转变，有望实现更清晰、更高效、更模块化的执行。性能改进和扩展的模型支持将直接惠及依赖 vLLM 进行可扩展、低延迟模型服务的开发者和组织。 此版本包含了来自 232 位贡献者的 558 次提交，其中 64 位是新贡献者。关键的技术新增内容包括对 EVS（高效语音搜索）、实时嵌入、Mamba 混合模型的前缀缓存，以及与完整 CUDA 图兼容的动态推测解码的支持。

github · khluu · Jul 11, 20:06

**背景**: vLLM 是一个用于大语言模型（LLM）的高吞吐量、内存高效的推理和服务引擎。Model Runner V2 (MRv2) 是 vLLM 重新设计的执行核心，从头构建以解决技术债务，并在原始 V1 设计基础上提高了模块化和效率。PagedAttention 是一种注意力机制，它通过使用类似于操作系统中虚拟内存和分页的概念来更高效地管理键值（KV）缓存内存，这是 vLLM 早期版本的一项基础性创新。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://vllm.ai/blog/2026-03-24-mrv2">Model Runner V2: A Modular and Faster Core for vLLM | vLLM Blog</a></li>
<li><a href="https://docs.vllm.ai/en/v0.22.1/design/model_runner_v2/">Model Runner V2 Design Document - vLLM</a></li>
<li><a href="https://dejaflow.com/blog/2025/02/05/vllm-paged-attention/">vLLM Paged Attention : A Game Changer for Memory Efficiency</a></li>

</ul>
</details>

**标签**: `#llm-inference`, `#machine-learning`, `#open-source`, `#performance-optimization`, `#model-serving`

---

<a id="item-2"></a>
## [英伟达、CoreWeave 与 Nebius：GPU 热潮背后的循环融资内幕](https://io-fund.com/ai-stocks/nvidia-coreweave-nebius-circular-financing-gpu-boom) ⭐️ 8.0/10

一项调查分析揭示了英伟达与 CoreWeave、Nebius 等 GPU 云提供商之间的战略投资和财务关系，暗示了一种“循环融资”模式，即英伟达投资其自己的客户以推动 AI 基础设施增长。这包括据报道英伟达向 CoreWeave 投资 20 亿美元换取 9% 的股份，而后者计划在 2026 年进行高达 350 亿美元的资本支出。 这很重要，因为它加速了 AI 基础设施的部署，但也引发了关于 AI 热潮是由真实市场需求驱动还是由人为制造的增长驱动的疑问，如果整个生态系统过度依赖一家公司的财务健康状况，可能会产生系统性风险。这也凸显了英伟达对冲超大规模云厂商（如 AWS 或谷歌）开发和优先使用自家 AI 芯片的战略举措。 一个关键细节是，英伟达的 20 亿美元投资仅占 CoreWeave 2026 年计划 350 亿美元资本支出的约 5.7%，这意味着绝大部分资金来自其他来源，一些人认为这削弱了“循环融资”的说法。此外，像 Nebius 这样的提供商提供对英伟达 B200 等高端 GPU 的按需访问，但关于总容量、利用率以及此类大规模建设长期经济盈利能力的问题仍然存在。

hackernews · adletbalzhanov · Jul 11, 17:21 · [社区讨论](https://news.ycombinator.com/item?id=48873836)

**背景**: CoreWeave 是一家专门提供 GPU 计算即服务的云提供商，主要使用英伟达硬件，随着 AI 处理需求的增长，其业务激增。Nebius 是另一个专注于 AI 的云平台，旨在基于英伟达 GPU 构建和运行 AI 模型。“循环融资”指的是一种模式，即占主导地位的基础设施供应商（如英伟达）投资其下游客户（云提供商），然后这些客户利用该资本购买更多供应商的产品，可能形成一个自我强化的循环，模糊了有机需求与供应商推动的增长之间的界限。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/CoreWeave">CoreWeave - Wikipedia</a></li>
<li><a href="https://builtin.com/articles/ai-circular-financing">How Circular Financing Is Fueling the AI Boom | Built In</a></li>
<li><a href="https://nebius.com/about">About Nebius</a></li>

</ul>
</details>

**社区讨论**: 社区情绪复杂，一些评论者质疑“循环融资”论点的说服力，因为英伟达的投资只占 CoreWeave 总资本支出的很小一部分。其他人则将讨论转向 GPU 建设扩张的长期经济可行性，关注每令牌投资回报率（ROI）和潜在产能过剩等指标。也有观点认为，英伟达的投资是应对超大规模云厂商开发自家芯片的战略对冲。

**标签**: `#AI Infrastructure`, `#Nvidia`, `#Cloud Computing`, `#Business Strategy`, `#Finance`

---

<a id="item-3"></a>
## [智谱 AI 创始人唐杰启动'摸高计划'，攻坚四大 AGI 核心挑战](https://mp.weixin.qq.com/s/3CQSkf_kBnXiCDgS4L-Cgg) ⭐️ 8.0/10

智谱 AI 创始人唐杰通过内部信宣布启动'摸高计划'，将投入巨量资源攻克通往 AGI 的四座高峰：长程任务、自治智能体系统、完全自我训练和极致安全治理。公司计划投入百亿级资源重点攻坚机械可解释性，以推动黑盒模型透明化。 这标志着一家领先的中国 AI 公司从短期商业变现转向对 AGI 基础研究的重大战略投入，旨在攻克该领域最困难且最关乎安全的核心问题。其对安全性和可解释性的高度重视，回应了全球对先进 AI 系统的普遍担忧，可能影响整个行业的研究重点。 智谱当前的旗舰模型 GLM-5.2 在长上下文任务和代码能力上表现出色，被认为已接近海外最前沿模型的水平。该计划被设定为一项'不登顶就是失败'的全力攻坚目标。

telegram · zaihuapd · Jul 11, 13:59

**背景**: 人工通用智能（AGI）指的是一种假想的 AI 系统，其能够像人类一样理解、学习并在广泛的认知任务中应用智能。'长程任务'是指需要 AI 规划并执行一长串步骤的复杂问题，当前模型在这方面常常遇到困难。'机械可解释性'是 AI 安全研究的一个子领域，旨在理解神经网络（常被称为'黑盒'）的内部计算机制，使其行为更可预测并与人类价值观对齐。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Artificial_general_intelligence">Artificial general intelligence - Wikipedia</a></li>
<li><a href="https://metr.org/blog/2025-03-19-measuring-ai-ability-to-complete-long-tasks/">Measuring AI Ability to Complete Long Tasks - METR</a></li>
<li><a href="https://arxiv.org/abs/2404.14082">[2404.14082] Mechanistic Interpretability for AI Safety -- A Review</a></li>

</ul>
</details>

**标签**: `#AGI`, `#AI Safety`, `#AI Research`, `#Company Strategy`

---

<a id="item-4"></a>
## [上海计划 2027 年前实现高质量脑控，推动半侵入式脑机接口临床应用并取得侵入式技术突破。](https://t.me/zaihuapd/42501) ⭐️ 8.0/10

上海市科学技术委员会印发了《上海市脑机接口未来产业培育行动方案（2025-2030 年）》，设定了到 2027 年实现高质量脑控的目标。该方案具体旨在让半侵入式脑机接口产品在国内率先实现临床应用，并在侵入式脑机接口研发上取得突破。 这一政府支持的路线图标志着推动脑机接口技术从研究走向实际医疗应用的一次重大、协调的行动，尤其针对失语、瘫痪等患者。它将上海乃至中国定位为全球神经技术商业化竞赛中的重要参与者，并可能加速改变生活的辅助设备的开发。 该行动方案包含一个具体里程碑，即推动 5 款以上侵入式、半侵入式脑机接口产品完成医疗器械型式检验和临床试验。其首要的初期应用重点是帮助患者恢复部分语言和运动功能。

telegram · zaihuapd · Jul 11, 15:49

**背景**: 脑机接口（BCI）在大脑与外部设备之间建立了一条直接的通信通路。根据侵入性程度，主要分为三类：非侵入式（如脑电图头戴设备）、半侵入式（通常放置于大脑表面或颅骨内，但不深入脑组织）和侵入式（直接植入脑组织，能提供更高的信号保真度）。侵入式脑机接口，例如 Neuralink 在 2024 年实现人体植入的技术，是恢复复杂运动功能的一个重要前沿领域。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://eu.36kr.com/en/p/3644383440572292">Mind-Controlled Object Manipulation: A Reality, Brain - Computer ...</a></li>
<li><a href="http://www.ks-chip.com/en/news/show-913.html">Global BCI: 2024 Breakthroughs and Future Prospects - Kingsense-high precision sensor chip</a></li>

</ul>
</details>

**标签**: `#brain-computer-interface`, `#neurotechnology`, `#medical-devices`, `#government-policy`, `#china-tech`

---

<a id="item-5"></a>
## [苹果起诉 OpenAI，指控其系统性窃取商业机密以推进硬件业务](https://t.me/zaihuapd/42502) ⭐️ 8.0/10

7 月 10 日，苹果在美国加州北区联邦法院起诉 OpenAI、两名前苹果员工以及公司 io Products。诉讼指控 OpenAI 通过系统性获取并利用苹果的产品设计、制造工艺及供应链机密，以加快其消费级硬件研发。 这起诉讼标志着传统硬件巨头与向实体产品扩张的 AI 原生公司之间竞争的重大升级。如果指控成立，可能会严重损害 OpenAI 的硬件雄心，导致巨额罚款，并为 AI 公司如何招聘人才和处理竞争情报设定法律先例。 具体指控包括前员工 Chang Liu 在离职后仍访问苹果内部网络并下载数十份硬件文件，以及 OpenAI 硬件负责人 Tang Yew Tan 被指在离职前将供应商资料发送至个人邮箱。OpenAI 收购 Jony Ive 的初创公司'io'（现已更名为'io Products'）是本次被指控的硬件推进计划的核心。

telegram · zaihuapd · Jul 11, 16:29

**背景**: 商业机密是指能为企业带来竞争优势的保密商业信息（如设计或工艺），通过盗窃或违反保密义务等手段窃取商业机密属于违法行为。io Products 是一家由苹果前设计主管 Jony Ive 等人于 2024 年创立的 AI 硬件初创公司，近期被 OpenAI 收购。供应链攻击是指通过破坏产品的制造或分销环节来获取未经授权的访问或信息，这一概念与本案中被指控的供应商数据窃取相关。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Io_(company)">io ( company ) - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Trade_secret">Trade secret - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Supply_chain_attack">Supply chain attack - Wikipedia</a></li>

</ul>
</details>

**标签**: `#Legal`, `#Artificial Intelligence`, `#Hardware`, `#Corporate Espionage`, `#OpenAI`

---