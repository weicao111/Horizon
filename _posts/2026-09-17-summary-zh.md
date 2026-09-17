---
layout: default
title: "Horizon Summary: 2026-09-17 (ZH)"
date: 2026-09-17
lang: zh
---

> From 31 items, 3 important content pieces were selected

---

1. [英伟达宣布在 CUDA 生态中支持使用 Rust 进行原生 GPU 内核编程。](#item-1) ⭐️ 8.0/10
2. [安全研究人员曝光 Flock 监控摄像头存在硬编码凭证和严重漏洞。](#item-2) ⭐️ 8.0/10
3. [华为公布昇腾 NPU 路线图：2028 年推昇腾 970，单芯 FP4 性能达 8 PFLOPS，支持 10 万亿参数模型训练](#item-3) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [英伟达宣布在 CUDA 生态中支持使用 Rust 进行原生 GPU 内核编程。](https://developer.nvidia.com/blog/introducing-cuda-rust-two-tracks-for-writing-gpu-kernels/) ⭐️ 8.0/10

英伟达正式宣布在其 CUDA 平台内原生支持使用 Rust 编程语言编写 GPU 内核，为开发者提供了两种不同的编程路径。此举使得 Rust 开发者能够直接面向英伟达 GPU 进行编程，而无需依赖外部绑定或中间层。 此举意义重大，因为它将 Rust 的内存安全保证和现代工具链引入了高性能 GPU 计算领域，有望减少关键并行代码中的错误和安全漏洞。这标志着 CUDA 生态向 C++ 和 Fortran 之外扩展的重要一步，顺应了 Rust 在系统编程和 AI 基础设施中日益增长的趋势。 公告详细说明了编写内核的两种路径：一种是使用新的、原生的 Rust CUDA 工具链，另一种是利用现有的生态系统包（crate）。这种原生集成不同于以往依赖 C/C++ CUDA 代码外部函数接口（FFI）的社区方案。

hackernews · nonmaskable · Sep 16, 11:15 · [社区讨论](https://news.ycombinator.com/item?id=49724881)

**背景**: CUDA（统一计算设备架构）是英伟达为其 GPU 设计的专有并行计算平台和编程模型，传统上通过 C、C++ 或 Fortran 进行访问。GPU 内核是编译后在 GPU 上运行的函数；GPU 是一种专为并行计算设计的处理器，广泛应用于图形渲染、科学模拟和人工智能。原生 GPU 编程指的是直接用高级语言编写这些内核，而无需手动与 OpenCL 或 Metal 等底层 API 对接。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/CUDA">CUDA - Wikipedia</a></li>
<li><a href="https://developer.nvidia.com/cuda">CUDA Platform for Accelerated Computing | NVIDIA Developer</a></li>
<li><a href="https://carpentries-incubator.github.io/lesson-gpu-programming/first_program.html">GPU Programming: Your First GPU Kernel - Carpentries Incubator</a></li>

</ul>
</details>

**社区讨论**: 社区反应不一，一些人对此举能让 GPU 代码更可靠、并能更好地与 Candle 等 Rust 项目集成感到兴奋，而另一些人则批评 CUDA 的供应商锁定问题，并更倾向于开放标准。一条值得注意的评论指出了此举与 Hugging Face 的 Candle crate（用于 Rust AI 推理）的潜在协同效应。还有人指出该公告的写作风格与英伟达典型的技术博客不同。

**标签**: `#rust`, `#gpu`, `#nvidia`, `#parallel-computing`, `#programming-languages`

---

<a id="item-2"></a>
## [安全研究人员曝光 Flock 监控摄像头存在硬编码凭证和严重漏洞。](https://www.wired.com/story/hackers-flock-camera-data-shows-how-system-works/) ⭐️ 8.0/10

安全研究人员发现，Flock Safety 的监控摄像头存在硬编码的 API 密钥和其他严重漏洞，允许攻击者未经授权物理或逻辑访问设备，并可能触及 Flock 的后端系统。这些漏洞由研究员 Micah Lee 和 404 Media 披露，相关数据由 Distributed Denial of Secrets 发布。 此事影响重大，因为 Flock 的自动车牌识别摄像头在美国被执法部门和社区广泛部署，用于监控，其系统性的安全缺陷构成了严重的隐私和公共安全风险。这些漏洞暴露了放置在公共场所的关键监控基础设施可能被攻破，导致敏感数据泄露或服务中断。 硬编码的凭证是一个 API 密钥，可用于请求以明文存储的设备凭证，这可能获得访问 Flock 服务器的权限。值得注意的是，据报道，Flock 的漏洞披露政策设置了限制条款，禁止与设备交互或下载数据，这可能会阻碍合法的安全研究。

hackernews · driverdan · Sep 16, 13:18 · [社区讨论](https://news.ycombinator.com/item?id=49726586)

**背景**: Flock Safety 是一家生产联网自动车牌识别摄像头的公司，其产品主要用于执法部门和社区进行车辆跟踪和监控。硬编码凭证在通用缺陷枚举中被分类为 CWE-798，指的是嵌入在软件或固件中的静态密码或密钥，由于容易被提取并绕过正常身份验证，构成了严重的安全风险。这些摄像头通常部署在公共场所，是日益增长的 AI 监控基础设施网络的一部分。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://owasp.org/www-community/vulnerabilities/Use_of_hard-coded_password">Use of hard-coded password | OWASP Foundation</a></li>
<li><a href="https://en.wikipedia.org/wiki/Flock_Safety">Flock Safety - Wikipedia</a></li>
<li><a href="https://builtin.com/articles/flock-cameras">Flock Cameras Explained: What They Track and Why It Matters | Built In</a></li>

</ul>
</details>

**社区讨论**: 社区强烈批评 Flock 的安全实践，将硬编码凭证称为“完全无能”和“纯粹懒惰”的表现，其动机是为了缩短产品上市时间。社区对 Flock 的漏洞披露政策提出了大量批评，认为该政策旨在营造负责任的表象，却通过禁止与设备交互来阻碍实际研究。评论者还指出了物理安全威胁，因为放置在公共场所的摄像头易于接触，其上所有数据都可能被未经授权的人员获取。

**标签**: `#security`, `#iot`, `#privacy`, `#vulnerability`, `#surveillance`

---

<a id="item-3"></a>
## [华为公布昇腾 NPU 路线图：2028 年推昇腾 970，单芯 FP4 性能达 8 PFLOPS，支持 10 万亿参数模型训练](https://t.me/zaihuapd/43878) ⭐️ 8.0/10

在 Connect 2025 大会上，华为发布了新一代昇腾 NPU 路线图，计划在 2026 至 2028 年间推出昇腾 950、960 和 970 系列芯片。其中，计划于 2028 年末亮相的昇腾 970，其单芯片 FP4 性能将提升至 8 PFLOPS，旨在支持训练规模迈向 10 万亿参数的 AI 模型。 这一路线图标志着华为在高性能 AI 加速器市场中长期竞争的坚定决心，直接对标英伟达等行业领导者。实现单芯片 8 PFLOPS 的性能并支持 10 万亿参数模型，有望大幅降低训练前沿 AI 模型的成本和能耗，对全球 AI 研究和产业能力产生影响。 新一代芯片将全面采用全新的 SIMD+SIMT 混合架构，并加入 FP8、MXFP4、HiF4 等低精度格式以提高能效。华为同时升级其超级集群方案，单个 SuperPod 可整合 1.5 万颗芯片，以构建超大规模计算系统。

telegram · zaihuapd · Sep 17, 03:20

**背景**: NPU（神经网络处理器）是一种专为加速人工智能和机器学习工作负载而设计的专用处理器。SIMD（单指令多数据）和 SIMT（单指令多线程）是两种并行计算架构；SIMD 对规则计算效率高，而 SIMT（常用于 GPU）则为复杂任务提供了更大的灵活性。FP4、MXFP4 等低精度格式通过减少表示数据所需的比特数，旨在维持模型精度的同时，实现更快的计算速度和更低的内存占用。SuperPod（超级集群）是一种高度集成的计算架构，它通过高速互连技术将大量处理单元（如 NPU 或 GPU）集群成一个逻辑上统一的强大实体，用于大规模 AI 训练。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://public-download.obs.cn-east-2.myhuaweicloud.com/ascend/昇腾950+NPU架构白皮书.pdf">昇腾 950 NPU 架构白皮书</a></li>
<li><a href="https://arxiv.org/html/2604.08826v1">HiFloat4 Format for Language Model Pre-training on Ascend NPUs</a></li>
<li><a href="https://ascentoptics.com/blog/superpods-redefining-the-future-of-ai-computing-architecture/">SuperPods: Redefining the Future of AI Computing Architecture - AscentOptics Blog</a></li>

</ul>
</details>

**标签**: `#AI Hardware`, `#NPU`, `#Huawei`, `#Roadmap`, `#High-Performance Computing`

---