---
layout: default
title: "Horizon Summary: 2026-08-22 (ZH)"
date: 2026-08-22
lang: zh
---

> From 31 items, 5 important content pieces were selected

---

1. [配置错误的 e164.arpa DNS 区域暴露了敏感电话号码查询，包括军事通话。](#item-1) ⭐️ 8.0/10
2. [美国公民在边境删除手机数据面临重罪指控](#item-2) ⭐️ 8.0/10
3. [DeepSeek V4 Flash 获得视觉能力，支持图像分词与自动缩放](#item-3) ⭐️ 8.0/10
4. [文件披露：Anthropic 启动“巴拿马计划”，破坏性扫描数百万册书籍训练 Claude。](#item-4) ⭐️ 8.0/10
5. [国家发改委发布对外投资管理办法修订征求意见稿，收紧资金出境并扩大安全审查范围](#item-5) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [配置错误的 e164.arpa DNS 区域暴露了敏感电话号码查询，包括军事通话。](https://lina.sh/blog/hijacking-e164-arpa) ⭐️ 8.0/10

一名安全研究人员发现，用于 e164.arpa 的公共 ENUM DNS 区域配置错误，导致其记录并意外暴露了针对数十万个电话号码的 DNS 查询。这些查询包括拨打属于军事基地和政府实体的敏感号码的尝试。 这一事件揭示了全球电话基础设施中一个关键部分存在重大且长期的安全疏忽，可能暴露敏感的呼叫模式和操作细节。它突显了关键但晦涩的遗留系统如何可能成为隐私和安全方面的单点故障。 暴露的数据是 DNS 查询日志，而非实际通话内容，但可能揭示了谁在何时试图拨打哪些敏感号码。研究人员指出，公共 ENUM 系统基本已失效，但其私有变体仍用于号码携带等服务，表明底层协议仍然具有现实意义。

hackernews · gavide · Aug 21, 13:11 · [社区讨论](https://news.ycombinator.com/item?id=49387570)

**背景**: ENUM（E.164 号码映射）是一种使用 DNS 将国际电话号码（E.164 格式）映射到互联网地址的系统。e164.arpa 域名是国际电信联盟为此目的指定的特殊 DNS 区域，旨在连接传统电话网络（PSTN）与基于 IP 的服务（如 VoIP）。对该区域的查询旨在寻找电话号码应如何通过互联网进行路由。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Telephone_number_mapping">Telephone number mapping - Wikipedia</a></li>
<li><a href="https://www.cloudns.net/enum-dns-zones/">What is ENUM? | ENUM (E.164) DNS Services | ClouDNS</a></li>
<li><a href="https://en.wikipedia.org/wiki/E.164">E.164 - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论者对研究人员报告此漏洞后未受惩罚表示惊讶，这是安全披露中常见的担忧。有人指出，讽刺的是，只有在涉及军事号码后，该问题才得到严肃关注；另一些人则讨论了 ENUM 的现状，解释其现在主要用于通过安全通道提供号码携带等私有服务。

**标签**: `#telephony`, `#DNS`, `#security`, `#infrastructure`, `#privacy`

---

<a id="item-2"></a>
## [美国公民在边境删除手机数据面临重罪指控](https://www.nytimes.com/2026/08/21/us/politics/samuel-tunick-deleted-phone-felony.html) ⭐️ 8.0/10

美国公民塞缪尔·图尼克在海关和边境保护局（CBP）官员命令其解锁手机后，因涉嫌删除手机数据而面临重罪指控。此案很可能为边境搜查期间的数据销毁和合规问题确立一个重要的法律先例。 此案之所以重要，是因为它直接检验了数字隐私与政府边境权力的法律边界，可能将保护个人数据的行为定为犯罪。其结果将对旅行者、科技用户以及数字领域中'财产'和'销毁'的法律定义产生重大影响。 这些指控突显了 CBP 在边境对电子设备进行无证搜查的广泛权力与个人数字隐私权之间的紧张关系。一个关键的法律问题是，删除数据是否构成相关法规下的'破坏财产'。

hackernews · floathub · Aug 21, 12:10 · [社区讨论](https://news.ycombinator.com/item?id=49386895)

**背景**: 根据美国法律，海关和边境保护局（CBP）基于第四修正案的'边境搜查例外'原则，拥有在入境口岸对旅行者及其物品（包括电子设备）进行无证搜查的广泛权力。CBP 指令允许进行基本搜查（审查可访问文件）和高级搜查（使用外部设备复制或分析数据），并且官员可以强制旅行者提供设备密码。这一法律框架创造了一个复杂的环境，使得数字隐私权在边境被大幅削弱。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cbp.gov/travel/cbp-search-authority/border-search-electronic-devices">Border Search of Electronic Devices at Ports of Entry</a></li>
<li><a href="https://thepixelspulse.com/posts/the-us-is-charging-an-american-citizen-for-wiping-his-phone-at-the-border/">The US is charging an American citizen for wiping his phone at the...</a></li>
<li><a href="https://iceencounter.com/know-your-rights/device-searches/">Electronic Device Searches at the Border: Your Rights in 2026</a></li>

</ul>
</details>

**社区讨论**: 社区评论反映出对技术对策和边境数据保护实用策略的高度关注。用户提出了诸如触发数据擦除的诱饵密码功能、创建可稍后恢复的加密手机镜像、以及使用自动化应用擦除设备等想法。此外，也有关于旅行中使用一次性手机的讨论，突显了社区在当前法律限制内积极寻求解决方案。

**标签**: `#digital-privacy`, `#legal`, `#border-security`, `#civil-liberties`, `#encryption`

---

<a id="item-3"></a>
## [DeepSeek V4 Flash 获得视觉能力，支持图像分词与自动缩放](https://api-docs.deepseek.com/guides/vision/) ⭐️ 8.0/10

DeepSeek 为其 v4-flash 模型发布了视觉能力，详细说明了如何根据图像尺寸进行分词，并与文本 token 一同计费。该系统还会自动调整图像大小，将较小的图像放大，较大的图像缩小至约 800x800 像素的目标分辨率。 此次升级解决了一个重要的用户痛点，即之前的模型在无法“看见”时会臆想出视觉工具，导致会话中断。它将 DeepSeek V4 Flash 转变为真正的多模态模型，扩展了其在处理截图、文档和视觉分析任务中的实用性，这对于智能体工作流和编程辅助至关重要。 图像根据其尺寸作为 token 进行计费，自动缩放使用的阈值约为 384x384 像素。社区指出的一个关键局限是，它在需要精确视觉推理的“时钟测试”中失败，且 800x800 的分辨率上限对于阅读完整 A4 页等高细节 OCR 任务可能不足。

hackernews · dares2573 · Aug 21, 10:33 · [社区讨论](https://news.ycombinator.com/item?id=49386163)

**背景**: DeepSeek V4 Flash 是一个拥有 3040 亿参数的稀疏混合专家语言模型，专为文本生成、编程和推理而设计。增加视觉能力需要图像分词，这是一个将图像压缩成 token 序列的过程，以便大语言模型能将其与文本一同处理。自动图像缩放是计算机视觉中常见的预处理步骤，用于标准化输入尺寸，但所选的目标大小会影响对细节敏感任务的性能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://build.nvidia.com/deepseek-ai/deepseek-v4-flash-0731/modelcard">deepseek-v4-flash-0731 Model by Deepseek-ai | NVIDIA NIM</a></li>
<li><a href="https://www.youngju.dev/blog/llm/2026-06-26-multimodal-tokenization-and-fusion.en">Multimodal Tokenization and Fusion — Turning Images and Audio ...</a></li>
<li><a href="https://keras.io/examples/vision/learnable_resizer/">Keras documentation: Learning to Resize in Computer Vision</a></li>

</ul>
</details>

**社区讨论**: 社区对这一期待已久的功能持积极态度，用户指出它修复了之前模型的“幻觉”问题。然而，技术批评指出，与 Qwen 等竞争对手相比，它在简单的读钟测试中失败，并且有人担心 800x800 的缩放限制可能会阻碍详细的 OCR 应用。一些用户分享了旧模型因试图分析不存在的图像而导致会话中断的实例。

**标签**: `#computer-vision`, `#llm`, `#deepseek`, `#multimodal-ai`

---

<a id="item-4"></a>
## [文件披露：Anthropic 启动“巴拿马计划”，破坏性扫描数百万册书籍训练 Claude。](https://t.me/zaihuapd/43305) ⭐️ 8.0/10

《华盛顿邮报》披露，Anthropic 在 2024 年内部启动了“巴拿马计划”，投入数千万美元，通过切掉书脊的方式“破坏性扫描”了数百万本实体书，用于训练 Claude 等模型，并强调“不想让外界知道”。文件还称其曾下载 LibGen 等“影子图书馆”的盗版数据。 这一披露揭示了主要 AI 公司为获取高质量、受版权保护的文本数据所采取的极端且有争议的措施，引发了关于版权侵权和数据来源透明度的重大法律与伦理问题。它也凸显了 AI 快速发展与知识产权保护之间的紧张关系，可能影响正在进行的法律诉讼和公众对 AI 发展的信任。 这种破坏性扫描过程旨在获取网络上尚未广泛存在的早期书籍，以提供独特的训练数据，但书籍本身被损毁。尽管有法官认为将扫描内容用于训练可能属于合理使用，但其获取方式——特别是从影子图书馆获取——仍可能构成侵权。

telegram · zaihuapd · Aug 21, 04:52

**背景**: 为 AI 训练进行的破坏性书籍扫描，是指物理上切掉书脊以高效扫描内页的做法，近期在亚马逊设施也有类似报道。影子图书馆，如 Library Genesis (LibGen)，是提供未经授权的、受版权保护的学术及大众图书和文章访问的文件共享网站。Anthropic 是一家主要的 AI 公司，以开发 Claude 系列大语言模型而闻名，这些模型的训练需要海量的文本数据。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cyberkendra.com/2026/08/amazon-scans-and-destroys-rare-books.html">Amazon Scans and Destroys Rare Books for AI Training - Report</a></li>
<li><a href="https://en.wikipedia.org/wiki/Library_Genesis">Library Genesis - Wikipedia</a></li>
<li><a href="https://www.linkedin.com/posts/worldtechnologycongress_anthropic-projectpanama-ai-activity-7425116130081615873-T4qb">Anthropic 's Secret Project Panama : Millions of Books... | LinkedIn</a></li>

</ul>
</details>

**标签**: `#AI Ethics`, `#Copyright`, `#Large Language Models`, `#Data Sourcing`, `#Anthropic`

---

<a id="item-5"></a>
## [国家发改委发布对外投资管理办法修订征求意见稿，收紧资金出境并扩大安全审查范围](https://yyglxxbsgw.ndrc.gov.cn/htmls/article/article.html?articleId=2c97d16c-9ff00a63-01a0-230bacc4-0001) ⭐️ 8.0/10

中国国家发展改革委公布了《对外投资管理办法（修订征求意见稿）》，拟取代 2017 年的《企业境外投资管理办法》。此次修订显著强化了管控，包括将安全审查范围扩大至存量资产转让，对境外再投资和返程投资实施事前报告，并建立了基于全国信用信息共享平台的联合惩戒机制。 这一政策变动标志着中国对跨境资本流动的资本项目管制和国家安全审查显著收紧。它将影响中国企业的海外扩张战略，增加金融机构的合规成本，并可能通过使某些类型的对外投资变得更加复杂和具有风险，从而影响全球投资格局。 征求意见稿引入了“实质重于形式”的原则来认定投资，并明确禁止为规避监管而“恶意分拆”项目。在广泛收紧管制的同时，它为通过合格境内机构投资者（QDII）、港股通、跨境理财通等渠道的投资提供了豁免，除非这些投资导致获得控制权或达到特定持股比例（如 10%的整数倍）。

telegram · zaihuapd · Aug 21, 13:05

**背景**: 中国的对外投资一直由国家发改委 2017 年发布的《企业境外投资管理办法》进行管理。此次修订草案与全球范围内出于国家安全原因加强对跨境投资审查的广泛趋势一致，例如美国的对外投资安全计划。“返程投资”是指境内资本通过各种渠道流出境外，再以外商直接投资的名义返回境内的投资，通常旨在获取税收或监管优惠。“全国信用信息共享平台”是中国的一个中央信用信息归集共享系统，用于共享实体的信用信息并在政府部门间实施联合惩戒。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://wiki.mbalib.com/wiki/返程投资">返程投资 - MBA智库百科</a></li>
<li><a href="https://baike.baidu.com/item/全国信用信息共享平台/19938870">全国信用信息共享平台 - 百度百科</a></li>
<li><a href="https://www.reuters.com/world/asia-pacific/china-revise-regulations-outbound-investment-2026-08-21/">China to revise regulations for outbound investment | Reuters</a></li>

</ul>
</details>

**标签**: `#Regulatory Policy`, `#Capital Controls`, `#Outbound Investment`, `#Financial Compliance`, `#China Economy`

---