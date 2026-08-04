---
layout: default
title: "Horizon Summary: 2026-08-04 (ZH)"
date: 2026-08-04
lang: zh
---

> From 29 items, 6 important content pieces were selected

---

1. [OpenAI 宣布在数学和理论计算机科学领域取得十项突破，并附有 Lean 证明。](#item-1) ⭐️ 9.0/10
2. [ComfyUI 为开源权重模型 MiniMax H3 提供 Day-0 支持](#item-2) ⭐️ 8.0/10
3. [DNA 分析设备安全漏洞使美国 30 年犯罪证据面临无法察觉的篡改风险。](#item-3) ⭐️ 8.0/10
4. [英伟达 CMP 170HX 矿卡被破解，解锁 80GB 显存导致二手价暴涨](#item-4) ⭐️ 8.0/10
5. [英国政府要求苹果为英国公民的加密 iCloud 备份创建后门](#item-5) ⭐️ 8.0/10
6. [苹果批准微软请求，iPhone 与 Windows 跨设备剪贴板共享功能将随 iOS 28 登陆欧盟](#item-6) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [OpenAI 宣布在数学和理论计算机科学领域取得十项突破，并附有 Lean 证明。](https://openai.com/index/ten-advances-in-mathematics/) ⭐️ 9.0/10

OpenAI 宣布，其未发布的 Astra 模型在几何、编码理论、计算复杂性、群论和量子信息等多个领域解决了十个难题。每个解决方案都附有由 Lean 4 定理证明器生成的形式化证明证书，使结果可被独立验证。 这标志着 AI 在执行复杂的结构化推理和形式化验证方面的能力取得了重大飞跃，这些领域以往主要由人类专家主导。这表明 AI 正成为推动数学和计算机科学基础研究的强大工具，可能加速这些领域的发现进程。 这些突破横跨多个子领域，表明 AI 具备广泛的能力而非仅限于某个专门方向。虽然结果通过公开的 Lean 证明变得可验证，但底层的 Astra 模型本身尚未发布，且这些发现尚未经过传统的同行评审。

hackernews · milkshakes · Aug 3, 16:27 · [社区讨论](https://news.ycombinator.com/item?id=49157930)

**背景**: 理论计算机科学研究计算背后的数学基础，包括计算复杂性、密码学等领域。近年来，像大语言模型（LLM）这样的 AI 模型越来越多地被用于解决形式化的数学问题，例如 Google DeepMind 在 cap set 问题上的工作就展示了其潜力。像 Lean 这样的形式化验证工具允许将数学证明编写成代码，并由计算机检查其绝对正确性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://remoteautopilot.com/top-math-computing-advances/">Advances in Mathematics and Theoretical Computer Science</a></li>
<li><a href="https://beyondtmrw.org/article/ten-advances-in-mathematics-and-theoretical-computer-science">OpenAI Mathematics Advances: Ten Breakthroughs in 2026</a></li>
<li><a href="https://www.technologyreview.com/2023/12/14/1085318/google-deepmind-large-language-model-solve-unsolvable-math-problem-cap-set/">Google DeepMind used a large language model to solve an unsolved math problem | MIT Technology Review</a></li>

</ul>
</details>

**社区讨论**: 评论者讨论了 AI 进步的指数级速度及其对数学等领域的变革性影响，指出 AI 现在可以生成和验证证明。一些人对 AI 不可否认的影响表示惊叹，而另一些人则希望专家能分析这些具体进展的新颖性和重要性。有观点将这一情况与道格拉斯·亚当斯的幽默相比较，认为 AI 可以通过人类无法匹敌的计算“苦工”来高效地证伪猜想。

**标签**: `#artificial-intelligence`, `#mathematics`, `#theoretical-computer-science`, `#research-breakthrough`, `#openai`

---

<a id="item-2"></a>
## [ComfyUI 为开源权重模型 MiniMax H3 提供 Day-0 支持](https://blog.comfy.org/p/minimax-h3-day-0-support-in-comfyui) ⭐️ 8.0/10

流行的基于节点的 AI 生成工作流工具 ComfyUI 已为新发布的开源权重模型 MiniMax H3 提供了 day-zero 支持。此次集成使用户能够在本地运行该模型，生成 2K 分辨率的视频和音频，并通过显著的内存优化将模型占用空间减少了 66%。 这很重要，因为它将前沿的高质量视频生成能力直接带到了本地消费级硬件上，使这项原本局限于研究实验室或云服务的技术得以普及。它加速了开源权重模型被集成到实用、用户友好的创意工具中的趋势，为艺术家和开发者赋能。 内存优化是通过将模型中约 40%的调制权重剪枝并替换为功能等效的查找表实现的。虽然这使得在 RTX 3060 等 GPU 上进行本地生成成为可能，但性能仍需考虑，早期报告显示在 RTX 4070 Ti Super 上生成一段 10 秒的 480p 视频需要 10 分钟。

hackernews · vblanco · Aug 3, 13:34 · [社区讨论](https://news.ycombinator.com/item?id=49155629)

**背景**: ComfyUI 是一个基于节点的图形界面，用于创建和执行生成式 AI 工作流，允许用户将不同的模型和流程串联起来。MiniMax H3 是最近发布的一个开源权重通用多模态模型，旨在根据文本、图像、视频和音频输入的组合来生成视频、音频和图像。'Day-zero 支持'指的是在新模型或系统公开发布的当天，软件兼容性就已可用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/MiniMaxAI/MiniMax-H3">MiniMaxAI/MiniMax-H3 · Hugging Face</a></li>
<li><a href="https://docs.comfy.org/development/core-concepts/nodes">Nodes - ComfyUI</a></li>
<li><a href="https://www.anoopcnair.com/intune-fully-supports-ios-ipados-18-macos-15/">Intune Fully Supports IOS IPadOS 18 And MacOS 15 New Features...</a></li>

</ul>
</details>

**社区讨论**: 社区讨论突出了对模型高质量输出和内存减少技术成就的兴奋，但也包含了对消费级硬件上生成速度的实际担忧。用户对许多场景下的视觉质量印象深刻，但也指出在遇到更不寻常或复杂的提示时性能会下降。此外，社区对权重剪枝优化方法及其对 LLM 等其他模型的潜在适用性也表现出技术上的好奇。

**标签**: `#video-generation`, `#ai-models`, `#comfyui`, `#open-weights`, `#local-ai`

---

<a id="item-3"></a>
## [DNA 分析设备安全漏洞使美国 30 年犯罪证据面临无法察觉的篡改风险。](https://www.wsj.com/tech/cybersecurity/security-flaw-placed-30-years-of-dna-evidence-at-risk-of-hacking-1932775a) ⭐️ 8.0/10

研究人员发现，美国多数犯罪实验室使用的 Thermo Fisher Scientific DNA 分析设备存在安全漏洞，可能导致自 1995 年以来的 DNA 扫描文件被黑客在无法察觉的情况下篡改。他们利用 Anthropic 的 Claude 生成的 AI 代码，仅用约 45 分钟就成功修改了文件，且未触发常用分析软件的警报。 该漏洞威胁着刑事案件中使用的数十年法医证据的完整性，可能破坏美国的司法体系。利用 AI 技术易于实施攻击，加上全美 200 多家犯罪实验室缺乏统一监管，凸显了关键法医基础设施面临的系统性风险。 Thermo Fisher Scientific 已于 7 月私下承认这一高危漏洞，并发布了软件更新，通过添加数字签名来帮助检测篡改。该公司正与美国网络安全和基础设施安全局(CISA)合作，并表示目前尚未发现该漏洞在现实中被利用的案例。

telegram · zaihuapd · Aug 3, 05:15

**背景**: Thermo Fisher Scientific 是向法医犯罪实验室提供 DNA 分析解决方案的主要供应商。数字签名是一种用于验证数字数据真实性和完整性的密码学技术，可确保数据在签名后未被篡改。像 Claude 这样的 AI 模型可以生成代码，在本案例中，该功能被用于创建针对该漏洞的攻击程序。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.msn.com/en-us/news/other/security-flaw-placed-30-years-of-dna-evidence-at-risk-of-hacking/ar-AA29fzqF">Security flaw placed 30 years of DNA evidence at risk of hacking</a></li>
<li><a href="https://www.thermofisher.com/us/en/home/industrial/forensics/human-identification/forensic-dna-analysis/dna-analysis.html">DNA Analysis - Thermo Fisher Scientific - US</a></li>
<li><a href="https://www.signix.com/blog/bid/109951/the-easy-way-to-detect-tampering-in-digitally-signed-documents">The Easy Way to Detect Tampering in Digitally Signed Documents</a></li>

</ul>
</details>

**标签**: `#Cybersecurity`, `#Forensic Science`, `#AI Security`, `#Critical Infrastructure`, `#Vulnerability`

---

<a id="item-4"></a>
## [英伟达 CMP 170HX 矿卡被破解，解锁 80GB 显存导致二手价暴涨](https://finance.sina.com.cn/tech/roll/2026-08-03/doc-inikzqsf4659769.shtml) ⭐️ 8.0/10

亚利桑那州立大学的研究人员公开了英伟达 CMP 170HX 矿卡的破解方案，利用 Falcon 安全协处理器的栈溢出漏洞，绕过了官方的硬件熔丝锁定。该破解将显存最高扩展至 80 GB，并将 FP32 算力从 0.39 TFLOPS 暴增至 94 TFLOPS，导致该卡二手价从约 300–500 元人民币飙升至 3000–4000 元。 这一破解将一款受限制、低价值的加密货币矿卡转变为一款性能堪比昂贵 A100 的高性能 AI 计算卡，可能扰乱 AI 硬件的二手市场。它揭示了一个重大的硬件安全绕过漏洞，可能对制造商如何实施产品细分以及高端计算资源的可及性产生更广泛的影响。 解锁是通过利用 Falcon 协处理器中的 DMA 无界溢出漏洞来劫持权限并修改硬件寄存器实现的。虽然解锁后的卡现在可以在 Windows 和 Linux 下运行 AI 图像生成及大语言模型推理，但其长期稳定性以及不同生产批次的解锁上限仍是不确定的风险。

telegram · zaihuapd · Aug 3, 11:29

**背景**: 英伟达 CMP 170HX 是 2021 年推出的专用加密货币矿卡，基于与旗舰 A100 数据中心加速器相同的 GA100 GPU 核心。为防止其用于 AI 等其他应用，英伟达在制造时使用 OTP（一次性可编程）熔丝施加了不可逆的硬件锁定，从物理上限制了其显存、计算能力和 PCIe 接口。Falcon 是英伟达 GPU 内部的一个安全协处理器，负责管理安全启动和固件执行，而被利用的漏洞使研究人员得以绕过这些硬件强制实施的限制。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.osnews.com/story/137653/all-gb-s-without-flops-nvidia-cmp-170hx-review-performance-lockdown-workaround-teardown-watercooling-and-repair/">All GB/s without FLOPS – Nvidia CMP 170 HX review, performance...</a></li>
<li><a href="https://hexkyz.blogspot.com/2021/11/je-ne-sais-quoi-falcons-over-horizon.html">Hacking the planet...: Je Ne Sais Quoi - Falcons over the Horizon</a></li>
<li><a href="https://en.wikipedia.org/wiki/EFuse">eFuse - Wikipedia</a></li>

</ul>
</details>

**标签**: `#Hardware`, `#GPU`, `#Security`, `#AI Hardware`, `#Cryptocurrency Mining`

---

<a id="item-5"></a>
## [英国政府要求苹果为英国公民的加密 iCloud 备份创建后门](https://t.me/zaihuapd/42953) ⭐️ 8.0/10

英国内政部于 9 月初向苹果公司发出新的技术能力通知，要求其创建后门以访问加密的 iCloud 备份，但此次要求仅针对英国公民的数据。此前 1 月份的通知曾要求访问全球用户数据，引发了外交冲突，并导致苹果于 2 月份从英国撤回了其 iCloud 高级数据保护服务。 此举重新引发了政府为国家安全进行监控与维护用户隐私的强加密之间的根本性辩论。强制创建的后门，即使最初仅限于一个国家，也可能开创一个削弱全球加密的先例，并为其他政府要求类似访问权限树立一个危险的模板。 这一要求是根据英国的《2016 年调查权力法案》提出的，该法案授予当局发布此类通知的权力。苹果的 iCloud 高级数据保护功能使用端到端加密，只有用户受信任的设备持有密钥，这意味着苹果自身也无法解密数据，这使得遵守后门要求在技术上和理念上都极具挑战性。

telegram · zaihuapd · Aug 3, 15:40

**背景**: 技术能力通知是英国《2016 年调查权力法案》（常被称为“窥探者宪章”）下的一种法律工具，可以强制公司修改其产品或服务以协助合法监听。iCloud 高级数据保护是苹果的一项可选服务，它将端到端加密扩展到大多数 iCloud 数据，包括备份、照片和备忘录，从而防止苹果访问其内容。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Technical_capability_notice">Technical capability notice</a></li>
<li><a href="https://support.apple.com/guide/security/advanced-data-protection-for-icloud-sec973254c5f/web">Advanced Data Protection for iCloud - Apple Support</a></li>

</ul>
</details>

**标签**: `#encryption`, `#privacy`, `#government-regulation`, `#apple`, `#cloud-security`

---

<a id="item-6"></a>
## [苹果批准微软请求，iPhone 与 Windows 跨设备剪贴板共享功能将随 iOS 28 登陆欧盟](https://appleinsider.com/articles/26/08/04/iphone-to-windows-clipboard-sharing-coming-to-ios-28-in-the-eu) ⭐️ 8.0/10

苹果已批准微软提交的互操作性请求，将开发 iPhone 与 Windows PC 之间的跨设备剪贴板共享功能，预计该功能将于 2027 年秋季作为 iOS 28 的一部分面向欧盟用户推出。该请求依据欧盟《数字市场法案》（DMA）提出，于 2026 年 3 月 25 日提交，并于 6 月 26 日获批。 这标志着强制性平台互操作性迈出了重要一步，通过实现两大主要且历来存在竞争关系的平台间的无缝数据传输，直接挑战了传统的封闭生态系统。它可能重塑用户的工作流程，并为欧盟乃至全球范围内由监管压力驱动的更多跨平台功能开创先例。 该功能的实现将利用苹果的 AccessorySetupKit 框架进行一次性配对授权，类似于 iOS 26.5 中的配件通知框架。虽然该功能最初仅为欧盟开发，但苹果并未排除未来推广至全球的可能性，且其能否赶上 iOS 28 的首个正式版尚不确定。

telegram · zaihuapd · Aug 4, 03:15

**背景**: 欧盟的《数字市场法案》（DMA）将大型数字平台指定为“守门人”，并强制要求互操作性，要求它们允许第三方访问其自身服务可用的相同操作系统硬件和软件功能。AccessorySetupKit 是苹果在 iOS 18 中引入的一个框架，旨在为开发者简化蓝牙和 Wi-Fi 配件的发现、配对和绑定流程。iOS 28 是苹果移动操作系统的未来版本，预计将于 2027 年 6 月的 WWDC 大会上发布。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://digital-markets-act.ec.europa.eu/developer-portal/interoperability_en">Interoperability - Digital Markets Act (DMA) - European Commission</a></li>
<li><a href="https://developer.apple.com/videos/play/wwdc2024/10203/">Meet AccessorySetupKit - WWDC24 - Videos - Apple Developer</a></li>
<li><a href="https://memeburn.com/ios-28-release-date/">iOS 28: Release Date, New Features, Codename, and What to Expect From Apple's Biggest Update Yet - Memeburn</a></li>

</ul>
</details>

**标签**: `#Interoperability`, `#Digital Markets Act`, `#iOS`, `#Microsoft`, `#Regulation`

---