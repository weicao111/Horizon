---
layout: default
title: "Horizon Summary: 2026-10-05 (ZH)"
date: 2026-10-05
lang: zh
---

> From 16 items, 1 important content pieces were selected

---

1. [Strata 框架使 1250 亿参数的 Qwen 3.8 Flash Next 模型在 RTX 4090 上以 100 tokens/秒的速度运行。](#item-1) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Strata 框架使 1250 亿参数的 Qwen 3.8 Flash Next 模型在 RTX 4090 上以 100 tokens/秒的速度运行。](https://github.com/Niko1221/Strata) ⭐️ 8.0/10

开源推理引擎 Strata 已成功在消费级的 NVIDIA GeForce RTX 4090 GPU 上运行 1250 亿参数的 Qwen 3.8 Flash Next 模型，速度高达每秒 100 个 token。这一成就是通过使用激进的量化技术，大幅降低了模型的内存占用实现的。 这一突破使得个人开发者和研究者无需昂贵的数据中心专用硬件，也能使用最先进的大规模多模态 AI 模型。它实现了高性能 AI 推理的民主化，并可能加速在代码辅助、多模态理解等领域的实验和应用开发。 Qwen 3.8 Flash Next 是一个混合专家模型，每个 token 仅激活约 60 亿参数，这本身就提高了效率。然而，社区测试表明，所使用的激进量化（可能低于 4-bit）可能导致在某些视觉任务上的输出质量，相比在其他框架上运行的非激进量化版本，出现可测量的下降。

hackernews · snehesht · Oct 4, 12:51 · [社区讨论](https://news.ycombinator.com/item?id=49953495)

**背景**: 量化是一种通过降低模型权重的数值精度（例如从 16-bit 降至 4-bit 或更低）来大幅减少内存需求并通常能提高推理速度的技术，但这可能会影响模型精度。Qwen 3.8 Flash Next 是阿里巴巴开源的一个大型多模态模型，采用了混合专家架构。Strata 是一个新发布的开源推理框架，专门针对在消费级 GPU 上运行此类大型量化模型进行了优化。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/qwenlm/qwen3.8-flash-next">GitHub - QwenLM/ Qwen 3 . 8 - Flash - Next : Qwen 3 . 8 - Flash - Next is the...</a></li>
<li><a href="https://reintech.io/blog/llm-quantization-explained-int8-int4-gptq-production-deployment">LLM Quantization Explained: INT8, INT4, and GPTQ for Production</a></li>

</ul>
</details>

**社区讨论**: 社区反应不一，有用户在 RTX 4090 和 RTX 5090 等硬件上报告了成功的高速运行案例，验证了其性能宣称。然而，对于激进量化带来的质量折损存在明显的怀疑，一位用户提供了基准测试数据，显示在同一个视觉任务上，与在 llama.cpp 上运行相同模型权重相比，错误率显著更高。

**标签**: `#model-inference`, `#quantization`, `#large-language-models`, `#gpu-optimization`, `#ai-hardware`

---