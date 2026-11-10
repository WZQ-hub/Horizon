---
layout: default
title: "Horizon Summary: 2026-11-10 (ZH)"
date: 2026-11-10
lang: zh
---

> 从 193 条内容中筛选出 12 条重要资讯。

---

**科技新闻**
1. [Claude Code 本地设置文件暴露 2539 个凭据](#item-tech-news-1) ⭐️ 8.0/10
2. [AlphaProof Code 引发形式化验证讨论](#item-tech-news-2) ⭐️ 7.0/10
3. [Blender 5.3 发布，支持 Gaussian Splat](#item-tech-news-3) ⭐️ 7.0/10
4. [.NET 11 运行时更新引发兼容性讨论](#item-tech-news-4) ⭐️ 7.0/10
5. [Anthropic 拟以 1.4 万亿美元估值上市](#item-tech-news-5) ⭐️ 7.0/10
6. [Megaspeed 涉嫌转运英伟达芯片受审视](#item-tech-news-6) ⭐️ 7.0/10
7. [SWE-Pair 测试编码智能体同时修复两个漏洞](#item-tech-news-7) ⭐️ 7.0/10
8. [断电预测模型在留出年份测试中优于天气预警基线](#item-tech-news-8) ⭐️ 7.0/10
9. [英国议员提议手机预装儿童性虐待内容屏蔽软件](#item-tech-news-9) ⭐️ 7.0/10
10. [Fireworks 再遭攻击，部分客户数据外泄](#item-tech-news-10) ⭐️ 7.0/10
11. [Anthropic 支持地区政策排除中国大陆及港澳](#item-tech-news-11) ⭐️ 7.0/10
12. [MiniMax H3 Image 开放权重，支持 4K 图像生成](#item-tech-news-12) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [Claude Code 本地设置文件暴露 2539 个凭据](https://www.ithome.com/1/024/888.htm) ⭐️ 8.0/10

安全公司 Apiiro 报告称，在 1994 个 GitHub 代码库中发现了 2539 个真实凭据，包括数据库密码和 API Token。这些凭据出现在被提交到公共仓库的 Claude Code 本地设置文件中：超过 10 万份此类文件被上传，其中约 1100 份含机密数据。Claude Code 会将获准执行的 Shell 命令写入本地设置文件；团队表示正研究预防措施，并考虑内置密钥扫描，但尚未称该功能已经推出。

telegram · zaihuapd · 11月10日 11:20

**「背景」** Claude Code 会将获准执行的 Shell 命令写入本地设置文件；如果命令中含有凭据，且设置文件未被 Git 忽略，凭据就可能随项目提交到公开仓库。

**「对开发者的影响」** 使用 Claude Code 的开发者应检查本地设置文件是否包含凭据，以及是否被 Git 忽略；未被忽略的文件可能随项目提交到公共仓库。

**标签**: `#Claude Code`, `#credential exposure`, `#GitHub`, `#secret scanning`, `#AI coding tools`

---

<a id="item-tech-news-2"></a>
### [AlphaProof Code 引发形式化验证讨论](https://deepmind.google/blog/introducing-alphaproof-code/) ⭐️ 7.0/10

DeepMind 一篇题为《AlphaProof Code》的文章引发了关于 AI 辅助形式化验证的讨论。由于未提供文章正文，目前无法核实该项目的具体能力、验证结果或创新之处。

hackernews · Google DeepMind · 11月10日 12:11 · [社区讨论](https://news.ycombinator.com/item?id=50439193)

**「背景」** 形式化验证通过数学证明检查软件是否满足给定的形式化规格；证明的范围取决于所选性质，不能自动保证规格涵盖了所有预期要求。DeepMind 将 AlphaProof Code 描述为多大语言模型代理框架，由人类专家与 AI 共同决定证明目标，再由一组 AI 代理开展验证工作。

**「社区讨论」** 评论者 hedora 质疑，若验证未发现缺陷，可能是定理有误或证明的属性过于狭窄；thibsrn 也提出，该工具似乎只检验实现而不质疑规范本身。这些是评论者对证明范围和规范正确性的疑问，并非已核实的项目结论。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://deepmind.google/blog/introducing-alphaproof-code/">Formal Verification of Signal’s Protocol with... — Google DeepMind</a></li>

</ul>
</details>

**标签**: `#formal verification`, `#AI coding agents`, `#proof assistants`, `#software correctness`

---

<a id="item-tech-news-3"></a>
### [Blender 5.3 发布，支持 Gaussian Splat](https://www.blender.org/download/releases/5-3/) ⭐️ 7.0/10

Blender 5.3 据报道已发布，为 3D 图形工作流加入 Gaussian Splat 支持。现有材料未说明该功能的具体能力、兼容性或性能。

hackernews · amlib · 11月10日 16:15 · [社区讨论](https://news.ycombinator.com/item?id=50442426)

**「背景」** 高斯泼溅是一种使用三维高斯体来表示和渲染场景的技术，与使用三角形网格构建模型的方法不同。在 Blender 中，高斯泼溅数据可作为点云导入，并通过几何节点处理。

**「社区讨论」** 一位用户表示，几何节点中的 Bundle 支持配合列表和闭包，有助于构建复杂工作流；他曾在 alpha 版本中使用该功能。另一位用户称，在搭载 M4 的设备上用 beta 版本测试了包含 400 万个 splat 的场景，认为其速度和界面集成都表现良好；这属于个人体验，并非独立性能测试。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.blender.org/download/releases/5-3/">5 . 3 — Blender</a></li>

</ul>
</details>

**标签**: `#Blender`, `#Gaussian splatting`, `#3D rendering`, `#geometry nodes`, `#open source`

---

<a id="item-tech-news-4"></a>
### [.NET 11 运行时更新引发兼容性讨论](https://learn.microsoft.com/en-us/dotnet/core/whats-new/dotnet-11/runtime) ⭐️ 7.0/10

微软发布了介绍 .NET 11 运行时新特性的文档，面向使用 .NET 的开发者。所提供的正文仅包含 .NET 11 公告链接，未列出运行时的具体变更或适用条件，因此无法据此评估各项新特性。

hackernews · stevefan1999 · 11月10日 12:20 · [社区讨论](https://news.ycombinator.com/item?id=50439284)

**「背景」** C\# 中的浮点数和 decimal 使用不同的数值表示方式：0.1 无法用二进制浮点数精确表示，因此从浮点数转换为 decimal 时，转换规则可能影响最终显示的数值。

**「社区讨论」** 一名评论者提醒开发者注意 decimal 转换的兼容性，并给出示例：在 .NET 10 中，\(decimal\)0.1 得到 0.1，而在 .NET 11 中得到 0.1000000000000000055511151231；所提供的正文不足以独立核实这一变化及其条件。另有评论者对运行时异步支持可能如何影响自定义 AsyncBuilder 表示疑问。

**标签**: `#.NET 11`, `#.NET runtime`, `#C\#`, `#backward compatibility`

---

<a id="item-tech-news-5"></a>
### [Anthropic 拟以 1.4 万亿美元估值上市](https://www.aljazeera.com/economy/2026/11/10/anthropic-targets-1-4-trillion-valuation-in-massive-stock-market-debut?traffic_source=rss) ⭐️ 7.0/10

据报道，Claude 开发商 Anthropic 计划下周首次公开募股，目标估值为 1.4 万亿美元，拟筹资最多 644 亿美元。报道描述的是上市目标，而非已经完成的发行。

rss · Al Jazeera · 11月10日 17:21

**「背景」** 首次公开募股（IPO）是公司首次向公众发行股票的过程，可为公司筹集资金。Anthropic 开发了 Claude 人工智能助手。

**标签**: `#Anthropic`, `#Artificial Intelligence`, `#IPO`, `#Technology Industry`

---

<a id="item-tech-news-6"></a>
### [Megaspeed 涉嫌转运英伟达芯片受审视](https://www.dw.com/zh/%E9%BB%84%E4%BB%81%E5%8B%8B%E9%A3%8E%E6%B3%A2%E8%B0%83%E6%9F%A5%EF%BC%9A%E9%BB%84%E4%B9%90%E4%BB%BB%E8%81%8C%E7%9A%84%E6%96%B0%E5%8A%A0%E5%9D%A1%E5%85%AC%E5%8F%B8%E4%BB%80%E4%B9%88%E6%9D%A5%E5%A4%B4%EF%BC%9F/a-79907996?maca=chi-rss-chi-all-1127-rdf) ⭐️ 7.0/10

新加坡公司 Megaspeed 因涉嫌向中国转运英伟达芯片而受到审视，其资产据报道在一年内从 3300 万美元增至 30 亿美元。曾任该公司高管的黄乐被指为中国间谍，据报曾被新加坡限制离境。美国商务部调查人员对 Megaspeed 调查数月后，调查工作于去年年底突然中止；报道未说明中止原因，也未提供涉嫌转运的具体证据。

rss · DW 中文 · 11月10日 11:16

**「背景」** Megaspeed 是英伟达的一家新加坡客户，曾购买该公司的先进 AI 芯片；美国商务部对它的调查与涉嫌将受限制的芯片转供中国企业有关。有关转运仍是指控，并非已证实的事实。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.nytimes.com/2026/11/09/business/economy/nvidia-megaspeed-investigation-huang.html">U.S. Commerce Dept . Inquiry Into Megaspeed Was Halted After...</a></li>
<li><a href="https://www.cnbc.com/2026/11/10/jensen-huang-nvidia-china-ties.html">Huang affair with alleged Chinese spy complicates Nvidia China...</a></li>

</ul>
</details>

**标签**: `#Nvidia`, `#AI chip supply chains`, `#China chip transfers`, `#US Commerce Department`, `#Singapore`

---

<a id="item-tech-news-7"></a>
### [SWE-Pair 测试编码智能体同时修复两个漏洞](https://www.reddit.com/r/MachineLearning/comments/1xsuqem/swepair_a_codingagent_benchmark_where_every_task/) ⭐️ 7.0/10

SWE-Pair 发布了一组编码智能体基准任务，涵盖 69 个 Python 项目中的 161 项任务，每项要求同时修复两个真实漏洞。基准创建者报告称，DeepSeek V4.1 Flash 在 medium 推理强度下解决了 90% 的任务，平均每解决一项约花费 0.06 美元；GPT-6 Luna 在 max 强度下解决了 78%，每项约 0.23 美元。创建者还称，DeepSeek 在 max 强度下的成功率为 88%，成本是 medium 的 1.7 倍；这些结果尚未得到独立验证，帖文也未说明详细评测方法。

reddit · r/MachineLearning · /u/heyitsdannyle · 11月10日 18:33

**「背景」** 编码智能体基准通过软件修复等任务评估模型解决实际编程问题的能力。SWE-Pair 的任务要求智能体同时修复两个真实漏洞，因此其结果应结合这类任务和具体运行配置理解。

**「对开发者的影响」** 开发者可以使用已发布的数据集和智能体运行记录检查结果，也可以通过帖文提供的 Harbor 命令运行自己的智能体。

**标签**: `#coding agents`, `#software engineering benchmarks`, `#bug fixing`, `#LLM evaluation`

---

<a id="item-tech-news-8"></a>
### [断电预测模型在留出年份测试中优于天气预警基线](https://www.reddit.com/r/MachineLearning/comments/1xs4hq8/forecasting_new_power_outages_per_county_hourly_2/) ⭐️ 7.0/10

一名开发者称，其基于 XGBoost 的模型每小时为密苏里州和伊利诺伊州的 216 个县预测新发断电风险：从预测时刻起两小时后的六小时内，县内至少 5% 的用户新遭断电的概率。作者报告，在 2025 年留出测试中，模型的 PR-AUC 为 0.094，基于美国国家气象局（NWS）预警和风暴预测中心（SPC）首日展望的基线为 0.039，约相差 2.4 倍；按风暴日配对自助法估计的 95% 区间为 2.0 至 3.3 倍。在相同预警数量下，模型捕获了 30% 的新发断电，基线为 17%；精确率分别为 15% 和 11%。这些结果由作者自行报告，且主要测试限于两州；项目据称已于 11 月 1 日上线，并保存每次预测以供盲测。

reddit · r/MachineLearning · /u/CarRepresentative843 · 11月9日 21:34

**「方法背景」** 模型使用发布时的 HRRR 天气预报最近五次运行的均值，以及县级信息、当前断电和邻县数据，而非事后观测天气。预测目标只计新发断电，不因预测到已经发生的断电而得分；作者称模型使用 2020 至 2024 年数据训练、以 2024 年验证，并用 2025 年测试。

**「实际使用」** 对需要筛选断电风险的用户而言，该测试显示模型在相同预警数量下可比所选基线捕获更多新发断电，但 15% 的精确率意味着多数预警对应的目标事件仍未发生。作者还报告了对艾奥瓦州、印第安纳州和密歇根州的初步迁移测试：三州合计捕获率为 31%，基线为 19%，但这尚不足以证明模型在更广地区稳定有效。

**标签**: `#machine learning`, `#power outage forecasting`, `#XGBoost`, `#weather forecasting`, `#model evaluation`

---

<a id="item-tech-news-9"></a>
### [英国议员提议手机预装儿童性虐待内容屏蔽软件](https://observer.co.uk/news/national/article/fight-to-block-child-sexual-abuse-images-unites-peers-and-mps-in-cross-party-campaign) ⭐️ 7.0/10

英国跨党派议员和上院议员提出，要求科技公司在英国销售的所有手机和平板电脑上预装软件，自动模糊儿童性虐待图像和视频，包括 AI 生成内容，并使相关直播无法进行。提案还要求通过强制更新覆盖旧设备；目前尚未说明检测技术、实施细节或立法前景。

telegram · zaihuapd · 11月10日 05:11

**「背景」** 英国政府此前已承诺立法，要求苹果和谷歌阻止儿童拍摄和分享裸照；这一承诺与跨党派联盟现提出的设备预装软件方案不同。

**「潜在影响」** 如果提案成为法律，设备制造商可能需要为英国销售的手机和平板预装相关软件，并向旧设备推送强制更新。

**标签**: `#设备端内容检测`, `#儿童安全`, `#英国科技监管`, `#AI生成内容`, `#移动设备`

---

<a id="item-tech-news-10"></a>
### [Fireworks 再遭攻击，部分客户数据外泄](https://finance.sina.com.cn/stock/usstock/c/2026-11-10/doc-iniyfzhx2605532.shtml) ⭐️ 7.0/10

Fireworks 确认遭遇新一轮黑客攻击，部分客户的账单信息、模型权重和数据集外泄，正与帕洛阿尔托网络旗下 Unit 42 联合调查。客户 Harvey 表示其客户数据未受影响；其他客户及终端用户是否受到波及仍不清楚。

telegram · zaihuapd · 11月10日 13:00

**「背景」** 模型权重是人工智能模型在训练过程中形成的参数；数据集则可用于模型训练或评估。这两类资料可能包含客户投入开发的资源或敏感信息。

**「客户影响」** 据知情人士称，部分每年向 Fireworks 支付数百万美元的大客户正考虑迁移，但报道未确认其最终决定。

**标签**: `#Fireworks`, `#数据泄露`, `#AI 模型权重`, `#网络安全`

---

<a id="item-tech-news-11"></a>
### [Anthropic 支持地区政策排除中国大陆及港澳](https://www.anthropic.com/legal/supported-regions) ⭐️ 7.0/10

据报道，Anthropic 发布支持地区政策，将 Claude 产品和服务的可用范围限定在名单所列的 185 个国家和地区，中国大陆、香港及澳门均不在名单内。限制涵盖 Claude.ai、Claude Code、Cowork、API，以及通过云平台和授权经销商提供的 Claude 模型。来源称政策于 11 月 12 日生效，但未注明年份。

telegram · zaihuapd · 11月10日 13:44

**「背景」** 地区白名单是指只有明确列入政策的国家和地区才受支持；未列入名单并不意味着可以使用，而是被视为不受支持。

**「使用限制」** 身处不受支持地区的用户不能使用相关服务，包括赴当地出差的受支持地区公司员工。在不受支持地区注册或设总部的实体及其人员，以及被这些地区主体直接或间接多数持股或控制的公司人员，也受到限制，无论使用者身处何地。

**标签**: `#Anthropic`, `#Claude`, `#regional availability`, `#AI policy`, `#API access`

---

<a id="item-tech-news-12"></a>
### [MiniMax H3 Image 开放权重，支持 4K 图像生成](https://huggingface.co/MiniMaxAI/MiniMax-H3-Image) ⭐️ 7.0/10

稀宇科技发布并开放 MiniMax H3 Image 图像模型的权重，支持文生图、图像参考和编辑，最多可输入 16 张参考图。官方称，该模型生成一张 4096×4096 图像约需 10 秒，但所提供的资料未说明测试条件或独立验证结果。模型已上线 Hugging Face 和开放平台 API，并接入 MiniMax Code、海螺等产品；官方同时推出 Highspeed 高速版本。标准版 4K 图像价格约为每张 0.069 美元，发布首周优惠价约为 0.034 美元。

telegram · zaihuapd · 11月10日 15:39

**「背景」** 图像生成模型既可以根据文字描述生成画面，也可以参考已有图像进行生成或编辑。开放模型权重意味着开发者可以获取模型参数，而不必只通过厂商的托管接口使用模型。

**「使用影响」** 开发者可以获取模型权重，也可以通过 API 使用其图像生成和编辑能力；评估速度或成本时，应注意约 10 秒的生成时间缺少具体测试条件。

**标签**: `#image generation`, `#open-weight models`, `#image editing`, `#MiniMax`, `#4K images`

---