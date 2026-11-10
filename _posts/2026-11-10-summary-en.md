---
layout: default
title: "Horizon Summary: 2026-11-10 (EN)"
date: 2026-11-10
lang: en
---

> From 193 items, 12 important content pieces were selected

---

**Technology News**
1. [Claude Code Settings Exposed 2,539 Credentials in Public Repositories](#item-tech-news-1) ⭐️ 8.0/10
2. [AlphaProof Code Prompts Debate Over AI-Assisted Verification](#item-tech-news-2) ⭐️ 7.0/10
3. [Blender 5.3 Released With Gaussian Splat Support](#item-tech-news-3) ⭐️ 7.0/10
4. [.NET 11 Runtime Update Prompts Compatibility Discussion](#item-tech-news-4) ⭐️ 7.0/10
5. [Anthropic Targets $1.4 Trillion Valuation in Planned IPO](#item-tech-news-5) ⭐️ 7.0/10
6. [Singapore’s Megaspeed Scrutinized Over Suspected Nvidia Chip Transfers](#item-tech-news-6) ⭐️ 7.0/10
7. [SWE-Pair Benchmarks Coding Agents on Two-Bug Tasks](#item-tech-news-7) ⭐️ 7.0/10
8. [County Outage Forecast Reports 2.4× Baseline PR-AUC](#item-tech-news-8) ⭐️ 7.0/10
9. [UK Cross-Party Campaign Seeks Abuse-Image Blocking Software on Devices](#item-tech-news-9) ⭐️ 7.0/10
10. [Fireworks Confirms New Attack Exposing Customer Data and Model Weights](#item-tech-news-10) ⭐️ 7.0/10
11. [Anthropic’s Supported-Regions Policy Excludes Mainland China, Hong Kong and Macau](#item-tech-news-11) ⭐️ 7.0/10
12. [MiniMax Releases H3 Image Weights With 4K Generation](#item-tech-news-12) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Claude Code Settings Exposed 2,539 Credentials in Public Repositories](https://www.ithome.com/1/024/888.htm) ⭐️ 8.0/10

Security firm Apiiro reports finding 2,539 real credentials, including database passwords and API tokens, across 1,994 GitHub repositories where Claude Code local settings were exposed. More than 100,000 such settings files had been uploaded to public repositories, and approximately 1,100 contained sensitive data. The files can record approved shell commands and may be committed with a project if Git does not ignore them. The team says it is investigating preventive measures, including built-in secret scanning; the source does not say that a fix has shipped.

telegram · zaihuapd · Nov 10, 11:20

**「Background」** Claude Code records approved shell commands in a local settings file. If that file is not excluded from Git, it can be committed to a repository along with any credentials contained in those commands.

**「Developer impact」** Developers using Claude Code should check whether local settings files are tracked or publicly exposed, particularly when approved shell commands contain credentials.

**Tags**: `#Claude Code`, `#credential exposure`, `#GitHub`, `#secret scanning`, `#AI coding tools`

---

<a id="item-tech-news-2"></a>
### [AlphaProof Code Prompts Debate Over AI-Assisted Verification](https://deepmind.google/blog/introducing-alphaproof-code/) ⭐️ 7.0/10

A DeepMind post titled “AlphaProof Code” prompted discussion about AI-assisted formal verification of software. The post’s contents were not supplied, so the project’s capabilities, results, availability, and novelty cannot be assessed from the available material.

hackernews · Google DeepMind · Nov 10, 12:11 · [Discussion](https://news.ycombinator.com/item?id=50439193)

**「Background」** Formal verification uses mathematical proofs to establish that software satisfies specified properties. The scope of the result depends on those properties: proving an implementation against a specification does not by itself establish that the specification captures every desired behavior.

**「Community discussion」** Commenters questioned whether the approach checks specifications themselves or only proves that implementations satisfy stated properties. One commenter was skeptical of an apparent zero-bug result, suggesting that the proven properties might be narrow or the theorems incorrect; the unavailable source prevents verification of that result.

**Tags**: `#formal verification`, `#AI coding agents`, `#proof assistants`, `#software correctness`

---

<a id="item-tech-news-3"></a>
### [Blender 5.3 Released With Gaussian Splat Support](https://www.blender.org/download/releases/5-3/) ⭐️ 7.0/10

Blender 5.3 is reported to add support for Gaussian splats, giving users a new option for 3D rendering workflows. The supplied material does not detail the feature’s capabilities or limitations.

hackernews · amlib · Nov 10, 16:15 · [Discussion](https://news.ycombinator.com/item?id=50442426)

**「Background」** Gaussian splatting represents a 3D scene using collections of translucent, ellipsoid-shaped primitives rather than a conventional triangle mesh. Blender treats imported Gaussian splats as point clouds, which can be manipulated with Geometry Nodes.

**「Community discussion」** One commenter who tested the beta on an M4 with a 4-million-splat scene reported that it felt fast and well integrated, though this was not a controlled benchmark. Another praised bundle support in geometry nodes for complex workflows, particularly alongside lists and closures, based on experience with alpha builds.

<details><summary>References</summary>
<ul>
<li><a href="https://www.blender.org/download/releases/5-3/">5 . 3 — Blender</a></li>

</ul>
</details>

**Tags**: `#Blender`, `#Gaussian splatting`, `#3D rendering`, `#geometry nodes`, `#open source`

---

<a id="item-tech-news-4"></a>
### [.NET 11 Runtime Update Prompts Compatibility Discussion](https://learn.microsoft.com/en-us/dotnet/core/whats-new/dotnet-11/runtime) ⭐️ 7.0/10

Microsoft has announced .NET 11, with a runtime update of interest to .NET developers. The supplied source content does not describe the runtime changes, so their scope and availability cannot be assessed from it.

hackernews · stevefan1999 · Nov 10, 12:20 · [Discussion](https://news.ycombinator.com/item?id=50439284)

**「Background」** Binary floating-point cannot represent 0.1 exactly, so converting it to the decimal type involves a choice about how much of the approximation to preserve. That distinction helps explain the compatibility concern raised about the different conversion results in .NET 10 and .NET 11.

**「Developer discussion」** One commenter warned that casting 0.1 to decimal produces 0.1 in .NET 10 but 0.1000000000000000055511151231 in .NET 11; that reported compatibility change is not independently verified in the supplied material. Another questioned what runtime async support could mean for custom async builders, while a third welcomed the prospect of friendlier stack traces.

**Tags**: `#.NET 11`, `#.NET runtime`, `#C\#`, `#backward compatibility`

---

<a id="item-tech-news-5"></a>
### [Anthropic Targets $1.4 Trillion Valuation in Planned IPO](https://www.aljazeera.com/economy/2026/11/10/anthropic-targets-1-4-trillion-valuation-in-massive-stock-market-debut?traffic_source=rss) ⭐️ 7.0/10

Anthropic, the maker of Claude, is reportedly targeting a $1.4 trillion valuation in an upcoming initial public offering. The company is looking to raise up to $64.4 billion in a stock market debut expected next week. Those figures are targets, not the result of a completed offering.

rss · Al Jazeera · Nov 10, 17:21

**「Background」** An initial public offering \(IPO\) is a process through which a company offers shares to public investors for the first time. The valuation targeted in an IPO is not necessarily the value the market will assign once trading begins.

**Tags**: `#Anthropic`, `#Artificial Intelligence`, `#IPO`, `#Technology Industry`

---

<a id="item-tech-news-6"></a>
### [Singapore’s Megaspeed Scrutinized Over Suspected Nvidia Chip Transfers](https://www.dw.com/zh/%E9%BB%84%E4%BB%81%E5%8B%8B%E9%A3%8E%E6%B3%A2%E8%B0%83%E6%9F%A5%EF%BC%9A%E9%BB%84%E4%B9%90%E4%BB%BB%E8%81%8C%E7%9A%84%E6%96%B0%E5%8A%A0%E5%9D%A1%E5%85%AC%E5%8F%B8%E4%BB%80%E4%B9%88%E6%9D%A5%E5%A4%B4%EF%BC%9F/a-79907996?maca=chi-rss-chi-all-1127-rdf) ⭐️ 7.0/10

Singapore-based Megaspeed, where Huang Le formerly served as an executive, is under renewed scrutiny over suspected transfers of Nvidia chips to China. The company’s assets reportedly rose from $33 million to $3 billion in one year, and US Commerce Department investigators spent months examining it before the investigation abruptly stopped at the end of last year. Huang, who has been accused of being a Chinese spy, was reportedly restricted from leaving Singapore. The account does not establish whether the suspected transfers occurred or why the investigation stopped.

rss · DW 中文 · Nov 10, 11:16

**「Background」** Megaspeed is a Singapore-based Nvidia customer that bought advanced AI chips. It has been accused of diverting restricted Nvidia chips to Chinese companies; the supplied accounts do not establish whether those transfers occurred.

<details><summary>References</summary>
<ul>
<li><a href="https://www.nytimes.com/2026/11/09/business/economy/nvidia-megaspeed-investigation-huang.html">U.S. Commerce Dept . Inquiry Into Megaspeed Was Halted After...</a></li>
<li><a href="https://www.cnbc.com/2026/11/10/jensen-huang-nvidia-china-ties.html">Huang affair with alleged Chinese spy complicates Nvidia China...</a></li>

</ul>
</details>

**Tags**: `#Nvidia`, `#AI chip supply chains`, `#China chip transfers`, `#US Commerce Department`, `#Singapore`

---

<a id="item-tech-news-7"></a>
### [SWE-Pair Benchmarks Coding Agents on Two-Bug Tasks](https://www.reddit.com/r/MachineLearning/comments/1xsuqem/swepair_a_codingagent_benchmark_where_every_task/) ⭐️ 7.0/10

SWE-Pair introduces 161 coding-agent tasks across 69 Python projects, each requiring fixes for two real bugs. Its creators report that DeepSeek V4.1 Flash at medium effort solved 90% of tasks at about $0.06 per solved task, while GPT-6 Luna at maximum effort solved 78% at about $0.23 per solved task. They also report that DeepSeek at maximum effort scored 88% and cost 1.7 times as much as its medium-effort configuration; the supplied post does not establish the evaluation methodology or independent verification.

reddit · r/MachineLearning · /u/heyitsdannyle · Nov 10, 18:33

**「Background」** Coding-agent benchmarks evaluate how well agents perform software development tasks. SWE-Pair focuses on a specific scenario: fixing two real bugs within a single task.

**「Availability」** Developers can access the published task dataset and agent runs, and the creators provide a Harbor command for evaluating other agents on SWE-Pair.

**Tags**: `#coding agents`, `#software engineering benchmarks`, `#bug fixing`, `#LLM evaluation`

---

<a id="item-tech-news-8"></a>
### [County Outage Forecast Reports 2.4× Baseline PR-AUC](https://www.reddit.com/r/MachineLearning/comments/1xs4hq8/forecasting_new_power_outages_per_county_hourly_2/) ⭐️ 7.0/10

A developer reports that an XGBoost model forecasting new power outages across 216 Missouri and Illinois counties achieved a 2025 held-out-year PR-AUC of 0.094, versus 0.039 for a baseline based on National Weather Service warnings and the Storm Prediction Center’s Day 1 outlook. The model predicts whether at least 5% of a county’s customers will newly lose power during a six-hour window starting two hours ahead. The reported ratio was about 2.4×, with a paired storm-day bootstrap range of 2.0–3.3×; the results are self-reported.

reddit · r/MachineLearning · /u/CarRepresentative843 · Nov 9, 21:34

**「How the test worked」** The model uses issued HRRR weather forecasts, county-specific information, current outages and neighboring counties rather than observed future weather. It was trained on 2020–2024 data, validated on 2024 and tested on 2025; the warning-based baseline was fitted on the same rows. The target excludes outages already underway.

**「Alert trade-off」** At equal alert volume, the developer reports that the model caught 30% of new outages versus 17% for the baseline, with precision of 15% versus 11%. With events occurring in just 0.5% of county-hours, the reported precision means most alerts were still false positives. An early combined test in Iowa, Indiana and Michigan found 31% caught versus 19% for the baseline; forecasts have also been saved since November 1 for a future blind test.

**Tags**: `#machine learning`, `#power outage forecasting`, `#XGBoost`, `#weather forecasting`, `#model evaluation`

---

<a id="item-tech-news-9"></a>
### [UK Cross-Party Campaign Seeks Abuse-Image Blocking Software on Devices](https://observer.co.uk/news/national/article/fight-to-block-child-sexual-abuse-images-unites-peers-and-mps-in-cross-party-campaign) ⭐️ 7.0/10

A cross-party group of UK lawmakers is proposing that phones and tablets sold in the country come with software that automatically blurs child sexual abuse images and videos, including AI-generated material, and prevents related livestreams. The proposal would also require mandatory updates for older devices. It is led by Conservative peer John Nash and Labour MP Jess Phillips; the supplied report does not explain how detection would work or whether the proposal will become law.

telegram · zaihuapd · Nov 10, 05:11

**「Earlier government commitment」** The UK government had previously committed to legislating to require Apple and Google to prevent children from taking and sharing nude images. The cross-party proposal would extend the focus to child sexual abuse images and videos on phones and tablets.

**「Potential effect」** If adopted as described, the proposal would require technology companies to preload the software on devices sold in the UK and extend it to older devices through mandatory updates.

**Tags**: `#设备端内容检测`, `#儿童安全`, `#英国科技监管`, `#AI生成内容`, `#移动设备`

---

<a id="item-tech-news-10"></a>
### [Fireworks Confirms New Attack Exposing Customer Data and Model Weights](https://finance.sina.com.cn/stock/usstock/c/2026-11-10/doc-iniyfzhx2605532.shtml) ⭐️ 7.0/10

Fireworks confirmed a new cyberattack that exposed some customers’ billing information, model weights and datasets, according to the report. The company is investigating with Palo Alto Networks’ Unit 42. Harvey said its customer data was unaffected, but the extent of exposure for other customers and end users remains unclear.

telegram · zaihuapd · Nov 10, 13:00

**「Background」** Model weights are the learned parameters that determine how an AI model behaves, while datasets can contain information used to train or evaluate it. Both can be valuable or sensitive assets for organizations using AI services.

**「Customer impact」** The report says some large customers paying millions of dollars annually are considering moving away from Fireworks, citing people familiar with the matter.

**Tags**: `#Fireworks`, `#数据泄露`, `#AI 模型权重`, `#网络安全`

---

<a id="item-tech-news-11"></a>
### [Anthropic’s Supported-Regions Policy Excludes Mainland China, Hong Kong and Macau](https://www.anthropic.com/legal/supported-regions) ⭐️ 7.0/10

Anthropic’s supported-regions policy reportedly limits Claude.ai, Claude Code, Cowork, the API and Claude models provided through cloud platforms or authorized resellers to 185 listed countries and regions. Mainland China, Hong Kong and Macau are not listed; Taiwan is included, while five regions of Ukraine are excluded. The source says the policy takes effect on November 12 but does not specify the year.

telegram · zaihuapd · Nov 10, 13:44

**「Background」** A supported-region list defines where Anthropic permits access to its products and services. The policy also considers users’ physical location and an organization’s registration, headquarters, and ownership or control—not just where an account holder is based.

**「Who is affected」** According to the report, use from an unsupported region is prohibited even for employees of a company based in a supported region. The restrictions also cover entities registered or headquartered in an unsupported region, and companies majority-owned or controlled by an entity there, regardless of where their personnel are located.

**Tags**: `#Anthropic`, `#Claude`, `#regional availability`, `#AI policy`, `#API access`

---

<a id="item-tech-news-12"></a>
### [MiniMax Releases H3 Image Weights With 4K Generation](https://huggingface.co/MiniMaxAI/MiniMax-H3-Image) ⭐️ 7.0/10

MiniMax has released the weights for MiniMax H3 Image, an image generation and editing model that supports text prompts and up to 16 reference images. The company says it can generate a 4096 × 4096 image in about 10 seconds and has also introduced a Highspeed version; the supplied source does not specify the hardware or benchmark conditions. The model is available on Hugging Face and through an API, with standard 4K generation priced at about $0.069 per image, or $0.034 during the first week after release.

telegram · zaihuapd · Nov 10, 15:39

**「Background」** An open-weight model makes its trained parameters available for others to run, whereas a hosted API provides access to the model as a service. Reference-image inputs let users guide generation or editing with existing images rather than relying on text alone.

**Tags**: `#image generation`, `#open-weight models`, `#image editing`, `#MiniMax`, `#4K images`

---