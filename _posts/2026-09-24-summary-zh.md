---
layout: default
title: "Horizon Summary: 2026-09-24 (ZH)"
date: 2026-09-24
lang: zh
---

> From 30 items, 3 important content pieces were selected

---

1. [Anthropic 的 Claude AI 自主发现新型 CRISPR 样酶系统。](#item-1) ⭐️ 9.0/10
2. [分析：LLM 推理成本下降过快，或将变得'便宜到无需计量'](#item-2) ⭐️ 8.0/10
3. [字节跳动 AI 应用豆包日活跃用户突破 1 亿，系推广成本最低的破亿产品](#item-3) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Anthropic 的 Claude AI 自主发现新型 CRISPR 样酶系统。](https://www.anthropic.com/news/claude-discovers-novel-enzyme-system) ⭐️ 9.0/10

Anthropic 宣布，其 Claude AI 智能体在分析逆转录酶附近的基因组序列时，自主发现了一个此前未知的酶系统，识别出一个让人联想到 CRISPR 的串联重复阵列。这是 Anthropic 新成立的生命科学研究实验室发布的首个成果。 这标志着 AI 能够在基因组学中自主做出新科学发现的范式转变，可能加速新生物工具和机制的识别。它凸显了 AI 智能体在分子生物学等复杂领域，正超越数据分析，进入真正的假设生成和探索阶段。 这一发现是 Claude 智能体通过挖掘约 20 万个逆转录酶序列实现的，它识别出了一个未被注意到的模式——一个与 RT 基因相邻的串联重复阵列。该相关酶系统及其伴侣基因的具体功能尚属未知，需要进一步的实验验证。

hackernews · raahelb · Sep 23, 18:06 · [社区讨论](https://news.ycombinator.com/item?id=49820134)

**背景**: CRISPR 是一种源自细菌免疫系统的革命性基因编辑技术，其特点是具有成簇规律间隔短回文重复序列（CRISPR 阵列），这些序列能引导 Cas 酶切割特定的 DNA 序列。逆转录酶是一种以 RNA 为模板合成 DNA 的酶，被 HIV 等逆转录病毒和某些遗传元件所利用。串联重复是 DNA 中核苷酸序列一个接一个重复出现的模式，在功能基因附近发现它们可能预示着新的调控或结构系统。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://interestingengineering.com/ai-robotics/claude-discovers-crispr-like-enzyme-system">Claude scans 200,000 enzymes, uncover CRISPR - like system in...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Tandem_repeat">Tandem repeat - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Reverse_transcriptase">Reverse transcriptase - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 社区情绪复杂，既有对 AI 驱动发现这一叙事的兴奋，也有对其实际新颖性和影响的怀疑。一些用户对重现发现时刻的“智能体对话记录”感到着迷，而另一些用户则质疑其实际意义，认为这仅仅是识别了一个新的基因组排列。一个显著的讨论点是 Anthropic 立场的矛盾性，它一方面警告不要将 AI 用于生物工程，另一方面又宣布了一项与基因组相关的发现。此外，也有关于语言模型如何能够对生物化学进行推理的根本性质疑。

**标签**: `#artificial-intelligence`, `#genomics`, `#crispr`, `#scientific-discovery`, `#anthropic`

---

<a id="item-2"></a>
## [分析：LLM 推理成本下降过快，或将变得'便宜到无需计量'](https://jyn.dev/tokens-too-cheap-to-meter/) ⭐️ 8.0/10

近期一篇分析文章认为，大语言模型（LLM）的推理成本正在以前所未有的速度下降，达到特定性能基准的价格每年下降 9 倍到 900 倍。作者引用了历史类比，暗示这一趋势可能导致未来生成一个 AI token 的成本变得微不足道，类似于核能'便宜到无需计量'这一未能实现的承诺。 如果这一趋势持续下去，可能会从根本上重塑 AI 经济，使先进智能成为一种近乎无处不在且负担得起的公共事业，从而释放出无数目前不具备商业可行性的新应用。然而，这也引发了关于当前大规模基础设施投资的可持续性以及 AI 公司长期商业模式的严峻问题。 分析指出，成本下降是由算法改进和硬件创新共同驱动的，但下降速度差异巨大。一个关键的警示是'斯坦因定律'的适用性——如果某事不能永远持续，它就会停止——这意味着这些指数级的效率提升可能不是无限的。

hackernews · teoruiz · Sep 23, 09:21 · [社区讨论](https://news.ycombinator.com/item?id=49813482)

**背景**: LLM 推理是指运行训练好的模型以生成预测或文本（token）的过程。其成本是 AI 服务经济性的主要因素。'便宜到无需计量'这一短语源于 1954 年美国原子能委员会主席刘易斯·斯特劳斯，他预测核能发电将变得极其便宜，以至于无需计量——这一承诺后来众所周知地未能实现。当前 AI 推理成本的降低源于专用硬件（如 NPU 和 OpenAI 的 Jalapeño 等定制芯片）的进步以及更高效的算法。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://epoch.ai/data-insights/llm-inference-price-trends">LLM inference prices have fallen rapidly but unequally across ...</a></li>
<li><a href="https://a16z.com/llmflation-llm-inference-cost/">Welcome to LLMflation – LLM inference cost is going down fast LLM API Pricing Trends & Updates (September 2026) | BenchLM.ai GitHub - MichaelKokin/llm-price-trends: LLM inference price ... AI Inference Cost Statistics 2026: The Market That Split in Two LLM inference prices have fallen rapidly but unequally across ... LLM Inference Cost 2026: Complete Pricing Guide</a></li>
<li><a href="https://web.archive.org/web/20070204122504/http://www.cns-snc.ca/media/toocheap/toocheap.html">Too Cheap to Meter ?</a></li>

</ul>
</details>

**社区讨论**: 社区讨论广泛且具有批判性，突显了对成本趋势线性外推的怀疑。关键观点包括援引'斯坦因定律'来论证效率提升不可能无限期持续，将其与核能未能兑现的承诺相类比，并批评该分析忽略了为大规模基础设施投资辩护的商业模式的可行性。此外，也有人批评了原分析中使用的可视化图表。

**标签**: `#AI Economics`, `#LLM Inference`, `#Technology Trends`, `#Business Models`, `#Hacker News`

---

<a id="item-3"></a>
## [字节跳动 AI 应用豆包日活跃用户突破 1 亿，系推广成本最低的破亿产品](https://t.me/zaihuapd/43996) ⭐️ 8.0/10

字节跳动旗下 AI 应用豆包的日均活跃用户数（DAU）已突破 1 亿大关。据内部人士透露，该产品是字节跳动历史上推广费用最低的破亿 DAU 产品。 这一里程碑意味着消费级 AI 应用获得了大规模用户采纳，可能使豆包在中国竞争激烈的 AI 助手市场中占据领先地位。其低推广成本成就凸显了高效的成长策略和强大的产品市场契合度，这可能给竞争对手带来压力，并影响整个 AI 应用市场的商业模式。 豆包是一款多模态 AI 助手，以其通过字节跳动火山引擎提供的低成本 API 定价以及在自然语言处理和图像生成方面的强大功能而闻名。虽然报告的 1 亿 DAU 是一个重要里程碑，但它代表的是特定的日活指标，并不能直接等同于收入或盈利能力。

telegram · zaihuapd · Sep 23, 06:18

**背景**: 日活跃用户数（DAU）是一个关键指标，用于统计在 24 小时内使用应用的不同用户数量，反映了应用的日常受欢迎程度和用户留存情况。豆包是字节跳动的旗舰 AI 助手，属于一个包含文本和图像生成能力的模型家族。在中国 AI 市场中，实现高 DAU 是新技术产品获得主流采纳的重要标志。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://mwm.ai/glossary/dau">Daily Active Users ( DAU ) — Definition, Benchmarks, and How... | MWM</a></li>
<li><a href="https://howaiworks.ai/ai-tools/doubao">Doubao (豆包) - AI Tool | HowAIWorks. ai</a></li>
<li><a href="https://sden.ai/learn/guides/doubao">Doubao guide · SDEN</a></li>

</ul>
</details>

**标签**: `#AI Applications`, `#User Growth`, `#ByteDance`, `#Market Milestone`

---