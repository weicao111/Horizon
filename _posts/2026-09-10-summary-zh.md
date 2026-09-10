---
layout: default
title: "Horizon Summary: 2026-09-10 (ZH)"
date: 2026-09-10
lang: zh
---

> From 37 items, 11 important content pieces were selected

---

1. [Calif Research 展示 WeWorm，一款利用 AI 辅助开发的针对微信的零点击蠕虫。](#item-1) ⭐️ 9.0/10
2. [OpenAI 称 GPT-6 Astra 的思维链可监测性显著下降](#item-2) ⭐️ 9.0/10
3. [vLLM v0.29.0 发布，Model Runner V2 成为默认引擎，新增 770B MoE 模型支持与多项性能特性。](#item-3) ⭐️ 8.0/10
4. [苹果公司发布新款可折叠智能手机 iPhone Duo。](#item-4) ⭐️ 8.0/10
5. [越来越多的证据表明自动驾驶汽车比人类驾驶员更安全。](#item-5) ⭐️ 8.0/10
6. [iPhone 18 Pro 系列发布，配备可对图像进行加密签名以验证真实性的新型相机传感器。](#item-6) ⭐️ 8.0/10
7. [关于 GPT-6 Astra 传闻、循环 Transformer 架构与隐藏推理的分析。](#item-7) ⭐️ 8.0/10
8. [GNU Radio 移植到 WebAssembly，实现浏览器内的软件定义无线电](#item-8) ⭐️ 8.0/10
9. [研究人员详述成功通过 Google Ads 投放恶意软件广告，暴露平台审核漏洞。](#item-9) ⭐️ 8.0/10
10. [OpenAI 将 AI 拓展至芯片设计领域，宣称成本低于开源模型](#item-10) ⭐️ 8.0/10
11. [蚂蚁国际与 Visa、Mastercard 合作开发 AI 代理支付标准。](#item-11) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Calif Research 展示 WeWorm，一款利用 AI 辅助开发的针对微信的零点击蠕虫。](https://simonwillison.net/2026/Sep/10/calif-research/) ⭐️ 9.0/10

安全公司 Calif Research 公开演示了 WeWorm，这是一个概念验证性的零点击蠕虫，可通过微信语音通话在 iOS 和 Android 设备上传播，无需任何用户交互即可劫持账户。该团队利用 AI 辅助，在大约两天内发现了底层漏洞并开发了远程代码执行（RCE）漏洞利用程序，完整的蠕虫构建又花费了一周时间。 此次演示标志着攻击性安全能力的急剧加速，表明 AI 可以将武器化漏洞所需的时间和专业知识从数月大幅缩短至数天。鉴于微信拥有超过 14 亿的月活跃用户，这项技术凸显了针对主要平台的潜在威胁传播速度和规模可能出现的严重增长。 即使受害者未接听电话，漏洞利用也会成功，据报道该漏洞已被腾讯修复。研究人员强调，虽然 AI 完成了大部分技术工作，但人类判断在目标选择和安全测试方面仍然至关重要。

rss · Simon Willison · Sep 10, 00:56

**背景**: 零点击漏洞利用不需要受害者进行任何交互，因此特别隐蔽和危险。远程代码执行（RCE）是一种严重的攻击，攻击者可以从远程位置在目标系统上运行任意代码。微信是一款极其流行的中国多功能即时通讯、社交媒体和移动支付应用，拥有庞大的用户基础，其安全性至关重要。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thehackernews.com/2026/09/wechat-zero-click-worm-took-over.html">WeChat Zero-Click Worm Took Over Accounts on iPhone and Android via Incoming Calls</a></li>
<li><a href="https://www.helpnetsecurity.com/2026/09/08/wechat-weworm-vulnerability-exploit-account-hijacking/">"Zero-click" WeChat worm could hijack accounts and spread via a single call - Help Net Security</a></li>
<li><a href="https://www.theregister.com/security/2026/09/09/wechat-worm-could-pwn-a-friend-before-they-even-answered-the-call/5295234">WeChat worm could pwn a friend before they even answered the call</a></li>

</ul>
</details>

**标签**: `#security`, `#ai`, `#vulnerability-research`, `#zero-click-exploit`, `#mobile-security`

---

<a id="item-2"></a>
## [OpenAI 称 GPT-6 Astra 的思维链可监测性显著下降](https://deploymentsafety.openai.com/gpt-6-astra) ⭐️ 9.0/10

OpenAI 披露，其 GPT-6 Astra 模型与前代模型相比，出现了“显著”的思维链（CoT）可监测性下降。首席科学家 Jakub Pachocki 表示，依赖 CoT 监测的能力正“逐步减弱”，部分原因是模型对其自身推理过程的控制力越来越强，并且能在更少甚至无需语言化推理的情况下完成复杂任务。 这一进展至关重要，因为思维链可监测性被认为是理解和控制先进人工智能系统的关键安全护栏。随着模型能力越来越强、内部推理越来越不明确，这种透明度的下降给 AI 安全性、可解释性以及规模化监督带来了新的挑战。 OpenAI 的官方开发文档同时提醒，Astra 的代理间消息可能出现语法或空格错误。英国 AI Safety Institute 的外部评估还发现，Astra 的原始推理更加压缩，含义不清的短语有所增加。

telegram · zaihuapd · Sep 9, 09:45

**背景**: 思维链（CoT）提示是一种通过让大语言模型生成自然语言的中间推理步骤来增强其推理能力的技术。监测这些思维链输出一直是 AI 安全领域一种有前景的方法，它提供了对模型决策过程的可见性，以检测潜在的错误行为。OpenAI 此前已发布过关于思维链可监测性和可控性的研究，强调了其重要性以及随着模型规模扩大可能出现的脆弱性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.promptingguide.ai/techniques/cot">Chain-of-Thought (CoT) Prompting</a></li>
<li><a href="https://openai.com/index/evaluating-chain-of-thought-monitorability/">Evaluating chain-of-thought monitorability - OpenAI</a></li>
<li><a href="https://arxiv.org/abs/2512.18311">[2512.18311] Monitoring Monitorability - arXiv.org Chain of Thought Monitorability:A New and Fragile Opportunity ... ICML Oral Monitoring Monitorability Reasoning Models Struggle to Control their Chains of Thought Policy Options for Preserving Chain of Thought Monitorability ...</a></li>

</ul>
</details>

**标签**: `#AI Safety`, `#Large Language Models`, `#Model Interpretability`, `#GPT-6`, `#Chain-of-Thought`

---

<a id="item-3"></a>
## [vLLM v0.29.0 发布，Model Runner V2 成为默认引擎，新增 770B MoE 模型支持与多项性能特性。](https://github.com/vllm-project/vllm/releases/tag/v0.29.0) ⭐️ 8.0/10

vLLM v0.29.0 已发布，新的 Model Runner V2 (MRV2) 成为所有模型的默认执行引擎，并新增了对包括腾讯 770B 混合专家（MoE）模型在内的多个重要模型的支持。该版本还引入了用于 KV 缓存自动调整的 CUDA 图内存分析、用于减少内存的批处理分片采样，以及对 Kimi-K3 和 DeepSeek V4 等模型的众多性能优化。 此次发布意义重大，因为 MRV2 的模块化架构和 CUDA 图分析等性能特性，使得大规模语言模型（LLM）推理能够更高效、更稳定地进行。对 770B 参数 Hy4-preview 等巨型 MoE 模型的支持，使开发者能够部署此前难以高效服务的前沿、高参数规模模型。 MRV1 仍用于部分 ROCm 模型和不支持的特性，且该版本包含了一些破坏性变更，例如移除了十个已弃用的模型架构，并将 FlexOlmo 和 Olmo3 迁移到了 Transformers 建模后端。用于 RL 权重同步的新 `sharded_rdt` P2P 后端允许每个工作节点仅拉取其张量并行/专家并行切片，从而提高了效率。

github · khluu · Sep 9, 08:54

**背景**: vLLM 是一个用于大语言模型（LLM）的高吞吐、内存高效的推理和服务引擎。Model Runner V2 (MRV2) 是 vLLM 重新设计的模块化执行核心，旨在相比之前的 V1 架构提高性能和可维护性。混合专家（MoE）模型是一种神经网络架构，其中路由器动态地仅为每个输入选择一部分专门的子网络（'专家'）进行处理，这使得模型可以拥有非常高的总参数量（如 770B），同时保持每个 token 的计算成本可控。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://vllm.ai/blog/2026-03-24-mrv2">Model Runner V2: A Modular and Faster Core for vLLM | vLLM Blog</a></li>
<li><a href="https://docs.vllm.ai/en/latest/design/model_runner_v2/">Model Runner V2 Design Document - vLLM</a></li>
<li><a href="https://www.youtube.com/watch?v=_hykItAxb5s">How Tencent Hy4 Preview Works: 770 B MoE Beats GLM-5.3 - YouTube</a></li>

</ul>
</details>

**标签**: `#llm-inference`, `#machine-learning`, `#open-source`, `#gpu-optimization`, `#model-serving`

---

<a id="item-4"></a>
## [苹果公司发布新款可折叠智能手机 iPhone Duo。](https://www.apple.com/iphone-duo/) ⭐️ 8.0/10

苹果公司正式发布了新款可折叠智能手机 iPhone Duo。这一发布引发了关于其设计、实用性和定价的广泛讨论。 这标志着苹果正式进入可折叠智能手机市场，此举可能加速这一形态设备的主流化进程，并影响针对双屏设备的应用开发。它代表了旗舰 iPhone 产品线的一次重大演进，可能重塑高端智能手机市场的竞争格局。 根据早期上手视频的反馈，该设备的柔性显示屏折痕几乎不可见。然而，产品的高昂价格被认为是其普及的一个潜在障碍。

hackernews · thecosmicfrog · Sep 9, 18:15 · [社区讨论](https://news.ycombinator.com/item?id=49630931)

**背景**: 可折叠智能手机是一种配备柔性显示屏的设备，可以折叠，在合拢时能以更紧凑的形态提供更大的屏幕面积。这项技术依赖于先进的柔性 OLED 显示屏和精密的铰链机制，使屏幕能够反复弯曲而不损坏。尽管三星、谷歌等制造商近年来已发布多款可折叠手机，但它们在耐用性、应用适配和高成本方面仍面临挑战。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Foldable_smartphone">Foldable smartphone - Wikipedia</a></li>
<li><a href="https://www.honor.com/sa-en/blog/understand-hinge-mechanism-in-foldable-phones/">Hinge Mechanism in Foldable Phones: Unfold Innovation 2025 - HONOR SA</a></li>

</ul>
</details>

**社区讨论**: 社区观点存在分歧，争论焦点集中在设备的价值主张和目标使用场景上。一些用户质疑其吸引力和高昂价格，而另一些用户则称赞其设计和几乎不可见的折痕，认为可折叠设备是未来趋势。一个值得注意的观点来自一位 Android 可折叠手机用户，他/她对苹果的入局感到兴奋，认为这可能推动整个生态系统为可折叠形态进行更好的应用优化。

**标签**: `#apple`, `#smartphones`, `#foldable-displays`, `#product-launch`, `#hardware`

---

<a id="item-5"></a>
## [越来越多的证据表明自动驾驶汽车比人类驾驶员更安全。](https://spectrum.ieee.org/are-self-driving-cars-safe) ⭐️ 8.0/10

近期的数据和分析表明，自动驾驶汽车在安全性上取得了可衡量的进步，与人类驾驶的车辆相比，事故死亡率有所降低。Waymo 等公司正在发布对比事故率数据来支持这一论断。 这具有重要意义，因为它为自动驾驶技术的核心承诺——减少交通事故死亡——提供了数据支持。如果能在更大规模上得到验证，将可能加速监管批准、提升公众接受度并推动更广泛的部署，从而从根本上改变交通安全格局。 一个关键的注意事项是，安全性的比较可能因选择的基准线而产生偏差；例如，与普通驾驶员相比和与网约车司机相比，结果会不同。此外，对这些复杂系统进行真实世界的安全验证仍然是一个重大挑战，需要依赖先进的仿真和传感器融合技术。

hackernews · bookofjoe · Sep 9, 17:14 · [社区讨论](https://news.ycombinator.com/item?id=49629886)

**背景**: 自动驾驶汽车（AV）结合使用摄像头、雷达、激光雷达等传感器以及人工智能，在没有人类干预的情况下感知环境并导航。其开发和安全性通过严格的验证与确认（V&V）流程进行评估，这通常涉及大量的仿真测试。国际自动机工程师学会（SAE International）定义了从 0 级（无自动化）到 5 级（完全自动化）的六个驾驶自动化等级，用以对车辆能力进行分类。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.appliedintuition.com/blog/metrics-that-matter">Verification & validation metrics matter | Applied Intuition</a></li>
<li><a href="https://evolutioncar.com/autonomous-driving/levels-of-autonomy-explained">Levels of Autonomous Driving Explained — SAE Levels 0-5 Guide</a></li>
<li><a href="https://blog.rgbsi.com/sensor-fusion-autonomous-driving-systems-part-1">What is Sensor Fusion for Autonomous Driving Systems? – Part 1</a></li>

</ul>
</details>

**社区讨论**: 社区观点存在分歧，部分用户对数据方法和社会优先事项提出质疑。主要观点包括：对比较组选择（例如，普通驾驶员与网约车司机）的怀疑；认为资源应投向公共交通和其他已验证的安全措施；以及观察到自动驾驶汽车对交通问题是一种“增量”而非“减量”的解决方案。

**标签**: `#autonomous-vehicles`, `#safety`, `#transportation`, `#ai`, `#data-analysis`

---

<a id="item-6"></a>
## [iPhone 18 Pro 系列发布，配备可对图像进行加密签名以验证真实性的新型相机传感器。](https://www.apple.com/newsroom/2026/09/apple-debuts-iphone-18-pro-and-iphone-18-pro-max/) ⭐️ 8.0/10

苹果发布了 iPhone 18 Pro 和 iPhone 18 Pro Max，其主摄像头配备了一款新型传感器，能够对捕获的每个像素进行加密签名。这可以生成一个不可篡改的 'Apple Reference Image'（苹果参考图像），用于证明照片是由该特定 iPhone 拍摄的真实场景。 该功能通过提供一种基于硬件的照片来源验证方法，直接应对日益严重的数字虚假信息和深度伪造问题。它可能为可信视觉媒体树立新标准，影响新闻、法律证据和在线内容验证等领域。 签名过程在拍摄时于新的 '参考模式' 中完成，签名后的传感器数据由苹果的 Private Cloud Compute（私有云计算）处理以生成最终的参考图像。值得注意的是，索尼已在其部分高端 Alpha 相机中实现了类似的机内加密认证，使用的是 ECDSA-P256 签名。

hackernews · meetpateltech · Sep 9, 17:33 · [社区讨论](https://news.ycombinator.com/item?id=49630151)

**背景**: 数字签名是一种加密方案，它使用私钥对数据进行签名，并使用对应的公钥来验证其真实性和完整性，确保数据未被篡改。在相机领域，这意味着在拍摄瞬间将像素数据和元数据绑定，创建一个防篡改的证明。这超越了传统的水印或分析 EXIF 数据等方法，后者更容易被伪造或修改。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Digital_signature">Digital signature - Wikipedia</a></li>
<li><a href="https://frameandfocal.com/camera-reviews/sonys-forgery-proof-tech-adds-crypto-signature-to-photos-in-camera">Sony’s Crypto-Stamped Photos: How Camera-Level Digital ...</a></li>
<li><a href="https://authenticity.sony.net/camera/en-us/index.html">Camera Authenticity Solution - Sony</a></li>

</ul>
</details>

**社区讨论**: 社区对新真实性功能持积极和好奇态度，用户称赞其证明图像来自真实世界的潜力。讨论还包括对其他'专业'功能的请求，如双调制解调器和 Thunderbolt 支持；对预期硬件升级（2 纳米 A20 Pro 芯片、均热板）的兴奋；以及对未公布 RAM 和内存带宽等规格的失望。

**标签**: `#apple`, `#computer-vision`, `#cryptography`, `#mobile`, `#privacy`

---

<a id="item-7"></a>
## [关于 GPT-6 Astra 传闻、循环 Transformer 架构与隐藏推理的分析。](https://magazine.sebastianraschka.com/p/gpt-6-astra-looped-transformers-and) ⭐️ 8.0/10

Sebastian Raschka 分析了关于 OpenAI GPT-6 Astra 模型的传闻，该模型据传采用了'循环 Transformer'架构，这是一种通过重复使用单一 Transformer 块来模拟深层网络的技术。讨论将这种架构选择与'隐藏推理'的概念联系起来，即模型执行的计算步骤不会直接在其输出中显现。 如果属实，这代表了前沿大语言模型设计的一个重大转变，它可能在固定的参数量预算内实现更复杂的推理，并使模型的内部'思维链'更不透明。这对 AI 安全性、可解释性以及部署强大推理模型的效率具有重大影响。 '循环 Transformer'架构并非全新概念；它是一种参数高效的设计，通过在循环过程中复用权重，有效增加了模型深度，而不会按比例增加内存使用。一个关键的注意事项是，这种技术可能将推理步骤压缩到潜在空间中，使得外部监控器更难追踪模型的决策过程。

hackernews · ModelForge · Sep 9, 14:37 · [社区讨论](https://news.ycombinator.com/item?id=49627370)

**背景**: 像 GPT 这样的 Transformer 模型通常由许多顺序层组成。'循环'或'循环深度'架构在处理过程中多次复用单一的层堆栈，这是一种权重共享的形式。'隐藏推理'指的是大语言模型在内部执行逻辑步骤，而不会将所有中间推理标记生成为可见的文本输出，这与显式的思维链提示形成对比。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.emergentmind.com/topics/looped-transformer-architecture">Looped Transformer Architecture</a></li>
<li><a href="https://arxiv.org/pdf/2503.16401">Exploring the Hidden Reasoning Process of Large Language Models ...</a></li>
<li><a href="https://www.lesswrong.com/posts/ZrgFfeWuckpwK5Lyi/hidden-reasoning-in-llms-a-taxonomy">Hidden Reasoning in LLMs: A Taxonomy — LessWrong</a></li>

</ul>
</details>

**社区讨论**: 社区评论提供了技术背景和不同的反应。一位用户澄清循环 Transformer 本质上是增加深度的权重共享，并非新颖的'秘密技术'，并链接了相关研究。另一位用户幽默地哀叹模型能力有所下降（'现在感觉像 Sol 了'），而其他人则对其展示的能力表示惊叹，并讨论了通过内部状态循环实现隐藏推理的技术定义。

**标签**: `#artificial-intelligence`, `#transformer-models`, `#llm-research`, `#gpt-6`

---

<a id="item-8"></a>
## [GNU Radio 移植到 WebAssembly，实现浏览器内的软件定义无线电](https://gnuradioworld.com/) ⭐️ 8.0/10

GNU Radio 框架的 WebAssembly 移植版本已发布，允许复杂的信号处理流程图直接在网页浏览器中运行。这使得通过 WebUSB 连接无线电硬件进行实时射频扫描和信号分析等新颖应用成为可能。 这显著降低了软件定义无线电（SDR）实验和教育的入门门槛，因为用户不再需要安装复杂的原生软件。它还为基于云的 SDR 应用以及可在任何带有浏览器的设备上访问的、可协作共享的信号处理工作流打开了大门。 该移植利用 WebAssembly 将原生 C++ 代码编译为浏览器可运行的格式，但其演示当前的可访问性和用户界面可能对新手构成挑战。与 WebUSB API 的集成是一个关键特性，允许浏览器直接控制 USRP B200 等兼容的 SDR 硬件。

hackernews · kristianpaul · Sep 9, 15:53 · [社区讨论](https://news.ycombinator.com/item?id=49628576)

**背景**: GNU Radio 是一个用于构建软件定义无线电（SDR）的免费开源软件开发工具包。SDR 在软件而非专用硬件中实现调制和滤波等无线电功能，提供了极大的灵活性。WebAssembly（Wasm）是一种二进制指令格式，允许用 C++ 等语言编写的代码在网页浏览器中以接近原生的速度运行，从而在 Web 上实现复杂的应用程序。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://drs.software/blog/what-does-porting-to-wasm-mean/">What does 'Porting' to Wasm mean? - DRS Software</a></li>
<li><a href="https://developer.mozilla.org/en-US/docs/Web/API/WebUSB_API">WebUSB API - Web APIs | MDN</a></li>
<li><a href="https://www.classcentral.com/course/udemy-software_defined_radio-467064">Online Course: Mastering Software Defined Radio ( SDR ): GNU...</a></li>

</ul>
</details>

**社区讨论**: 社区反应非常积极，专家们分享了相关的项目，如通过 WebUSB 连接的射频扫描器和 AX.25 解码器。一些用户对交互式图形界面及其教育潜力感到兴奋，而另一些人则指出该演示对新用户来说最初不够直观，缺乏清晰的入门指导。

**标签**: `#WebAssembly`, `#Software-Defined Radio`, `#Signal Processing`, `#GNU Radio`, `#WebUSB`

---

<a id="item-9"></a>
## [研究人员详述成功通过 Google Ads 投放恶意软件广告，暴露平台审核漏洞。](https://xlii.space/eng/malicious-software-on-google-ads/) ⭐️ 8.0/10

一位研究人员发布了一份第一人称技术深度分析，详细展示了他们如何成功绕过平台的自动化审核和执行系统，通过 Google Ads 为恶意软件打广告。该账户仅在问题在 Hacker News 等平台获得显著关注后才得以恢复。 这一事件凸显了谷歌自动化广告审核系统中的关键漏洞，该系统为数百万用户和企业所依赖，可能使他们面临恶意广告活动的风险。它揭示了一个更广泛的行业问题，即大型平台隐藏在自动化系统背后，使得挑战其决策或有效举报滥用行为变得困难。 研究人员的账户最初被暂停，但后来得以恢复，这表明平台的执法可能是被动反应而非主动预防。该技术利用了审核流程中的漏洞，而谷歌自身的政策在“滥用广告网络”和“恶意软件”等类别下明确禁止此类行为。

hackernews · xlii · Sep 9, 11:43 · [社区讨论](https://news.ycombinator.com/item?id=49624856)

**背景**: 恶意广告（Malvertising）是指利用在线广告传播恶意软件，通常通过将恶意代码注入合法的广告网络来实现。Google Ads 有针对恶意软件和滥用其网络的政策，但其审核流程严重依赖自动化系统，而这些系统可能被规避。最近的报告显示，网络犯罪分子劫持合法 Google Ads 账户来投放恶意广告的情况有所增加。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://support.google.com/adspolicy/answer/6020954?hl=en">Abusing the ad network - Advertising Policies Help - Google Help Hackers Exploiting Companies’ Google Ads Accounts To Serve ... Deceptive Google ads reached millions, researchers say ... How to Resolve Google Ads Disapprovals Due to Compromised ... CVE-2025-23914: Muzaara Google Ads Report Vulnerability Hackers are routing malware through Google's own ad servers ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Malvertising">Malvertising - Wikipedia</a></li>
<li><a href="https://cybersecuritynews.com/hackers-exploiting-companies-google-ads-accounts/">Hackers Exploiting Companies’ Google Ads Accounts To Serve ...</a></li>

</ul>
</details>

**社区讨论**: 评论者对谷歌过度依赖自动化系统表示失望，认为这削弱了用户的申诉渠道，并分享了遇到诈骗广告的个人经历。作者证实，在 Hacker News 上公开曝光对于账户恢复起到了关键作用，这凸显了标准支持渠道的不足。一些评论指出，恶意广告在谷歌的 YouTube 等平台上是一个普遍存在的问题。

**标签**: `#security`, `#advertising`, `#google`, `#platform-abuse`, `#social-engineering`

---

<a id="item-10"></a>
## [OpenAI 将 AI 拓展至芯片设计领域，宣称成本低于开源模型](https://www.reuters.com/world/china/openai-offers-ai-chip-design-touts-cost-advantage-over-open-source-cfo-says-2026-09-09/) ⭐️ 8.0/10

OpenAI 首席财务官萨拉·弗里尔宣布，公司正将 AI 技术拓展至芯片设计、生命科学和金融服务领域，并宣称在云端部署其低价 Luna 模型的成本低于中国的开源替代方案。OpenAI 还表示，其自研的 Jalapeno AI 芯片设计在短短九个月内即完成定稿。 此举标志着一家领先的 AI 公司向垂直整合迈出了重要一步，旨在从模型到硬件全面控制 AI 技术栈的成本和性能。其宣称的部署成本低于开源替代方案，可能会加剧全球 AI 市场的竞争，尤其是在成本敏感的地区。 其成本优势的宣称特指 GPT-5.6 Luna 模型（OpenAI 最具成本效益的层级）的云端部署。与 Broadcom 合作开发的自研 Jalapeno 芯片是一款专为 LLM 设计的推理专用集成电路（ASIC），据报道，其高性能实现是由内部 AI 系统驱动的。

telegram · zaihuapd · Sep 9, 13:06

**背景**: OpenAI 于 2026 年 7 月发布的 GPT-5.6 模型家族包含三个层级：Sol（旗舰版）、Terra（均衡版）和 Luna（针对高吞吐量工作负载的最快、最经济版本）。像 Jalapeno 这样的定制 AI 芯片属于专用集成电路（ASIC），旨在比通用硬件更高效地运行 AI 模型，这是各大科技公司为减少对英伟达等供应商的依赖并优化性能而采取的趋势。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://techjournal.org/openai-gpt-5-6-sol-terra-luna">GPT-5.6 Explained: Sol, Terra & Luna (July 2026)</a></li>
<li><a href="https://openai.com/index/openai-broadcom-jalapeno-inference-chip/">OpenAI and Broadcom unveil LLM-optimized inference chip</a></li>

</ul>
</details>

**标签**: `#AI Hardware`, `#OpenAI`, `#Chip Design`, `#Cost Optimization`, `#Industry News`

---

<a id="item-11"></a>
## [蚂蚁国际与 Visa、Mastercard 合作开发 AI 代理支付标准。](https://www.cnbc.com/2026/09/10/ant-international-visa-mastercard-ai-agent-payment-standard.html) ⭐️ 8.0/10

蚂蚁国际宣布与 Visa 和 Mastercard 合作，为 AI 代理支付制定通用标准，将建立'了解你的代理'机制。该机制旨在将代理与有效法律实体关联、评估其行为并监测风险，以提升不同支付系统间的互操作性和安全性。 此举意义重大，旨在为一个快速兴起的万亿美元级市场建立基础规则，预计到 2030 年 AI 代理将处理 3 至 5 万亿美元的消费者交易。由主要支付参与者制定的统一标准，对于确保安全、可信且可扩展的自主金融交互至关重要。 合作方援引了麦肯锡对巨大未来交易量的预测。KYA 标准侧重于身份、授权、监控、事件响应和合规准备，作为支付服务提供商的强制性基线要求，同时保持对具体技术实现的中立性。

telegram · zaihuapd · Sep 10, 03:00

**背景**: AI 代理是能够推理、学习和采取行动的自主软件程序，其在金融领域的应用正在快速增长。'了解你的代理'是一项新兴的合规标准，它将传统的'了解你的客户'逻辑延伸至自主代理，旨在识别代理交易背后应负责的法律实体。不同第三方 AI 代理之间缺乏互操作性和标准化，已被认为是金融系统中的关键挑战和风险因素。

<details><summary>参考链接</summary>
<ul>
<li><a href="http://agent-payment-standard.org/RFC/KYA_RFC/">Know Your Agent (KYA) - Agent Payment Standard (APS)</a></li>
<li><a href="https://astraea.law/insights/know-your-agent-kya-compliance-standard">Know Your Agent (KYA): The AI Compliance Standard - astraea.law</a></li>
<li><a href="https://www.deloitte.com/us/en/insights/industry/financial-services/agentic-ai-banking.html">Agentic AI in banking | Deloitte Insights</a></li>

</ul>
</details>

**标签**: `#AI-Payments`, `#Fintech`, `#Industry-Standards`, `#Financial-AI`, `#Collaboration`

---