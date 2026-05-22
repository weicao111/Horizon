---
layout: default
title: "Horizon Summary: 2026-05-22 (EN)"
date: 2026-05-22
lang: en
---

> From 29 items, 6 important content pieces were selected

---

1. [AI GPU demand for HBM memory drives up costs for consumer device RAM.](#item-1) ⭐️ 8.0/10
2. [Cleve Moler, creator of MATLAB and pioneer in numerical computing, has died.](#item-2) ⭐️ 8.0/10
3. [Freenet Redesigned as a Decentralized Key-Value Store with WebAssembly Contracts](#item-3) ⭐️ 8.0/10
4. [Eli Lilly's Retatrutide Achieves 28.3% Average Weight Loss in Phase 3 Obesity Trial](#item-4) ⭐️ 8.0/10
5. [ByteDance open-sources Lance, a 3B-parameter unified multimodal model for image/video understanding and generation.](#item-5) ⭐️ 8.0/10
6. [Chinese regulators launch crackdown on unlicensed cross-border securities platforms, targeting Tiger Brokers and Futu.](#item-6) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [AI GPU demand for HBM memory drives up costs for consumer device RAM.](https://davidoks.blog/p/ai-is-killing-the-cheap-smartphone) ⭐️ 8.0/10

A detailed analysis explains that the surging demand for High Bandwidth Memory (HBM) used in AI training GPUs is diverting advanced semiconductor manufacturing capacity, which in turn is increasing the production costs and market prices for DDR and LPDDR memory used in smartphones and laptops. This supply chain shift directly impacts consumer electronics affordability, potentially leading to higher prices for smartphones and laptops as manufacturers pass on memory cost increases. It highlights how the explosive growth in AI infrastructure can have tangible, inflationary effects on broader technology markets. The article notes that building a state-of-the-art DRAM fabrication facility costs $15-20 billion, and it takes years for a new fab to achieve acceptable production yields. The technical complexity and high capital intensity of memory manufacturing limit how quickly supply can respond to sudden demand shifts between different memory types like HBM and DDR.

hackernews · d0ks · May 21, 21:55 · [Discussion](https://news.ycombinator.com/item?id=48229319)

**Background**: High Bandwidth Memory (HBM) is a specialized type of DRAM designed for high-performance computing. It stacks multiple memory dies vertically and uses a very wide data bus to achieve much higher bandwidth and lower power consumption compared to traditional DDR (Double Data Rate) memory, which is mounted flat on circuit boards. LPDDR (Low-Power DDR) is a variant optimized for mobile devices where power efficiency is critical. AI training GPUs, like NVIDIA's H200, require massive amounts of fast memory bandwidth, making HBM their preferred choice, whereas consumer devices like laptops and phones primarily use DDR and LPDDR.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/High_Bandwidth_Memory">High Bandwidth Memory - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/LPDDR">LPDDR - Wikipedia</a></li>
<li><a href="https://www.nvidia.com/en-us/data-center/h200/">H200 GPU | NVIDIA</a></li>

</ul>
</details>

**Discussion**: Commenters found the article to be a fascinating, deep explanation of the memory market dynamics, with one noting the headline undersold its value. A key discussion point questioned whether the trend toward higher RAM consumption in phones is inevitable, suggesting that software optimization and older algorithms could allow for devices with less memory, potentially mitigating cost pressures.

**Tags**: `#semiconductors`, `#hardware`, `#economics`, `#supply-chain`, `#ai-hardware`

---

<a id="item-2"></a>
## [Cleve Moler, creator of MATLAB and pioneer in numerical computing, has died.](https://www.mathworks.com/company/aboutus/founders/clevemoler.html) ⭐️ 8.0/10

Cleve Moler, the mathematician and computer scientist who created the MATLAB programming language and environment, has passed away. He originally developed MATLAB in the late 1970s as a teaching tool to provide interactive access to matrix software libraries without requiring students to compile FORTRAN code. Moler's creation, MATLAB, became a foundational tool for scientific computing, engineering education, and research for decades, directly influencing millions of engineers and scientists. Its design philosophy and success also inspired the development of major open-source scientific computing ecosystems like SciPy/NumPy, which underpin modern data science and AI. The original version of MATLAB, known as MATrix LABoratory, was written in FORTRAN and comprised about 2000 lines of code. While MATLAB itself evolved into a commercial product, its core concepts of interactive matrix manipulation and numerical algorithm accessibility became a model for subsequent tools.

hackernews · mychele · May 22, 02:35 · [Discussion](https://news.ycombinator.com/item?id=48231319)

**Background**: Numerical computing involves using algorithms to solve mathematical problems with numerical approximations, which is essential in engineering, physical sciences, and data analysis. MATLAB is a high-level language and interactive environment specifically designed for numerical computation, matrix manipulations, and algorithm implementation. Its creation stemmed from Moler's work on canonical FORTRAN libraries for numerical linear algebra and his desire to make these tools more accessible for teaching.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Numerical_computing">Numerical computing</a></li>
<li><a href="https://en.wikipedia.org/wiki/MATLAB">MATLAB - Wikipedia</a></li>
<li><a href="https://www.mathworks.com/company/technical-articles/a-brief-history-of-matlab.html">A Brief History of MATLAB - MATLAB & Simulink</a></li>

</ul>
</details>

**Discussion**: The community expresses deep respect and gratitude, highlighting Moler's foundational role in numerical methods and the creation of essential FORTRAN libraries. Commenters note MATLAB's profound impact on engineering education and its role as a direct inspiration for the open-source data science stack (NumPy, SciPy). Many share personal stories of how MATLAB introduced them to programming and was an indispensable tool in their studies and careers.

**Tags**: `#obituary`, `#numerical-computing`, `#matlab`, `#scientific-computing`, `#history`

---

<a id="item-3"></a>
## [Freenet Redesigned as a Decentralized Key-Value Store with WebAssembly Contracts](https://freenet.org/) ⭐️ 8.0/10

The original creator of Freenet has released a ground-up redesign of the project, now architecturally a global, decentralized key-value store where keys are WebAssembly contracts that define and manage state. The new platform has been operational since December 2024 and already hosts applications like River (decentralized chat) and Delta (decentralized CMS). This redesign represents a significant evolution for a foundational peer-to-peer project, shifting it from a file-sharing network to a programmable platform for decentralized applications (dApps). By using WebAssembly contracts to enforce state consistency through commutative merge operations, it offers a novel architecture for building censorship-resistant, serverless web applications that run directly in browsers. A core technical innovation is the requirement for each contract to define a commutative merge operation for its state, allowing updates to propagate 'like a virus' and achieve global consistency in seconds. Applications are downloaded from the network and run in a web browser, connecting locally to the Freenet peer via WebSocket instead of remote data centers; however, mobile installers are not yet available.

hackernews · sanity · May 21, 14:34 · [Discussion](https://news.ycombinator.com/item?id=48223362)

**Background**: Freenet, originally launched in the early 2000s, is a peer-to-peer platform designed for censorship-resistant communication and publishing. In mid-2023, the original codebase was renamed to Hyphanet, while this new 'Freenet' represents a separate, ground-up rewrite. A decentralized key-value store is a non-relational database that maps unique keys to values and is a fundamental building block for scalable, fault-tolerant distributed systems like Amazon DynamoDB.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Hyphanet">Hyphanet - Wikipedia</a></li>
<li><a href="https://dev.to/josephakayesi/design-a-distributed-key-value-store-2f">Design a Distributed Key-Value Store - DEV Community</a></li>

</ul>
</details>

**Discussion**: The discussion revealed significant controversy regarding the project's governance, with one comment alleging the redesign was a 'backroom decision' that discarded the original team's work. Technical concerns were raised about the practicality of the state-merge model for complex applications like voting systems, and questions were asked about limitations such as bootstrapping, latency, disk usage, and how naming/anonymity would be handled.

**Tags**: `#decentralization`, `#peer-to-peer`, `#webassembly`, `#distributed-systems`

---

<a id="item-4"></a>
## [Eli Lilly's Retatrutide Achieves 28.3% Average Weight Loss in Phase 3 Obesity Trial](https://www.prnewswire.com/news-releases/lillys-triple-agonist-retatrutide-delivered-powerful-weight-loss-in-pivotal-phase-3-obesity-trial-302778859.html) ⭐️ 8.0/10

Eli Lilly announced that its triple-agonist drug retatrutide met all primary and key secondary endpoints in the pivotal Phase 3 TRIUMPH-1 trial for obesity, with the highest dose (12 mg) achieving an average weight loss of 28.3% over 80 weeks. Additionally, 45.3% of participants in that group lost at least 30% of their body weight. This result represents a significant leap in efficacy for pharmacological obesity treatments, potentially setting a new benchmark for weight loss drugs and intensifying competition in the lucrative GLP-1 and multi-agonist market. The substantial weight reduction could translate into improved health outcomes for millions of people with obesity and related comorbidities. The trial enrolled approximately 2,500 adults with obesity or overweight and at least one weight-related comorbidity. The most common side effects were gastrointestinal, and the company reported no observed heart or liver safety issues, with a discontinuation rate due to adverse events (4.1%) lower than the placebo group (4.9%).

telegram · zaihuapd · May 22, 02:18

**Background**: Retatrutide is a novel 'triple agonist' that simultaneously activates three hormone receptors: GIP, GLP-1, and glucagon. This multi-target approach is designed to enhance metabolic effects like appetite suppression and energy expenditure beyond what single or dual agonists (like semaglutide or tirzepatide) can achieve. The TRIUMPH clinical program is evaluating retatrutide specifically for chronic weight management in adults with obesity or overweight.

<details><summary>References</summary>
<ul>
<li><a href="https://www.retatrutide.med/knowledge-base/mechanism-of-action">Mechanism of Action : How Retatrutide 's Triple Receptor Agonism...</a></li>
<li><a href="https://medical.lilly.com/us/products/answers/what-retatrutide-clinical-trials-are-being-conducted-in-people-with-obesity-or-overweight-229656">What retatrutide clinical trials are being conducted in people with...</a></li>
<li><a href="https://www.fiercebiotech.com/biotech/eli-lillys-triple-g-drug-drives-deep-weight-loss-phase-3-obesity-trial">Lilly’s triple-G drug drives deep weight loss in phase 3 trial</a></li>

</ul>
</details>

**Tags**: `#pharmaceuticals`, `#clinical-trials`, `#obesity-treatment`, `#biotechnology`

---

<a id="item-5"></a>
## [ByteDance open-sources Lance, a 3B-parameter unified multimodal model for image/video understanding and generation.](https://mp.weixin.qq.com/s/Xbfq72cr1796RZxJIs3L1A) ⭐️ 8.0/10

ByteDance has open-sourced Lance, a lightweight 3-billion-parameter multimodal model that natively unifies image/video understanding and generation tasks within a single architecture. The model, released under the Apache 2.0 license, is now available on Hugging Face and reportedly achieves leading results on benchmarks like GenEval for image generation and VBench for video generation. This release is significant because it provides a relatively small-scale, unified model that can perform both understanding and generation across images and video, making advanced multimodal AI more accessible and efficient. The permissive Apache 2.0 license and availability on a major platform like Hugging Face lower the barrier to entry for researchers and developers, potentially accelerating innovation in applications like content creation and interactive AI. Lance employs a shared context and dual-stream expert architecture, using separate encoders (Qwen2.5-VL for understanding and Wan2.2 for generation) for different tasks while facilitating information exchange. It also utilizes modality-aware positional encoding to address sequence boundary confusion, a technical detail crucial for handling mixed input and output modalities within a unified framework.

telegram · zaihuapd · May 22, 06:40

**Background**: Unified Multimodal Models (UMMs) are a growing trend in AI that aim to integrate multiple modalities like images, text, and video within a single architecture to jointly perform reasoning and generative tasks. These models often use specialized architectures, such as dual-stream designs, to maintain separate processing paths for different types of data while enabling cross-modal interaction. The goal is to move beyond separate, task-specific models towards more general and efficient AI systems capable of diverse multimodal functions.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/AIDC-AI/Awesome-Unified-Multimodal-Models">Awesome Unified Multimodal Models - GitHub</a></li>
<li><a href="https://www.emergentmind.com/topics/unified-multimodal-models-umms">Unified Multimodal Models (UMMs) Overview - emergentmind.com</a></li>
<li><a href="https://www.emergentmind.com/topics/dual-stream-context-architecture-0b723934-4838-4e1a-9555-1cfb22d8863f">Dual-Stream Context Architecture</a></li>

</ul>
</details>

**Tags**: `#multimodal-ai`, `#computer-vision`, `#open-source`, `#generative-ai`, `#video-generation`

---

<a id="item-6"></a>
## [Chinese regulators launch crackdown on unlicensed cross-border securities platforms, targeting Tiger Brokers and Futu.](https://mp.weixin.qq.com/s?__biz=MzA4NzAzMDgwMw==&amp;mid=2651090403&amp;idx=3&amp;sn=bca72a940ac72bef356f29b5b9576ac1&amp;chksm=8a1670281e2bc67d2df3608a313ba9fdaf0fcd2f43ce44475c6bf273b386af2e4f9d8e8e2e2b&amp;scene=0&amp;xtrack=1) ⭐️ 8.0/10

Eight Chinese regulatory bodies, including the China Securities Regulatory Commission (CSRC), have issued a two-year rectification plan to crack down on unlicensed cross-border securities, futures, and fund businesses. The plan explicitly forbids unapproved overseas institutions from soliciting clients, opening accounts, transmitting trading orders, or transferring funds within China, and it mandates that existing investors can only sell their positions and withdraw funds during this period. This crackdown represents a major enforcement action that will fundamentally reshape the landscape for retail investors in China seeking to access overseas markets, forcing popular fintech platforms like Tiger Brokers and Futu to wind down their mainland operations. It underscores the Chinese government's tightening control over cross-border capital flows and its push to channel investments through official, regulated channels like Stock Connect and QDII. The CSRC has already filed investigations and issued preliminary administrative penalty notices against Tiger Brokers, Futu, and Longbridge, with plans to confiscate all illegal gains and impose severe penalties. The platforms are accused of operating without approval for securities brokerage, margin financing, public fund sales, and futures brokerage businesses in China.

telegram · zaihuapd · May 22, 08:26

**Background**: Cross-border securities platforms like Tiger Brokers and Futu have historically allowed mainland Chinese investors to trade stocks listed in markets like the US and Hong Kong. In China, cross-border securities business requires specific regulatory approvals. The government has established official channels for outward investment, such as the Qualified Domestic Institutional Investor (QDII) scheme, which allows licensed domestic institutions to invest overseas, and the Cross-boundary Wealth Management Connect (WMC) in the Greater Bay Area, which facilitates personal cross-border investment between mainland China, Hong Kong, and Macau.

<details><summary>References</summary>
<ul>
<li><a href="https://zh.wikipedia.org/zh-sg/跨境理财通">跨境理财通 - 维基百科，自由的百科全书</a></li>
<li><a href="https://www.hkma.gov.hk/gb_chi/key-functions/international-financial-centre/wealth-management-connect/">香港金融管理局 - 粤港澳大湾区跨境理财通</a></li>

</ul>
</details>

**Tags**: `#Financial Regulation`, `#Fintech`, `#Cross-Border Investment`, `#Securities Law`, `#China Tech`

---