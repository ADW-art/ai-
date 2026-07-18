---
layout: default
title: "Horizon Summary: 2026-07-18 (ZH)"
date: 2026-07-18
lang: zh
---

> 从 67 条内容中筛选出 5 条重要资讯。

---

1. [GPT-5.6 Sol Pro 帮助填补凸优化 30 年空白](#item-1) ⭐️ 8.0/10
2. [AWS 计费单位错误导致账单飙升至数万亿美元](#item-2) ⭐️ 8.0/10
3. [微软警告针对企业客户的 ACR Stealer 攻击激增](#item-3) ⭐️ 7.0/10
4. [Mesa 26.2 提升 NVK Vulkan 性能](#item-4) ⭐️ 7.0/10
5. [AI 会改善还是恶化预授权流程？](#item-5) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [GPT-5.6 Sol Pro 帮助填补凸优化 30 年空白](https://old.reddit.com/r/math/comments/1uxj3cy/after_openais_cdc_proof_announcement_gpt56_used_a/) ⭐️ 8.0/10

OpenAI 最新模型的一个变体 GPT-5.6 Sol Pro 被用于证明一个在凸优化领域悬而未决 30 年的猜想。该结果在 Reddit 上分享，引发了关于 AI 在数学研究中作用的讨论。 这表明大型语言模型能够为真正的数学进展做出贡献，可能加速优化及相关领域的研究。同时也引发了关于人类数学家未来角色以及数学发现本质的讨论。 该猜想涉及在球形域上对 Lipschitz 函数求解凸优化问题的时间复杂度。证明使用的是专为复杂推理任务设计的 GPT-5.6 Sol Pro，而非更强大的 Ultra 变体。

hackernews · mbustamanter · 7月18日 13:00 · [社区讨论](https://news.ycombinator.com/item?id=48957779)

**背景**: 凸优化是数学优化的一个子领域，研究在凸集上最小化凸函数的问题。它在机器学习、工程、经济学和运筹学中有广泛应用。该猜想涉及找到近似解所需的最坏情况迭代次数，这是复杂性理论中的一个基本问题。30 年的空白表明先前的方法无法建立紧界。GPT-5.6 Sol Pro 是 OpenAI GPT-5.6 模型的高能力版本，针对困难任务和长时间工作流进行了优化。该模型进行数学推理和生成证明的能力表明了一种 AI 辅助研究的新范式。然而，该结果在凸优化领域被认为是小众的，且证明可能依赖于仔细的人工引导。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/index/gpt-5-6/">GPT-5.6: Frontier intelligence that scales with your ambition | OpenAI</a></li>
<li><a href="https://help.openai.com/en/articles/20001325-a-preview-of-gpt-56-sol-terra-and-luna">GPT-5.6 in ChatGPT | OpenAI Help Center</a></li>
<li><a href="https://en.wikipedia.org/wiki/Convex_optimization">Convex optimization - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: Reddit 社区既表达了兴奋也表达了谨慎。一些用户指出该猜想虽小众但确实是真正的贡献，而另一些用户则争论 AI 是否会让初级研究人员过时。还有人对 Sol Pro 和 Ultra 之间的区别感到好奇，猜测 Sol Pro 使用了多智能体编排。

**标签**: `#AI`, `#mathematics`, `#convex optimization`, `#LLM`, `#research`

---

<a id="item-2"></a>
## [AWS 计费单位错误导致账单飙升至数万亿美元](https://www.solidot.org/story?sid=84859) ⭐️ 8.0/10

2025 年 7 月 17 日，AWS 计费系统出现单位错误，由于 GB 与 Byte 的转换错误，全球客户看到从数百万到数万亿美元不等的预估费用。亚马逊确认了该问题并暂停了账单更新，预计在 7 月 19 日前完全恢复。 此事件凸显了 AWS 计费基础设施的严重故障，动摇了客户信任并引发广泛恐慌。它强调了在金融系统中进行严格单元测试的重要性，尤其是对于占主导地位的云服务提供商。 该错误源于预估计费计算子系统中的单位定价问题，可能将 GB 误解释为字节，导致费用膨胀了 1,073,741,824 倍。亚马逊表示实际使用量和费用未受影响，问题仅限于预估账单显示。

rss · Solidot · 7月18日 04:28

**背景**: AWS 是全球最大的云计算平台，服务数百万客户。其计费系统跟踪众多服务的使用情况，并根据消费生成预估费用。单位转换错误发生在系统错误解释测量单位时，例如将千兆字节视为字节。由于 1 GB 等于 1,073,741,824 字节，此类错误可使费用膨胀超过十亿倍。这类错误在自动化计费系统中尤其危险，因为它能在不被立即察觉的情况下产生天文数字。该事件最初由用户在社交媒体和论坛上报告，促使 AWS 调查并确认问题。其他系统也曾发生过类似的单位错误，但由于 AWS 庞大的客户群，此次规模前所未有。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thenextweb.com/news/aws-billing-bug-billion-dollar-estimates">An AWS billing bug sent users estimated charges of up to $2.5 trillion</a></li>
<li><a href="https://tech.yahoo.com/computing/articles/amazon-corrects-aws-billing-error-173026819.html">Amazon Corrects AWS Billing Error Behind Billion-Dollar Invoices</a></li>
<li><a href="https://www.wired.com/story/amazon-web-services-glitch-oh-no/">AWS Billing Glitch Hits Customers With Billion-Dollar Fees | WIRED</a></li>

</ul>
</details>

**社区讨论**: 输入中未提供社区评论。但根据网络搜索结果，Reddit 用户表达了震惊和幽默，一位用户指出其每月 0.19 美元的账单飙升至 25 亿美元。情绪混合了恐慌和调侃，部分用户质疑 AWS 的测试流程。

**标签**: `#AWS`, `#billing`, `#cloud computing`, `#incident`, `#unit error`

---

<a id="item-3"></a>
## [微软警告针对企业客户的 ACR Stealer 攻击激增](https://www.bleepingcomputer.com/news/security/microsoft-warns-of-surge-in-acr-stealer-attacks-on-customers/) ⭐️ 7.0/10

微软观察到使用 ACR Stealer 恶意软件的攻击显著增加，该恶意软件针对企业客户，窃取浏览器存储的密码、身份验证令牌和敏感文档。 这一激增凸显了信息窃取恶意软件日益增长的威胁，它通过窃取身份验证令牌可以绕过多因素认证（MFA），对企业安全构成严重风险。 ACR Stealer 是一种恶意软件即服务（MaaS）产品，于 2024 年 3 月出现，由 Amatera Stealer 更名而来，在俄语网络犯罪论坛上出售。

rss · BleepingComputer · 7月18日 14:17

**背景**: 信息窃取恶意软件（infostealer）旨在从受感染设备中收集敏感数据，如凭证、财务信息和浏览器 cookies。ACR Stealer 是一个复杂的例子，能够窃取身份验证令牌，这些令牌可用于绕过 MFA，因为它们证明用户已经过身份验证。该恶意软件通过钓鱼活动和漏洞传播，通常针对企业环境。微软的警告来自其检测与响应团队（DART），该团队追踪此类威胁。随着更多组织采用 MFA，令牌窃取的增加是一个日益严重的问题。ACR Stealer 的 MaaS 模式使其对技术能力较弱的攻击者也可用，从而扩大了威胁范围。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.microsoft.com/en-us/security/blog/2026/07/16/acr-stealer-two-observed-intrusion-chains-amid-increased-threat-activity/">ACR Stealer: Two observed intrusion chains amid increased threat ...</a></li>
<li><a href="https://cybersecuritynews.com/acr-stealer-uncovering-attack-chains/">ACR Stealer - Uncovering Attack Chains, Functionalities And IOCs</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#malware`, `#enterprise security`, `#Microsoft`

---

<a id="item-4"></a>
## [Mesa 26.2 提升 NVK Vulkan 性能](https://www.phoronix.com/news/NVK-Mesa-26.2-Performance) ⭐️ 7.0/10

作为开源 Mesa 图形栈一部分的 NVK Vulkan 驱动程序，在 Mesa 26.2 版本中持续提升性能，缩小了与 NVIDIA 专有 Vulkan 驱动程序的差距。 这一进展对 Linux 游戏玩家和开源倡导者意义重大，因为它提供了 NVIDIA 专有驱动程序的可行开源替代方案，可能减少对闭源软件的依赖。 NVK 是 NVIDIA GPU 的符合 Vulkan 1.4 标准的实现，并通过 Zink 支持 OpenGL。性能提升来自 Mesa 26.2 功能版本中的持续优化。

rss · Phoronix \(Linux\) · 7月18日 19:57

**背景**: NVK 是 NVIDIA GPU 的开源 Vulkan 驱动程序，作为 Mesa 3D 图形库的一部分开发。它旨在提供 NVIDIA 专有 Vulkan 驱动程序的完全开源替代方案。该驱动程序一直在积极开发中，每个 Mesa 版本都带来性能改进和新功能。Mesa 26.2 延续了这一趋势，进一步缩小了性能差距。该驱动程序基于 Nouveau 内核驱动程序，这是 NVIDIA 硬件的开源驱动程序。NVK 的进展受到 Linux 游戏社区的密切关注，因为它直接影响在 Linux 上无需专有驱动程序即可运行基于 Vulkan 的游戏和应用程序的能力。此外，相关项目如 DXVK 和 D7VK（将 Direct3D 调用转换为 Vulkan）也受益于 NVK 的改进。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.mesa3d.org/drivers/nvk.html">NVK — The Mesa 3D Graphics Library latest documentation</a></li>
<li><a href="https://www.phoronix.com/search/NVK">NVK - Phoronix</a></li>
<li><a href="https://www.collabora.com/news-and-blog/blog/2022/03/23/how-to-write-vulkan-driver-in-2022/">How to write a Vulkan driver in 2022</a></li>

</ul>
</details>

**标签**: `#Vulkan`, `#Mesa`, `#NVIDIA`, `#Linux graphics`, `#open-source driver`

---

<a id="item-5"></a>
## [AI 会改善还是恶化预授权流程？](https://arstechnica.com/ai/2026/07/will-ai-fix-prior-authorization-or-make-it-worse/) ⭐️ 6.0/10

美国政府正在试点一个使用 AI 自动化保险覆盖决策的项目，旨在简化预授权流程。 预授权是医疗保健中的主要行政负担，常导致治疗延迟和医生倦怠；AI 可能缓解这些问题，但也可能引入偏见决策和缺乏透明度等新风险。 该试点项目仍处于早期阶段，关于 AI 模型、数据源和监督机制的细节尚未完全披露。批评者担心，如果没有适当的保障措施，AI 可能会复制现有覆盖决策中的偏见。

rss · Ars Technica · 7月18日 11:18

**背景**: 预授权是健康保险公司要求在医疗服务或处方被覆盖之前获得批准的过程。它旨在控制成本并确保适当的护理，但因导致延误和行政浪费而受到批评。AI 在医疗保健中的应用迅速增长，从诊断工具到行政自动化。然而，AI 系统可能从训练数据中继承偏见，并且可能缺乏可解释性，引发对公平性和问责制的担忧。该政府试点是通过技术现代化医疗行政的更广泛努力的一部分。其他国家也提出了类似倡议，但尚未大规模实施。该试点的结果可能影响未来的政策和行业实践。

**标签**: `#AI`, `#healthcare`, `#policy`, `#automation`

---



---

## 技术专题

好的，我们来聊聊 **WebAssembly（简称Wasm）**。它不是一个你每天都会直接“编写”的语言，而是一个正在悄然改变Web乃至整个计算领域的基础设施级技术。

---

### 1. 背景和定位：从“JavaScript的无奈”到“浏览器里的第二引擎”

**背景：** 长久以来，JavaScript是浏览器中唯一能运行的原生语言。这带来了巨大的便利，但也暴露了其根本性的局限：JavaScript作为一门动态类型、解释执行（或JIT编译）的语言，其性能天花板是清晰可见的。对于需要大量计算的任务，比如3D游戏、视频编辑、科学模拟、图像处理，JavaScript显得力不从心。开发者要么忍受性能瓶颈，要么被迫使用插件（如Flash、Java Applet），但这些插件有严重的安全和兼容性问题。

**定位：** WebAssembly应运而生。它的定位非常精准：**一个面向Web的、低级的、可移植的、高效的二进制指令格式**。它不是要取代JavaScript，而是要成为JavaScript的“搭档”，一个专门负责处理重计算任务的“第二引擎”。你可以把它想象成浏览器里的一个“高性能沙盒”，允许你用C/C++、Rust、Go等语言编写代码，然后编译成Wasm字节码，在浏览器中以接近原生的速度运行。

**关键点：** Wasm不是一个语言，而是一个**编译目标**。你写C++代码，然后把它编译成.wasm文件，浏览器就能直接运行这个文件。

### 2. 核心原理：一个精心设计的“虚拟CPU”

Wasm的核心原理可以概括为：**设计一个抽象的、安全的、高效的虚拟指令集架构，并让所有主流浏览器都实现这个架构的虚拟机。**

*   **二进制格式：** Wasm代码以紧凑的二进制格式（.wasm）存储。这比JavaScript源代码小得多，加载和解析速度极快。浏览器只需要下载这个二进制文件，就能直接开始执行，省去了JavaScript的解析和编译时间。
*   **线性内存：** Wasm模块拥有一个连续的、可增长的线性内存空间。这就像一个巨大的数组，所有的数据（如纹理、模型数据）都存放在这里。JavaScript可以通过API来读写这块内存，实现了两者之间的高效数据交换。
*   **类型系统：** Wasm只支持有限的几种数值类型：i32、i64、f32、f64（整数和浮点数）。没有对象、字符串、数组等高级类型。这简化了编译器的实现，并确保了性能的可预测性。
*   **栈式虚拟机：** Wasm指令集是基于栈的。所有操作都在一个隐式的操作数栈上进行。例如，`i32.add`指令会从栈顶弹出两个32位整数，相加后再把结果压回栈顶。这种设计简单、指令密度高，非常适合硬件模拟。
*   **安全沙箱：** Wasm运行在一个严格的沙箱中。它不能直接访问系统资源（如文件系统、网络、DOM）。所有对外部世界的访问都必须通过JavaScript的API（称为“导入”）进行。这保证了安全性，防止恶意Wasm代码破坏用户系统。
*   **模块与实例：** 一个.wasm文件是一个“模块”。当需要执行它时，需要创建一个“实例”。实例化过程会分配线性内存、初始化全局变量，并将JavaScript提供的函数“导入”到Wasm模块中。之后，就可以调用Wasm模块导出的函数了。

**一个简单的比喻：** 想象你有一个超级高效的“计算器”（Wasm），但计算器本身没有屏幕和键盘。你需要一个“操作员”（JavaScript）来告诉计算器要算什么（通过导入函数），计算器算完后，再把结果写在纸上（线性内存），操作员再去读取。两者分工明确，各司其职。

### 3. 应用场景：从“不可能”到“可能”

Wasm的应用场景主要集中在那些对性能、可移植性和安全性有极高要求的领域：

*   **高性能Web应用：** 这是最直接的应用。
    *   **图像/视频编辑：** 如Figma、Adobe Photoshop Web版，使用Wasm运行C++的图像处理库，实现毫秒级的滤镜、缩放等操作。
    *   **3D游戏与引擎：** Unity、Unreal Engine等游戏引擎都支持导出为Wasm，让AAA级游戏在浏览器中流畅运行。
    *   **科学计算与数据可视化：** 运行复杂的物理模拟、金融模型、基因组分析等，将计算密集型任务卸载到Wasm。
*   **云原生与边缘计算：** Wasm的轻量级、快速启动和沙箱特性，使其成为Serverless和边缘计算的理想运行时。
    *   **Serverless函数：** 可以用Rust或Go编写Wasm函数，启动时间仅为毫秒级，远快于容器。
    *   **CDN边缘计算：** 在CDN节点上运行Wasm代码，实现请求处理、A/B测试、图像优化等，无需启动完整虚拟机。
*   **跨平台应用：** 通过Wasm，你可以将C/C++/Rust编写的库或应用，编译后运行在任何支持Wasm的环境中（浏览器、Node.js、独立运行时如Wasmer、Wasmtime），实现“一次编写，到处运行”。
*   **区块链与智能合约：** 许多新一代区块链（如Polkadot、EOS）使用Wasm作为智能合约的执行引擎，因为它比EVM（以太坊虚拟机）更高效、更安全、更灵活。

### 4. 同类对比：Wasm vs. JavaScript vs. Native

| 特性 | WebAssembly (Wasm) | JavaScript | Native (如C++编译的exe) |
| :--- | :--- | :--- | :--- |
| **性能** | 接近原生 | 中等（JIT优化后） | 最高 |
| **启动速度** | 极快（二进制解析） | 较慢（解析+编译） | 快（直接执行） |
| **安全性** | 高（沙箱隔离） | 高（浏览器沙箱） | 低（直接访问系统） |
| **可移植性** | 高（浏览器+独立运行时） | 高（浏览器+Node.js） | 低（需为每个平台编译） |
| **开发效率** | 低（需用其他语言编写） | 高（动态、灵活） | 中（需管理内存等） |
| **适用场景** | 计算密集型、跨平台库 | 交互逻辑、UI、DOM操作 | 高性能系统、桌面应用 |

**总结对比：** JavaScript擅长处理UI和逻辑，Wasm擅长处理计算。Native性能最强但可移植性最差。Wasm在性能、安全、可移植性之间取得了绝佳的平衡。

### 5. 学习建议：从“使用者”到“创造者”

对于不同背景的开发者，学习路径不同：

*   **如果你是Web前端开发者（JavaScript为主）：**
    *   **第一步：理解概念。** 不需要立刻写Wasm，先理解它是什么、能做什么、不能做什么。
    *   **第二步：使用现成的Wasm库。** 尝试在项目中使用一些由Wasm驱动的库，比如`ffmpeg.wasm`（视频处理）、`tesseract.js`（OCR，部分基于Wasm）、`squoosh`（图像压缩）。感受Wasm带来的性能提升。
    *   **第三步：用Rust或AssemblyScript编写Wasm。** 推荐从**AssemblyScript**开始，它的语法类似TypeScript，学习曲线平缓。尝试写一个简单的函数（如计算斐波那契数列），编译成Wasm，然后在JavaScript中调用它，对比性能。
    *   **第四步：深入学习Rust + Wasm。** Rust是Wasm生态中最主流的语言，拥有强大的工具链（`wasm-pack`、`wasm-bindgen`）。学习如何将Rust库编译成Wasm，并与JavaScript交互。

*   **如果你是系统编程开发者（C/C++/Rust为主）：**
    *   **第一步：理解Wasm的局限性。** 熟悉Wasm的线性内存模型、缺少系统调用等限制。
    *   **第二步：使用Emscripten（C/C++）或wasm-pack（Rust）。** 尝试将一个现有的C/C++库（如libjpeg、zlib）编译成Wasm，并在Node.js或浏览器中测试。
    *   **第三步：探索WASI。** 学习WebAssembly System Interface（WASI），它允许Wasm在浏览器之外访问文件系统、网络等系统资源，是Wasm在服务端和边缘计算应用的关键。
    *   **第四步：关注前沿。** 关注Wasm的GC（垃圾回收）、异常处理、多线程等提案的进展，这些将极大扩展Wasm的能力。

**一句话总结：** 不要试图用Wasm去写整个应用，而是把它当作一个高性能的“加速器”，用它来解决你最棘手的性能瓶颈。从一个小功能开始，体验“编译一次，到处飞”的乐趣。