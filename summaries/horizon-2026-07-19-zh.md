# Horizon 每日速递 - 2026-07-19

> 从 67 条内容中筛选出 12 条重要资讯。

---

1. [WordPress 核心 &\#x27;wp2shell&\#x27; RCE 漏洞遭公开利用](#item-1) ⭐️ 9.0/10
2. [Kimi K3：中国 AI 模型通过蒸馏逼近前沿水平](#item-2) ⭐️ 8.0/10
3. [GPT-5.6 Sol 解决 30 年凸优化猜想](#item-3) ⭐️ 8.0/10
4. [AI 狂热正在摧毁全球决策](#item-4) ⭐️ 8.0/10
5. [7-Zip 26.02 修复压缩包远程代码执行漏洞](#item-5) ⭐️ 8.0/10
6. [上下文炸弹：新型防御技术瘫痪 AI 黑客代理](#item-6) ⭐️ 8.0/10
7. [Claude Code 改用 Rust 版 Bun，启动速度提升 10%](#item-7) ⭐️ 7.0/10
8. [交互式 SQLite 查询解释器通过 Pyodide 在浏览器中运行](#item-8) ⭐️ 7.0/10
9. [微软警告 ACR 窃密软件攻击激增](#item-9) ⭐️ 7.0/10
10. [D7VK 2.0 发布，性能提升高达两倍](#item-10) ⭐️ 7.0/10
11. [邻近岩石超级地球 GJ3378b 确认位于宜居带](#item-11) ⭐️ 7.0/10
12. [经期追踪应用向第三方共享敏感数据](#item-12) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [WordPress 核心 &\#x27;wp2shell&\#x27; RCE 漏洞遭公开利用](https://www.bleepingcomputer.com/news/security/wordpress-core-wp2shell-rce-flaws-get-public-exploits-patch-now/) ⭐️ 9.0/10

针对 WordPress 核心的严重远程代码执行漏洞（统称为 &\#x27;wp2shell&\#x27;，包括 CVE-2026-63030 和 CVE-2026-60137）的公开利用代码已发布。这些利用代码允许未经身份验证的攻击者执行任意 SQL 查询，并在易受攻击的 WordPress 安装上实现远程代码执行。 WordPress 驱动着超过 40% 的网站，这使得该漏洞具有极高影响，可能导致大规模网站被接管。管理员必须立即修补以防止被利用。 该漏洞是 WordPress REST API \`/wp-json/batch/v1\` 端点中的未经身份验证的 SQL 注入，通过 REST 批量路由混淆链式实现远程代码执行。截至 2026 年 7 月 18 日，尚未公开报告大规模利用，但公开利用代码的发布增加了风险。

rss · BleepingComputer · 7月18日 17:22

**背景**: WordPress 是全球最流行的内容管理系统（CMS），被数百万网站使用。远程代码执行（RCE）漏洞是最严重的漏洞之一，因为它允许攻击者在服务器上运行任意命令。SQL 注入是一种攻击类型，将恶意 SQL 语句插入输入字段以执行。&\#x27;wp2shell&\#x27; 漏洞专门针对 REST API 的批量端点，该端点旨在高效处理多个请求。该利用无需身份验证，因此特别危险。WordPress 已发布安全补丁来解决这些漏洞；管理员应立即更新到最新版本。这些漏洞由安全研究人员发现，并已分配 CVE 编号进行跟踪。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/NULL200OK/WP2Shell">GitHub - NULL200OK/WP2Shell: WP2Shell - CVE-2026-63030 / CVE-2026-60137 ...</a></li>
<li><a href="https://github.com/Icex0/wp2shell-poc">GitHub - Icex0/wp2shell-poc: wp2shell (CVE-2026-63030 &amp; CVE-2026-60137 ...</a></li>
<li><a href="https://www.bleepingcomputer.com/news/security/wordpress-core-wp2shell-rce-flaws-get-public-exploits-patch-now/">WordPress Core &quot;wp2shell&quot; RCE flaws get public exploits, patch now</a></li>

</ul>
</details>

**标签**: `#security`, `#WordPress`, `#RCE`, `#vulnerability`, `#patch`

---

<a id="item-2"></a>
## [Kimi K3：中国 AI 模型通过蒸馏逼近前沿水平](https://stephen.bochinski.dev/blog/2026/07/18/the-kimi-k3-moment/) ⭐️ 8.0/10

中国实验室 Moonshot AI 发布了开源权重模型 Kimi K3，据称通过知识蒸馏技术，其性能接近 GPT-4 和 Claude 3.5 等美国前沿模型。 这加速了开源权重 AI 竞争的进程，挑战了美国的主导地位，并引发了对先进 AI 能力扩散的国家安全担忧。 Kimi K3 是一个开源权重模型，其训练参数可公开下载和微调。所使用的蒸馏技术将知识从更大的专有模型转移到更小、更高效的学生模型。

hackernews · sbochins · 7月18日 17:32 · [社区讨论](https://news.ycombinator.com/item?id=48960218)

**背景**: 知识蒸馏是一种机器学习技术，其中较小的“学生”模型学习模仿较大的“教师”模型的行为，通常以较低的计算成本实现可比的性能。开源权重模型公开发布训练参数，使任何人都能运行、修改或在此基础上构建。前沿 AI 实验室如 OpenAI 和 Anthropic 出于安全和竞争考虑，将其最强大的模型保持为专有。美国政府曾考虑将开源权重模型列为潜在的国家安全风险。Kimi K3 的报告性能表明，蒸馏可以有效地将前沿能力压缩到可访问的模型中，可能使先进 AI 民主化。这一发展类似于开源软件的早期趋势，专有创新很快被复制和分发。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Distillation_%28machine_learning%29">Distillation (machine learning)</a></li>
<li><a href="https://hai.stanford.edu/ai-definitions/what-is-an-open-weight-model">What is an Open-Weight Model? - Stanford HAI</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍认为蒸馏是不可避免的，但对 Kimi K3 的实际质量存在争议，一些人认为它不如其他模型。其他人则关注地缘政治影响，将潜在监管比作 Napster 时代。

**标签**: `#AI`, `#distillation`, `#open-source`, `#geopolitics`, `#machine learning`

---

<a id="item-3"></a>
## [GPT-5.6 Sol 解决 30 年凸优化猜想](https://old.reddit.com/r/math/comments/1uxj3cy/after_openais_cdc_proof_announcement_gpt56_used_a/) ⭐️ 8.0/10

一位研究者使用 GPT-5.6 Sol 在 148 分钟内证明了一个存在 30 年的凸优化猜想，标志着 AI 辅助数学的重大突破。 这展示了 AI 加速数学研究的潜力，但实际工作包括使用早期 GPT 版本进行的一年准备，削弱了自主发现的说法。 使用的模型是 GPT-5.6 Sol（而非 Ultra），提示词包含了研究者与 GPT-5.4 和 5.5 长达一年的聊天记录，使得该解决方案实际上是人与 AI 协作的结果。

hackernews · mbustamanter · 7月18日 13:00 · [社区讨论](https://news.ycombinator.com/item?id=48957779)

**背景**: 凸优化是数学优化的一个子领域，其中目标函数和约束是凸的，使得问题可解。该猜想涉及在球形域上优化凸 Lipschitz 函数的时间复杂度上界。GPT-5.6 是 OpenAI 最新的 LLM 系列，Sol 是最强大的变体，专为科学和编程中的高级推理而设计。研究者已为此问题工作了一年，使用早期 GPT 模型探索方法。最终给 GPT-5.6 Sol 的提示词包含了这些前期工作，从而在三小时内得到解决方案。这凸显了当前 AI 在研究中的能力与局限：AI 可以加速但尚不能取代人类洞察。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/GPT-5.6">GPT-5.6 - Wikipedia</a></li>
<li><a href="https://openai.com/index/previewing-gpt-5-6-sol/">Previewing GPT-5.6 Sol: a next-generation model | OpenAI</a></li>
<li><a href="https://en.wikipedia.org/wiki/Convex_optimization">Convex optimization - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 社区评论显示，研究者已使用 GPT-5.4 和 5.5 为此问题工作了一年，提示词包含了这些历史记录，使得“148 分钟”的说法具有误导性。一些评论者指出该猜想虽小众但确有贡献，其他人则讨论了 AI 在数学研究中的影响。

**标签**: `#AI`, `#mathematics`, `#convex optimization`, `#machine learning`, `#research`

---

<a id="item-4"></a>
## [AI 狂热正在摧毁全球决策](https://simonwillison.net/2026/Jul/19/ai-mania/#atom-everything) ⭐️ 8.0/10

Nik Suresh 发表了一篇博文，通过匿名轶事详细描述了 AI 狂热如何导致大公司做出非理性决策。 这篇批评文章揭示了 AI 炒作压倒合理商业策略的危险，可能导致各行业资源浪费和项目失败。 文中提到一位从未使用过 ChatGPT 的高管为一家营收超 20 亿美元的公司制定了以 AI 为中心的战略，还有工程师让 AI 将 Go 仓库重写为 Zig 以显得高产。

rss · Simon Willison · 7月19日 05:06

**背景**: AI 狂热指的是对人工智能技术的过度炒作和不加批判的采用，通常由害怕错过的心态驱动。大公司面临展示 AI 整合的压力，导致决策基于流行词而非证据。文章举例说明高管对生产力提升做出不切实际的声称，而供应商为避免合同取消不敢反驳客户。这种环境催生了无法交付价值的项目，Suresh 的团队观察到 18 个月内成功率为 0%。这一现象并非新鲜事，但随着 ChatGPT 等生成式 AI 的兴起而加剧。

**社区讨论**: Hacker News 的评论者意见不一：一些人同意批评，引用失败的 AI 项目；另一些人则认为，如果正确使用，Claude 等 AI 工具在编程任务上非常高效。少数人质疑“AI 项目”的定义，并认为文章声称 0%成功率是夸张的。

**标签**: `#AI`, `#corporate decision-making`, `#hype`, `#critique`, `#technology strategy`

---

<a id="item-5"></a>
## [7-Zip 26.02 修复压缩包远程代码执行漏洞](https://www.bleepingcomputer.com/news/security/update-now-7-zip-fixes-rce-flaw-exploitable-with-malicious-archives/) ⭐️ 8.0/10

7-Zip 26.02 版本发布，修复了一个远程代码执行漏洞（CVE-2025-11001），攻击者可通过利用符号链接的恶意 ZIP 压缩包执行任意代码。 该漏洞非常严重，因为 7-Zip 是全球最广泛使用的文件压缩工具之一，且已观察到野外主动利用，所有用户应立即更新。 该漏洞源于对精心构造的 ZIP 文件中符号链接的不当处理，导致目录遍历并在易受攻击应用程序的权限下执行代码。利用该漏洞需要提升的用户/服务账户或启用了开发者模式的机器。

rss · BleepingComputer · 7月18日 19:32

**背景**: 7-Zip 是一款免费、开源的文件压缩工具，压缩率高，广泛用于 Windows 及其他平台。远程代码执行（RCE）漏洞允许攻击者在受害者系统上运行任意代码。此漏洞（CVE-2025-11001）涉及符号链接——一种指向其他文件或目录的特殊文件。当 7-Zip 解压恶意压缩包时，可能跟随符号链接逃逸出目标解压目录，覆盖关键系统文件或执行代码。概念验证（PoC）利用代码已公开，NHS England Digital 和 Qualys 报告了主动利用。修复版本为 26.02，用户应立即安装。鉴于主动利用，手动修补已不足够，建议采用自动更新机制。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thehackernews.com/2025/11/hackers-actively-exploiting-7-zip.html">NHS Warns of PoC Exploit for 7-Zip Symbolic Link–Based RCE Vulnerability</a></li>
<li><a href="https://blog.qualys.com/product-tech/2025/12/04/active-exploitation-of-7-zip-rce-vulnerability-shows-why-manual-patching-is-no-longer-an-option">Active Exploitation of 7-Zip RCE Vulnerability Shows Why Manual Patching is No Longer an Option | Qualys</a></li>
<li><a href="https://socprime.com/blog/latest-threats/cve-2025-11001-and-cve-2025-11002-in-7zip/">CVE-2025-11001 and CVE-2025-11002 Vulnerabilities: Critical Flaws in 7-Zip Enable Remote Code Execution | SOC Prime</a></li>

</ul>
</details>

**社区讨论**: 社区讨论强调更新的紧迫性，许多用户对主动利用表示担忧。部分用户因需要提升权限而争论严重性，但总体意见是立即修补。

**标签**: `#security`, `#7-zip`, `#vulnerability`, `#RCE`, `#update`

---

<a id="item-6"></a>
## [上下文炸弹：新型防御技术瘫痪 AI 黑客代理](https://www.wired.com/story/prompt-injection-attacks-are-thwarting-ai-hacking-agents/) ⭐️ 8.0/10

一种名为“上下文炸弹”的技术利用提示注入来欺骗恶意 AI 代理，使其在造成危害之前自行关闭，从而将攻击向量转化为防御机制。 这标志着 AI 安全的范式转变：防御者不再仅仅检测 AI 驱动的攻击，而是可以利用使这些攻击成为可能的同一漏洞主动禁用它们。它为日益复杂的自主黑客代理提供了主动防御。 在 5 个前沿模型和 152 次运行的测试中，上下文炸弹将成功攻击路径从 91%降至 15%。该技术涉及在诱饵资源（蜜罐）中植入短字符串，当攻击者检索这些资源时，会触发 AI 模型自身的安全护栏。

rss · Wired · 7月18日 09:00

**背景**: 提示注入是一种网络安全利用手段，精心设计的输入会导致大型语言模型（LLM）产生意外行为。攻击者利用它绕过安全护栏，使 LLM 执行恶意操作。间接提示注入可以将对抗性提示嵌入到 LLM 检索的网站内容中。上下文炸弹将这种技术重新用于防御：防御者在诱饵凭证或文件中植入“上下文炸弹”。当 AI 黑客代理检索并处理这些诱饵时，嵌入的指令会触发模型的安全机制，使其拒绝进一步操作或自行关闭。该方法由 Tracebit 开发，并在真实的 AWS 环境中进行了测试。它代表了将对抗性技术用于防御目的的新颖应用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://tracebit.com/blog/context-bombs-stopping-ai-attackers-in-their-tracks">Context bombs: stopping AI attackers in their tracks | Tracebit</a></li>
<li><a href="https://www.helpnetsecurity.com/2026/07/14/context-bombs-for-defensive-prompt-injection/">&quot;Context bombs&quot; can frustrate AI-driven attacks... - Help Net Security</a></li>
<li><a href="https://en.wikipedia.org/wiki/Prompt_injection_attack">Prompt injection attack</a></li>

</ul>
</details>

**标签**: `#AI security`, `#prompt injection`, `#cybersecurity`, `#adversarial attacks`

---

<a id="item-7"></a>
## [Claude Code 改用 Rust 版 Bun，启动速度提升 10%](https://simonwillison.net/2026/Jul/19/claude-code-in-bun-in-rust/#atom-everything) ⭐️ 7.0/10

Simon Willison 通过二进制文件检查证实，Claude Code v2.1.181 及更高版本使用了 Rust 移植的 Bun，在 Linux 上启动速度提升了 10%。 这表明一款主流 AI 编程工具正在采用基于 Rust 的运行时来提升性能，凸显了用 Rust 重写性能关键组件的趋势。 Claude Code 中嵌入的 Bun 版本为 v1.4.0，比公开版本 v1.3.14 更新，表明 Anthropic 正在使用预览版。二进制文件中包含 500 多个 Rust 源文件路径，证实了 Rust 移植。

rss · Simon Willison · 7月19日 03:54

**背景**: Bun 是一个快速的全能 JavaScript 运行时、打包器和包管理器，旨在作为 Node.js 的直接替代品。Bun 最初用 Zig 编写，现在正用 Rust 重写以提升性能和可维护性。Claude Code 是 Anthropic 的智能编程工具，运行在终端中，帮助开发者编辑文件、运行命令并更快地交付代码。Rust 移植版的 Bun 尚未公开发布，Claude Code 正在使用预览版。Simon Willison 使用 &\#x27;strings&\#x27; 命令从 Claude Code 二进制文件中提取了版本信息和 Rust 源文件路径，提供了具体证据。10% 的启动提升虽然不大，但对开发者体验有实际意义。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/oven-sh/bun">GitHub - oven-sh/bun: Incredibly fast JavaScript runtime, bundler, test runner, and package manager – all in one</a></li>
<li><a href="https://docs.anthropic.com/en/docs/claude-code/overview">Claude Code overview - Anthropic</a></li>

</ul>
</details>

**标签**: `#Claude Code`, `#Bun`, `#Rust`, `#performance`, `#reverse engineering`

---

<a id="item-8"></a>
## [交互式 SQLite 查询解释器通过 Pyodide 在浏览器中运行](https://simonwillison.net/2026/Jul/18/sqlite-query-explainer/#atom-everything) ⭐️ 7.0/10

Simon Willison 构建了一个交互式 SQLite 查询解释器，该工具使用 Pyodide（一个基于 WebAssembly 的 Python 发行版）完全在浏览器中运行。它为 EXPLAIN 和 EXPLAIN QUERY PLAN 命令的输出添加了解释性注释。 该工具通过提供即时、可视化的解释，降低了开发者理解 SQLite 查询计划（一个公认的难点）的门槛，且无需安装任何软件。它展示了通过 WebAssembly 在浏览器中运行 Python 在开发者工具中的实际应用。 该工具使用 Pyodide 构建，Pyodide 将 Python 编译为 WebAssembly，使得 SQLite 可以在客户端运行。作者提醒说，他无法完全验证解释的正确性，因为他不是 SQLite 查询计划的专家。

rss · Simon Willison · 7月18日 17:19

**背景**: SQLite 是一个广泛使用的嵌入式数据库引擎。当执行 SQL 查询时，SQLite 会制定一个查询计划——一系列用于检索数据的操作。EXPLAIN 命令显示底层的虚拟机指令，而 EXPLAIN QUERY PLAN 则提供策略的高级摘要，包括索引使用情况。理解这些计划对于优化查询性能至关重要，但其输出可能难以理解。Pyodide 是一个将 CPython 移植到 WebAssembly 的项目，使得 Python 代码可以在浏览器中运行。Simon Willison 是知名开发者，也是 Datasette（一个用于探索和发布数据的工具）的创建者。该工具的灵感来源于 Julia Evans 关于学习 SQLite 内部机制的博客文章。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://pyodide.org/">Pyodide — Version 314.0.2</a></li>
<li><a href="https://www.sqlite.org/eqp.html">Explain query plan</a></li>
<li><a href="https://github.com/pyodide/pyodide">GitHub - pyodide/pyodide: Pyodide is a Python distribution for the browser and Node.js based on WebAssembly · GitHub</a></li>

</ul>
</details>

**标签**: `#sqlite`, `#query-plan`, `#developer-tools`, `#webassembly`, `#sql`

---

<a id="item-9"></a>
## [微软警告 ACR 窃密软件攻击激增](https://www.bleepingcomputer.com/news/security/microsoft-warns-of-surge-in-acr-stealer-attacks-on-customers/) ⭐️ 7.0/10

微软发出警告，称使用 ACR 窃密软件的攻击激增，该恶意软件针对企业客户，窃取浏览器存储的密码、身份验证令牌和敏感文档。 此次攻击激增对企业安全构成重大威胁，因为窃取的凭证和令牌可能导致数据泄露和对关键系统的未授权访问。微软的警告凸显了组织需要加强防御信息窃取型恶意软件的必要性。 ACR 窃密软件于 2024 年 3 月首次出现，作为恶意软件即服务在俄语网络犯罪论坛上出售。此后它不断演变，并于 2025 年更名为 Amatera 窃密软件，具备更强的规避技术。

rss · BleepingComputer · 7月18日 14:17

**背景**: 信息窃取型恶意软件是一种旨在从受感染设备中提取敏感数据（如保存的密码、cookie 和身份验证令牌）的恶意程序。浏览器存储的密码是常见目标，因为许多用户依赖浏览器记住登录凭证。身份验证令牌使攻击者能够绕过多因素认证并保持持久访问。ACR 窃密软件是恶意软件即服务增长趋势的一部分，开发者将恶意软件出售或出租给其他犯罪分子。更名为 Amatera 窃密软件表明其持续开发以适应检测。微软的警告基于其安全产品观察到的遥测数据，反映了现实世界的攻击模式。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://malpedia.caad.fkie.fraunhofer.de/details/win.acr_stealer">ACR Stealer (Malware Family)</a></li>
<li><a href="https://www.proofpoint.com/us/blog/threat-insight/amatera-stealer-rebranded-acr-stealer-improved-evasion-sophistication">Amatera Stealer: Rebranded ACR Stealer With Improved Evasion, Sophistication | Proofpoint US</a></li>
<li><a href="https://www.microsoft.com/en-us/security/blog/2022/11/16/token-tactics-how-to-prevent-detect-and-respond-to-cloud-token-theft/">Token tactics: How to prevent, detect, and respond to cloud token theft | Microsoft Security Blog</a></li>

</ul>
</details>

**标签**: `#malware`, `#cybersecurity`, `#enterprise`, `#data theft`, `#Microsoft`

---

<a id="item-10"></a>
## [D7VK 2.0 发布，性能提升高达两倍](https://www.phoronix.com/news/D7VK-2.0-Released) ⭐️ 7.0/10

D7VK 2.0 作为 Direct3D 7 及更早版本到 Vulkan 的转换层的主要版本发布，性能提升高达两倍或更多。 此版本显著提升了在 Linux 及其他使用 Vulkan 的平台上运行旧版 Direct3D 7 游戏的性能，使老游戏更可玩，并扩展了兼容层生态系统。 D7VK 2.0 基于 DXVK 代码库构建，通过 Direct3D 9 中间层将 Direct3D 7、6、5 和 3 的调用转换为 Vulkan。性能提升源于转换管道和着色器编译的优化。

rss · Phoronix \(Linux\) · 7月18日 10:32

**背景**: D7VK 是一个开源转换层，允许 Direct3D 7 及更早版本的游戏在 Linux 和其他使用 Vulkan API 的平台上运行。它是 DXVK 的一个分支，DXVK 将 Direct3D 8/9/10/11 转换为 Vulkan。Direct3D 7 是微软 DirectX 7 中的旧版图形 API，许多老 Windows 游戏使用它。通过将这些调用转换为 Vulkan，D7VK 使这些游戏能够受益于现代 GPU 驱动程序和跨平台兼容性。该项目由 WinterSnowfall 在 GitHub 上维护，并与 Wine 或 Proton 结合使用，以在 Linux 上运行 Windows 游戏。2.0 版本的性能提升对于之前受限于 CPU 开销或着色器编译卡顿的游戏尤为显著。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/WinterSnowfall/d7vk">GitHub - WinterSnowfall/d7vk: Vulkan-based implementation of D3D7, 6, 5 and 3 for Linux / Wine, spun off from DXVK. · GitHub</a></li>
<li><a href="https://en.wikipedia.org/wiki/DXVK">DXVK</a></li>
<li><a href="https://en.wikipedia.org/wiki/Direct3D">Direct3D</a></li>

</ul>
</details>

**标签**: `#D7VK`, `#Vulkan`, `#Linux Gaming`, `#Performance`, `#Direct3D`

---

<a id="item-11"></a>
## [邻近岩石超级地球 GJ3378b 确认位于宜居带](https://www.solidot.org/story?sid=84862) ⭐️ 7.0/10

天文学家确认，距离地球仅 25 光年的系外行星 GJ3378b 是一颗位于红矮星宜居带内的岩石超级地球，修正了此前将其归类为迷你海王星的结论。 这使得 GJ3378b 成为已知最接近的潜在宜居岩石世界之一，为未来利用詹姆斯·韦伯太空望远镜等设备进行大气研究提供了绝佳目标。 该行星的质量从 5.26 个地球质量修正为 2.3 个地球质量，公转周期从 25 天修正为 21 天，使其恰好位于保守宜居带内，接收的恒星辐射量约为地球的 90%。

rss · Solidot · 7月18日 15:14

**背景**: GJ3378b 围绕红矮星 GJ3378 运行，该恒星距离地球约 25 光年，位于鹿豹座。红矮星体积小、温度低且寿命长，是系外行星搜寻的常见宿主。宜居带是指温度允许行星表面存在液态水的区域。该行星最初于 2024 年被法国天文学家发现，当时被认为是一颗气态迷你海王星。利用基特峰国家天文台的 WIYN 3.5 米望远镜等设备进行的后续观测修正了其质量和轨道，揭示了岩石质地。该行星接收的辐射量约为地球从太阳获取的 90%，这是潜在宜居性的有利条件。然而，它距离红矮星较近，引发了关于恒星活动可能剥离其大气的担忧。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/GJ_3378">GJ 3378</a></li>
<li><a href="https://science.nasa.gov/exoplanet-catalog/gj-3378-b/">GJ 3378 b - NASA Science</a></li>
<li><a href="https://noirlab.edu/public/videos/WIYN-Timelapse-3-22-22-CC/">A Busy WIYN 3.5-meter Telescope | NOIRLab</a></li>

</ul>
</details>

**标签**: `#exoplanet`, `#astronomy`, `#habitable zone`, `#super-Earth`, `#space science`

---

<a id="item-12"></a>
## [经期追踪应用向第三方共享敏感数据](https://www.wired.com/story/security-news-this-week-your-period-tracker-is-probably-spying-on-you/) ⭐️ 7.0/10

《连线》杂志文章警告，经期追踪应用可能向第三方共享敏感用户数据，凸显隐私风险。Mozilla 研究发现 Stardust 应用向第三方共享健康数据。 这很重要，因为经期追踪应用处理高度个人化的健康信息，数据共享可能导致隐私侵犯或歧视。用户可能在不知情的情况下向广告商或其他实体暴露敏感数据。 Mozilla 基金会调查了六款热门经期追踪应用：Flo、Clue、Stardust、Spot On、Period Calendar 和 Euki。部分应用有强保护措施，而其他应用以用户可能感到不安的方式共享数据。

rss · Wired · 7月18日 10:30

**背景**: 经期追踪应用允许用户记录月经周期、症状和受孕期。这些数据高度敏感，可能揭示怀孕、性活动和健康状况。许多应用依赖广告或数据变现，从而产生向第三方共享数据的动机。在罗诉韦德案被推翻后，隐私担忧加剧，因为经期数据可能被用于法律案件。Mozilla 的研究强调，并非所有应用都对其数据实践保持透明。用户应审查应用隐私政策，并考虑使用具有强隐私保护的应用，如 Euki。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.bbc.com/future/article/20260715-how-period-trackers-share-womens-private-details">How period trackers share your private details</a></li>
<li><a href="https://news.google.com/stories/CAAqNggKIjBDQklTSGpvSmMzUnZjbmt0TXpZd1NoRUtEd2ppMnZuT0VSSHNRcWtaV3RvLW1TZ0FQAQ?hl=en-US&amp;gl=US&amp;ceid=US:en">Mozilla study reveals data sharing in period tracking apps - Overview</a></li>

</ul>
</details>

**标签**: `#privacy`, `#security`, `#data collection`, `#apps`

---



---

## 技术专题

好的，我们来聊聊一个在数据科学和机器学习领域几乎无人不知，但又常常被误解其真正价值的工具——**Jupyter Notebook**。

### 1. 背景和定位：从“学术玩具”到“行业标配”

Jupyter Notebook 最初源于 2014 年的 IPython Notebook 项目。它的核心定位非常独特：**一个基于 Web 的交互式计算环境，允许你创建和共享包含实时代码、方程、可视化和叙述性文本的文档。**

在它出现之前，数据科学家的典型工作流是割裂的：用 Python/R 脚本写代码，用 Excel 或 Matplotlib 看结果，用 Word/LaTeX 写报告。调试和探索过程非常痛苦，每次修改代码都要重新运行整个脚本，或者手动记录中间结果。

Jupyter 的核心理念就是“**可复现的叙事性计算**”。它把代码、输出、图表、公式和解释性文字整合在一个文档（.ipynb 文件）里。这让它迅速成为学术界和工业界数据探索、原型设计、教学演示的首选工具。它不是一个“编程语言”，而是一个“编程环境”和“文档格式”的结合体。

### 2. 核心原理：Cell、Kernel 与交互式计算

Jupyter 的魔力源于三个核心概念：

*   **Cell (单元格)**：这是文档的基本单元。主要有两种类型：
    *   **Code Cell (代码单元格)**：你可以在这里编写并执行代码（如 Python、R、Julia）。执行后，输出（文本、表格、图片、甚至交互式控件）会直接显示在单元格下方。
    *   **Markdown Cell (Markdown 单元格)**：用于编写格式化文本、标题、列表、链接、数学公式（LaTeX）等。这是实现“叙事性”的关键。

*   **Kernel (内核)**：这是 Jupyter 的大脑。它是一个独立的计算引擎（比如一个 Python 解释器进程），负责执行 Code Cell 中的代码。当你在浏览器中点击“运行”按钮时，请求会发送到 Kernel，Kernel 执行代码，然后把结果（输出、错误信息、图表数据）返回给浏览器显示。**Kernel 是有状态的**——这意味着你在一个 Cell 中定义的变量、导入的库、训练好的模型，在后续的 Cell 中都可以直接使用。这彻底改变了“写脚本-运行-看结果-修改-再运行”的循环，变成了“写一段-运行-看结果-根据结果写下一段”的探索式工作流。

*   **交互式计算与状态持久化**：这是 Jupyter 区别于传统 IDE 最核心的一点。你可以分步执行代码，随时检查中间变量，修改代码后只重新运行受影响的部分。这种“REPL (Read-Eval-Print Loop) 的增强版”体验，非常适合数据探索和算法调试。当你关闭浏览器再打开，只要 Kernel 还在运行，所有状态都保留。你也可以将 .ipynb 文件保存，下次打开时，所有代码和输出都还在，实现了完美的“可复现”。

### 3. 应用场景：远不止于写 Python

*   **数据探索与清洗 (EDA)**：这是 Jupyter 最经典的应用。你可以快速加载数据，用 `df.head()` 查看前几行，用 `matplotlib` 或 `seaborn` 画个分布图，发现缺失值后写几行代码处理，再画个图对比处理前后效果。整个过程流畅、直观、可记录。
*   **机器学习和深度学习原型设计**：用 Jupyter 搭建模型原型非常高效。你可以在一个 Cell 里定义模型结构，下一个 Cell 训练，再下一个 Cell 评估。如果效果不好，可以回溯修改参数或模型结构，只重新运行相关 Cell。TensorFlow、PyTorch 的官方教程和示例代码大量使用 Jupyter Notebook。
*   **教学与演示**：将理论讲解（Markdown）、代码示例（Code）、运行结果（图表）放在一个文档里，学生可以边看边改边运行，学习效果远超静态的 PPT 或代码文件。
*   **报告与协作**：你可以将整个分析过程打包成一个 Notebook，直接分享给同事或发布到 GitHub。对方可以复现你的所有步骤。工具如 `nbconvert` 可以将 Notebook 导出为 HTML、PDF、幻灯片等格式。
*   **交互式数据可视化**：结合 `ipywidgets` 库，你可以在 Notebook 中创建滑块、下拉菜单等控件，让用户动态调整参数并实时更新图表，构建轻量级的交互式数据应用。

### 4. 同类对比：Jupyter vs. 传统 IDE vs. 其他 Notebook

| 特性 | Jupyter Notebook | 传统 IDE (如 VS Code, PyCharm) | 其他 Notebook (如 Google Colab, Deepnote) |
| :--- | :--- | :--- | :--- |
| **核心工作流** | 探索式、分步执行、状态持久化 | 脚本式、调试、项目管理 | 与 Jupyter 类似，但更侧重云端协作 |
| **代码组织** | 按 Cell 组织，非线性执行 | 按文件/项目组织，线性执行 | 按 Cell 组织 |
| **状态管理** | **Kernel 有状态**，变量跨 Cell 共享 | 通常无状态，每次运行整个脚本 | 有状态，但云端 Kernel 可能超时断开 |
| **适用场景** | 数据分析、原型设计、教学、报告 | 大型软件开发、复杂工程、重构 | 协作、云端 GPU 资源、分享 |
| **优点** | 交互性强、叙事性好、易于分享 | 代码补全、重构、调试、版本控制集成强 | 零配置、免费 GPU、实时协作 |
| **缺点** | 难以管理大型项目、代码可读性差（Cell 顺序依赖）、版本控制困难（JSON 格式） | 探索式工作流不流畅、报告生成能力弱 | 依赖网络、隐私和数据安全问题 |

**核心区别**：Jupyter 是为“探索”而生，IDE 是为“构建”而生。对于需要反复尝试、快速验证想法的数据科学任务，Jupyter 更胜一筹；对于需要编写健壮、可维护的生产级代码的软件工程任务，IDE 是更好的选择。

### 5. 学习建议：从“会用”到“用好”

1.  **安装与上手**：最简单的方式是安装 **Anaconda** 发行版，它自带 Jupyter Notebook 和常用数据科学库。打开终端输入 `jupyter notebook` 即可启动。创建一个新 Notebook，尝试运行 `print("Hello World")`，然后试试 Markdown Cell。
2.  **掌握快捷键**：这是提升效率的关键。`Shift+Enter` 运行当前 Cell 并选中下一个，`Ctrl+Enter` 运行当前 Cell，`A` 在上方插入 Cell，`B` 在下方插入，`D+D` 删除 Cell。熟悉这些快捷键能让你“手不离键盘”。
3.  **拥抱“探索式”思维**：不要试图一次性写完所有代码。先加载数据，观察它；然后写一小段清洗代码，运行，检查结果；再画个图，分析一下。把 Notebook 当作你的“实验记录本”。
4.  **注意“Cell 顺序依赖”陷阱**：这是新手最容易犯的错误。你可能会在 Cell 5 中定义了一个变量，然后回到 Cell 2 使用它。这在 Jupyter 里是可行的，但如果你重新运行整个 Notebook（Kernel -> Restart & Run All），Cell 2 会报错，因为变量还未定义。**最佳实践是：保持 Cell 的执行顺序是自上而下的。** 定期使用“Restart & Run All”来验证你的 Notebook 是否是可复现的。
5.  **善用 Markdown 和魔法命令**：用 Markdown 记录你的思考、假设和结论，让 Notebook 成为一份完整的报告。Jupyter 的“魔法命令” (Magic Commands) 非常强大，例如 `%timeit` 测量代码执行时间，`%matplotlib inline` 让图表直接显示在 Cell 下方，`%%writefile` 将 Cell 内容写入文件。
6.  **转向 JupyterLab**：JupyterLab 是 Jupyter Notebook 的下一代界面，提供了更现代的 IDE 体验（多标签、文件浏览器、终端、拖拽等）。强烈建议直接使用 JupyterLab。

**一句话总结**：Jupyter Notebook 不是一个用来写“最终代码”的工具，而是一个用来“思考、探索和沟通”你的数据科学思路的工具。掌握它，你将拥有一个强大的“数字实验笔记本”。