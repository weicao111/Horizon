---
layout: default
title: "Horizon Summary: 2026-08-05 (ZH)"
date: 2026-08-05
lang: zh
---

> From 34 items, 7 important content pieces were selected

---

1. [ChainDrop 蠕虫在大型供应链攻击中感染逾 1300 个 npm 包](#item-1) ⭐️ 9.0/10
2. [华为提出“韬定律”作为后摩尔时代新原则，以时间缩微替代几何缩微。](#item-2) ⭐️ 8.0/10
3. [谷歌联合华尔街为 Anthropic 搭建约 2000 亿美元 AI 芯片融资架构](#item-3) ⭐️ 8.0/10
4. [美国联邦通信委员会禁止进口新款中国产人形机器人、四足机器人和联网电力逆变器](#item-4) ⭐️ 8.0/10
5. [我国首部 L3/L4 自动驾驶强制性国标报批，将于 2027 年实施](#item-5) ⭐️ 8.0/10
6. [3D 打印仿生海绵体植入干细胞，成功在猪模型中恢复勃起功能。](#item-6) ⭐️ 8.0/10
7. [DeepSeek 重启第二轮融资，投前估值达 5000 亿元](#item-7) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [ChainDrop 蠕虫在大型供应链攻击中感染逾 1300 个 npm 包](https://www.bleepingcomputer.com/news/security/massive-chaindrop-npm-supply-chain-attack-infects-hundreds-of-packages/) ⭐️ 9.0/10

一个名为 ChainDrop 的自我传播蠕虫已入侵 npm 仓库超过 1300 个包，合计月下载量达 20 亿次，包括 Keyv、Cacheable 等热门缓存工具。攻击始于黑客攻破 Keyv 维护者的 GitHub 账号，并蔓延至 Deliveroo、Qlik 等机构的相关包；恶意版本通过正常的 GitHub Actions 流程发布。 鉴于受影响包的巨大下载量，这是一次关键且仍在持续的供应链攻击，可能影响全球数百万开发者和应用程序。该蠕虫能够窃取 GitHub、npm、AWS 等凭证，并通过感染其他维护者的包进行自我传播，从而引发一场难以遏制的连锁安全危机。 该恶意软件通过投放器 (`setup.mjs`) 和窃密脚本 (`Math_Symbol.js`) 在 `npm install` 期间自动执行。安全研究人员指出，由于中毒版本是通过受害者自己受信任的 CI/CD 管道发布的，因此具有加密合法性，这使得检测更加困难。攻击仍在扩散，域名 `npm-cache[.]com` 可作为失陷指标。

telegram · zaihuapd · Aug 5, 03:04

**背景**: npm 是 Node.js JavaScript 运行时的默认包管理器，托管着超过两百万个可复用代码包。针对 npm 的供应链攻击涉及入侵这些包以注入恶意代码，然后分发给下游用户和应用程序。GitHub Actions 是一个 CI/CD（持续集成/持续部署）平台，用于自动化软件工作流；配置错误或账户被入侵可能让攻击者滥用这些管道，为恶意代码披上合法的外衣进行发布。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.stepsecurity.io/blog/chaindrop-npm-worm">ChainDrop npm Worm: Bun-loaded CI/CD credential harvester with Ethereum dead-drop C2 - StepSecurity</a></li>
<li><a href="https://www.bleepingcomputer.com/news/security/massive-chaindrop-npm-supply-chain-attack-infects-hundreds-of-packages/">Massive ChainDrop npm supply-chain attack infects hundreds of packages</a></li>
<li><a href="https://thenextweb.com/news/chaindrop-npm-worm-shai-hulud-provenance-ai-tools">A worm tore through npm by making the malware look perfectly legitimate</a></li>

</ul>
</details>

**社区讨论**: 社区情绪表达了对依赖生态系统脆弱性的严重担忧。关键观点包括呼吁限制或取消包安装钩子，讨论因漏洞被即时利用而导致的清理困难，建议使用 Packj 等工具进行检测，请求用于扫描该蠕虫的 grep 命令，以及倡导使用开发容器（devcontainers）作为防护措施。

**标签**: `#security`, `#supply-chain-attack`, `#npm`, `#malware`, `#devops`

---

<a id="item-2"></a>
## [华为提出“韬定律”作为后摩尔时代新原则，以时间缩微替代几何缩微。](https://t.me/zaihuapd/42966) ⭐️ 8.0/10

在 2026 年于上海举行的国际电路与系统研讨会（ISCAS）上，华为提出了“韬定律”（Tau Scaling Law），主张以“时间缩微”（优化信号速度和延迟）作为半导体演进的新指导原则，以替代传统的“几何缩微”（缩小晶体管尺寸）。华为宣布过去六年已基于此理念设计并量产了 381 款芯片，并计划于今年秋季推出采用“逻辑折叠”（LogicFolding）架构的新款麒麟手机芯片。 这标志着半导体行业路线图的一次重大概念性转变，在传统摩尔定律缩放面临物理和经济极限之际，提供了一条潜在的替代路径。对于在获取尖端 EUV 光刻设备方面受限的华为而言，这种时域优化策略可能成为绕过几何缩微限制、持续提供有竞争力芯片性能的关键方法。 华为预计，到 2031 年，基于韬定律开发的高端芯片晶体管密度将达到相当于 1.4 纳米制程的水平。其实现技术“逻辑折叠”架构，通过将逻辑电路物理折叠并堆叠成双层三维结构，在器件、电路、芯片和系统多个层级进行协同优化。

telegram · zaihuapd · Aug 4, 08:04

**背景**: 摩尔定律是一个长期观察到的经验定律，指集成电路上可容纳的晶体管数量大约每两年翻一番，这主要通过“几何缩微”（即缩小晶体管尺寸）来实现。随着晶体管尺寸接近原子尺度，由于量子效应和制造挑战，进一步的几何缩微变得日益困难和昂贵。“时间缩微”则侧重于通过减小时间常数（τ）来提升性能，时间常数与信号传播速度和电路开关速度相关，而非单纯依赖缩小物理尺寸。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.huawei.com/en/news/2026/5/ieee-iscas-tau-scaling">HUAWEI Presents the Tau (τ) Scaling Law, Enabling ...</a></li>
<li><a href="https://globalsemiresearch.substack.com/p/huaweis-tau-scaling-law-a-technical">Huawei's Tau Scaling Law: A Technical Deep Dive Beyond the Hype</a></li>
<li><a href="https://www.tomshardware.com/tech-industry/semiconductors/huawei-claims-sanctions-busting-breakthrough-with-1-4nm-class-chips-by-2031-claims-55-percent-higher-transistor-density-firm-claims-new-logicfolding-chip-architecture-can-bypass-euv-restrictions-introduces-tau-scaling-law-to-replace-moores-law">Huawei claims sanctions-busting breakthrough with 1.4nm-class chips by 2031, claims 55% higher transistor density — firm claims new LogicFolding chip architecture can bypass EUV restrictions, introduces 'Tau Scaling Law' to replace Moore's Law | Tom's Hardware</a></li>

</ul>
</details>

**标签**: `#semiconductors`, `#hardware`, `#moores-law`, `#huawei`, `#chip-design`

---

<a id="item-3"></a>
## [谷歌联合华尔街为 Anthropic 搭建约 2000 亿美元 AI 芯片融资架构](https://www.ft.com/content/549f2e23-5aa2-49c7-9ea6-a9784ab7087c) ⭐️ 8.0/10

《金融时报》调查发现，谷歌已悄然搭建史上最大规模的基础设施融资架构之一，相关合同总额约 2000 亿美元，旨在支持向 Anthropic 交付价值超 1500 亿美元的 AI 芯片。今年 6 月，名为 Compute SPV 的特殊目的载体完成了首批交易，购入约 350 亿美元硬件，约合 1 吉瓦算力与 100 万颗 TPU。 这笔交易至关重要，因为它构建了一个庞大的表外融资机制，使得 AI 基础设施能够快速扩张，而无需任何单一公司承担其资产负债表压力。这展示了科技巨头如何与华尔街合作，为 AI 军备竞赛所需的巨额资本支出融资，并可能为未来大规模科技基础设施项目树立先例。 主要参与方包括：购买并协助融资芯片的博通；出资购买硬件后回租给 Anthropic 的阿波罗与黑石；以及摩根士丹利。谷歌则为数据中心提供担保。该融资模式借鉴了波音、通用电气等公司推销飞机和发动机时使用的厂商融资玩法。

telegram · zaihuapd · Aug 4, 10:52

**背景**: Anthropic 是一家以 AI 安全与研究闻名的公司，其旗舰产品是 Claude 系列大语言模型。TPU（张量处理单元）是谷歌专为神经网络机器学习开发的 AI 加速专用集成电路。特殊目的载体（SPV）是为特定、有限目的而设立的法律实体，在金融领域常被用来隔离财务风险。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Anthropic">Anthropic - Wikipedia</a></li>
<li><a href="https://jonathan-hui.medium.com/ai-chips-tpu-3fa0b2451a2d">AI Chips: Google TPU . Google’s chip designers argue that the | Medium</a></li>
<li><a href="https://www.investopedia.com/terms/s/spv.asp">investopedia.com/terms/s/ spv .asp</a></li>

</ul>
</details>

**标签**: `#AI Infrastructure`, `#Corporate Finance`, `#Semiconductors`, `#Anthropic`, `#Google`

---

<a id="item-4"></a>
## [美国联邦通信委员会禁止进口新款中国产人形机器人、四足机器人和联网电力逆变器](https://t.me/zaihuapd/42970) ⭐️ 8.0/10

美国联邦通信委员会于 7 月 28 日公布措施，禁止进口来自中国的新款人形机器人、四足机器人和联网电力逆变器。该禁令自发布起生效，仅适用于尚未推出的型号。 此举是美国为保护其技术供应链、防范与中国制造的先进机器人和能源设备相关的网络安全及数据安全风险而采取的重大升级措施。它将直接影响优必选、宇树科技等中国制造商，并可能重塑美国市场人形机器人和工业机器人的竞争格局。 该禁令明确针对“新款”型号，这意味着已获准销售的现有产品可能不受影响，但 FCC 保留撤销其授权的权力。预计该命令将对许多非中国供应商提供豁免，表明这是一种有针对性的措施，而非对所有外国机器人的全面禁止。

telegram · zaihuapd · Aug 4, 11:29

**背景**: 美国联邦通信委员会（FCC）是负责监管美国州际和国际通信的政府机构。近年来，其职责已扩展到包括授权射频设备以及应对联网设备中的网络安全威胁。人形和四足机器人是能在人类环境中执行任务的先进移动机器，它们通常依赖网络连接进行操作和更新，这引发了数据安全担忧。联网电力逆变器是太阳能和可再生能源系统中的关键部件，负责将直流电转换为交流电；它们接入电网后，可能成为网络攻击的目标，从而导致电力供应中断。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://easternherald.com/2026/07/30/trump-bans-chinese-humanoid-robots-china-retaliation/">Trump Bans Chinese Humanoid Robots as FCC Targets Unitree</a></li>
<li><a href="https://arxiv.org/html/2509.14096v1">The Cybersecurity of a Humanoid Robot An Early Study on the Cybersecurity of Humanoid Robots via the Unitree G1 Technical Report</a></li>
<li><a href="https://www.energy.gov/eere/solar/solar-cybersecurity-basics">Solar Cybersecurity Basics | Department of Energy</a></li>

</ul>
</details>

**标签**: `#geopolitics`, `#robotics`, `#trade-policy`, `#cybersecurity`, `#supply-chain`

---

<a id="item-5"></a>
## [我国首部 L3/L4 自动驾驶强制性国标报批，将于 2027 年实施](https://t.me/zaihuapd/42972) ⭐️ 8.0/10

中国工业和信息化部已完成《智能网联汽车自动驾驶系统安全要求》强制性国家标准的报批稿，并于 6 月 17 日起公示。这是中国首部针对 L3 和 L4 级自动驾驶的强制性标准，引入了安全档案（Safety Case）机制，建议于 2027 年 7 月 1 日实施。 该标准标志着中国对自动驾驶的监管从“概念松绑”转向“安全硬约束”，为高级别自动驾驶的商业化落地建立了明确的法律与技术框架。它将强制要求车企和技术开发商系统性论证其安全性，从而推动 L3 和 L4 级自动驾驶汽车在公共道路上更负责任地部署。 该标准强制要求采用安全档案（Safety Case）机制，企业需通过“声明—论据—证据”的体系来系统性论证安全性。同时，它对 L3 级系统的人机交接和 L4 级系统的自主风险处置分别提出了具体要求。

telegram · zaihuapd · Aug 4, 13:06

**背景**: SAE（国际汽车工程师学会）将驾驶自动化分为 L0 至 L5 六个等级。L3 级（有条件自动驾驶）能在特定条件下执行所有驾驶任务，但需要驾驶员在系统请求时接管。L4 级（高度自动驾驶）在其设计运行范围内可完成所有驾驶任务，无需人类干预。安全档案（Safety Case）是一种结构化的论证，由证据支持，旨在证明一个系统在特定运行环境下对于特定应用是足够安全的。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://torc.ai/understanding-the-levels-of-autonomy-3-4-5/">What Are The Levels of Autonomy? L3-L4 - Torc Robotics</a></li>
<li><a href="https://www.caranddriver.com/news/a36364986/sae-updates-refines-autonomous-driving-levels-chart/">SAE Updates, Refines Official Names for 'Autonomous Driving' Levels</a></li>
<li><a href="https://fiveable.me/autonomous-vehicle-systems/unit-11/handover-autonomous-manual-control/study-guide/ZSQikR09ZyMPGqeF">Handover between autonomous and manual control | Fiveable</a></li>

</ul>
</details>

**标签**: `#autonomous-driving`, `#regulation`, `#safety-standards`, `#smart-transportation`

---

<a id="item-6"></a>
## [3D 打印仿生海绵体植入干细胞，成功在猪模型中恢复勃起功能。](https://doi.org/10.1016/j.biomaterials.2026.124491) ⭐️ 8.0/10

研究人员成功利用 3D 打印技术制造出具有类似海绵体血管腔隙的仿生结构，并种植了脐带来源的间充质干细胞（MSCs），在猪模型中恢复了勃起功能。该研究通过单细胞测序揭示了其作用机制：干细胞促进内皮细胞分化以重建血管网络，减少 TGF-β分泌以抑制内皮-间质转化，同时调节免疫环境、激活抗炎因子。 这是勃起功能障碍（ED）再生医学领域的一项重大突破，超越了传统的症状缓解，旨在实现受损组织的结构性修复。如果未来能成功应用于人类，将为这一困扰众多男性、现有疗法常显不足的疾病提供一种全新的、可能具有治愈潜力的治疗方案。 该 3D 打印支架模拟了海绵体天然的血管腔隙结构，植入的间充质干细胞能加速凝胶基质降解以促进组织融合。然而，从猪模型到人类临床应用仍需更多研究，且个体差异可能影响最终的治疗效果。

telegram · zaihuapd · Aug 4, 13:52

**背景**: 海绵体是阴茎内两条可扩张的圆柱状勃起组织，在性兴奋时会充血从而产生勃起。勃起功能障碍（ED）常由该组织内的血管或神经系统损伤引起。间充质干细胞（MSCs）是一种成体干细胞，具有多向分化潜能、免疫调节能力和促进组织再生的特性，因此在组织工程领域应用前景广阔。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Corpus_cavernosum_penis">Corpus cavernosum penis - Wikipedia</a></li>
<li><a href="https://my.clevelandclinic.org/health/body/22511-corpus-cavernosum">Penis Corpus Cavernosum: Function, Anatomy & Conditions</a></li>
<li><a href="https://html.rhhz.net/QLGYDXXB/html/7e3f0d70-c510-4a8b-ae5d-16897f85b2c7.htm">干 细 胞 在美容行业中的 应 用 现状及展望</a></li>

</ul>
</details>

**标签**: `#3D Bioprinting`, `#Regenerative Medicine`, `#Tissue Engineering`, `#Stem Cells`, `#Medical Devices`

---

<a id="item-7"></a>
## [DeepSeek 重启第二轮融资，投前估值达 5000 亿元](https://finance.sina.com.cn/wm/2026-08-05/doc-inimfmyv1554159.shtml) ⭐️ 8.0/10

据报道，DeepSeek 已重启第二轮融资，计划募资 500 亿元人民币，投前估值约 5000 亿元，预计 8 月下旬完成签约。本轮融资曾在 7 月底暂停，据称是因创始人梁文锋对网上流传的疑似泄露的“面向投资者的会议实录”言论不满。 此次大规模融资若顺利完成，将使 DeepSeek 在短短几个月内总募资额超 1000 亿元人民币，这显示出投资者极强的信心，并使其成为全球 AI 竞赛中一个资金雄厚的主要竞争者。其估值较 6 月完成的首轮融资提升约 43%，突显了 AI 行业的高风险、快节奏特性以及市场对 DeepSeek 技术潜力的认可。 本轮融资至少在 7 月中旬就已开启，后于 7 月底暂停，投资方希望融资重启后能低调进行。部分此前积极接触的机构表示尚未接到重启消息，表明相关通道可能仍处于暂缓状态。

telegram · zaihuapd · Aug 5, 02:46

**背景**: DeepSeek（深度求索）是一家中国人工智能公司，由量化对冲基金幻方量化联合创始人梁文锋于 2023 年 7 月创立。该公司于 2025 年 1 月发布了 DeepSeek-R1 大语言模型及配套聊天机器人应用，从而在国际上崭露头角。“投前估值”指的是公司在获得新投资资金之前的估计价值，是风险投资融资轮次中的一个关键指标。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/DeepSeek">DeepSeek - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Liang_Wenfeng">Liang Wenfeng - Wikipedia</a></li>

</ul>
</details>

**标签**: `#AI`, `#Funding`, `#Valuation`, `#DeepSeek`, `#Business`

---