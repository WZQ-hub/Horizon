---
layout: default
title: "Horizon Summary: 2026-11-16 (ZH)"
date: 2026-11-16
lang: zh
---

> 从 152 条内容中筛选出 8 条重要资讯。

---

**科技新闻**
1. [Meta FAIR 与 NYU 研究：视觉编码器预训练并非必需](#item-tech-news-1) ⭐️ 8.0/10
2. [美团开放 LongCat-2.5 权重，称全程使用华为升腾训练](#item-tech-news-2) ⭐️ 8.0/10
3. [Protomaps：自托管地图瓦片的成本与实践](#item-tech-news-3) ⭐️ 7.0/10
4. [酒店加氯设备故障，Microsoft 365 邮件警报亦失效](#item-tech-news-4) ⭐️ 7.0/10
5. [马斯克等人联名呼吁英伟达让黄仁勋复任](#item-tech-news-5) ⭐️ 7.0/10
6. [美国财长呼吁外部人士领导 Nvidia](#item-tech-news-6) ⭐️ 7.0/10
7. [cudaMemcpy 调优工具报告 B300 传输速度提升](#item-tech-news-7) ⭐️ 7.0/10
8. [美法官允许 DRAM 价格操纵案继续审理](#item-tech-news-8) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [Meta FAIR 与 NYU 研究：视觉编码器预训练并非必需](https://www.reddit.com/r/MachineLearning/comments/1xx1k2o/meta_fair_nyu_unbundling_multimodal_vision/) ⭐️ 8.0/10

据研究作者介绍，Meta FAIR 与纽约大学的一项研究训练了 200 多个多模态大语言模型，比较视觉编码器的预训练、视觉专用参数和编码器位置。研究称，在相同计算预算下，单独预训练视觉编码器至多与从头联合训练持平；而没有视觉专用参数的模型在测试的各个规模上都落后，追平约需 3 倍计算量。作者还称，将视觉专用权重加入语言模型前 8 层，可在部分模型规模上达到独立编码器的视觉问答表现，首词元生成时间约低 13%。这些是作者报告的特定实验结果，不代表所有多模态架构都无需视觉编码器预训练。

reddit · r/MachineLearning · /u/trungh98 · 11月15日 17:38

**「实验背景」** 常见视觉编码器将三种设计选择捆绑在一起：单独预训练、使用仅供视觉词元处理的参数，以及将编码器置于语言模型之前。研究尝试分别检验这些选择：模型使用相同数据从头训练，编码器预训练也计入总计算预算；评估包括 16 项视觉问答基准和 12 项语言基准。

**「对模型设计的启示」** 对受计算预算约束的多模态模型开发者而言，这项研究提供了一种值得测试的方案：省去单独的视觉编码器预训练，但保留视觉专用参数。作者报告，在 1.7B 模型中，把这些参数放在前 8 层的视觉问答表现优于放在最后 8 层，因此参数位置也需要纳入设计比较。

**标签**: `#multimodal-llms`, `#vision-encoders`, `#model-pretraining`, `#compute-budget`

---

<a id="item-tech-news-2"></a>
### [美团开放 LongCat-2.5 权重，称全程使用华为升腾训练](https://the-decoder.com/meituan-releases-a-1-6-trillion-parameter-agent-model-that-never-touched-an-nvidia-gpu/) ⭐️ 8.0/10

美团 LongCat 团队在模型正式发布一周后公布了 LongCat-2.5 权重，采用允许商用的 MIT 许可证。该多模态模型面向执行长流程任务、尤其是编程任务的智能体，支持文本、图像和视频输入，每个 token 约激活 480 亿参数。团队称模型训练全程使用华为升腾加速卡，未使用英伟达 GPU；其公布的 Terminal Bench v2.1 得分为 88.4，略低于 Claude Opus 5 的 89.1，但所提供材料未说明测试方法。

telegram · zaihuapd · 11月15日 11:08

**「背景」** 模型权重是训练过程中得到的参数，公开权重让使用者可以自行部署模型；MIT 许可证则允许商业使用。LongCat-2.5 面向智能体任务，旨在让模型执行较长的多步骤任务，而不只是回答单次提问。

**标签**: `#LongCat-2.5`, `#open-weight models`, `#AI agents`, `#Huawei Ascend`, `#AI benchmarks`

---

<a id="item-tech-news-3"></a>
### [Protomaps：自托管地图瓦片的成本与实践](https://bruceroettgers.eu/blog/protomaps/) ⭐️ 7.0/10

一篇关于 Protomaps 的文章讨论了自托管地图瓦片，面向希望自行管理地图基础设施的开发者。文章标题称这种方式已变得便宜且简单，但现有材料未提供具体技术方案或成本数据。

hackernews · bcye · 11月15日 19:26 · [社区讨论](https://news.ycombinator.com/item?id=50509837)

**「背景」** PMTiles 是一种将地图瓦片打包进单个文件的归档格式，可存放在 S3 等对象存储平台上。客户端可以通过 HTTP 范围请求获取所需的瓦片，无须下载整个文件，也不需要专门的瓦片服务后端。

**「社区讨论」** 一位评论者称，Protomaps 让其街道地图游戏的地图渲染费用变得可负担；另一位称其团队使用 Cloudflare R2 托管地图，以控制隐私和访问权限。也有开发者提醒，高分辨率卫星影像的存储需求会随缩放级别迅速增长；另有评论者推荐 OpenFreeMap 作为类似项目。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://protomaps.com/">Protomaps - The open source map in a file</a></li>
<li><a href="https://github.com/protomaps/PMTiles">GitHub - protomaps / PMTiles : Pyramids of map tiles in a single file on...</a></li>

</ul>
</details>

**标签**: `#Protomaps`, `#map tiles`, `#self-hosting`, `#geospatial infrastructure`

---

<a id="item-tech-news-4"></a>
### [酒店加氯设备故障，Microsoft 365 邮件警报亦失效](https://www1.wdr.de/nrw/rheinland/rhein-erft-kreis/technischer-defekt-chlor-phantasialand-100.html) ⭐️ 7.0/10

据一名评论者对德文报道的概述，一家酒店的加氯设备出现投加过量故障，同时监控系统通过 Microsoft 365 发送的邮件警报未能送达。该评论者称，先后有 15 名住客出现呼吸道刺激症状，其中 4 人被送往医院；原文未随素材提供，这些细节及 Microsoft 365 故障的作用无法独立核实。现有信息不足以认定邮件服务故障直接导致了事件。

hackernews · DeepLogin · 11月15日 18:36 · [社区讨论](https://news.ycombinator.com/item?id=50509411)

**「背景」** 加氯系统通过投加含氯药剂控制水质，而监控和告警可以是独立于投加设备的环节。邮件告警未送达本身并不意味着邮件服务造成了投加设备故障。

**「社区讨论」** 多名评论者认为，危险化学品监控不应仅依赖电子邮件，应配备冗余警报或人工复核。一名自称运营闭环加氯系统的评论者还指出，传感器读数偏低可能导致系统过量投加，因此需要同时防范氯含量过高和过低。

**标签**: `#safety-critical systems`, `#cloud reliability`, `#monitoring and alerting`, `#industrial control systems`

---

<a id="item-tech-news-5"></a>
### [马斯克等人联名呼吁英伟达让黄仁勋复任](https://www.theguardian.com/technology/2026/nov/16/elon-musk-tech-execs-open-letter-jensen-huang-return-nvidia-ceo) ⭐️ 7.0/10

黄仁勋辞去英伟达首席执行官职务数日后，埃隆·马斯克及其他科技界高管等超过 15.8 万人签署公开信，呼吁董事会让他复任。公开信要求在独立调查厘清事实期间让黄仁勋回归。《卫报》报道称，他的离职发生在其与一名涉嫌为中国间谍的人士有婚外情的消息曝光之后；所提供的报道摘录未详述相关指控或调查情况。

rss · The Guardian World · 11月16日 01:01

**「背景」** 据《卫报》报道，黄仁勋在被曝与一名涉嫌为中国间谍的人有婚外情后辞去了英伟达首席执行官职务。公开信要求在独立调查查明事实期间恢复他的职务；报道摘录未提供有关指控或调查的更多细节。

**标签**: `#Nvidia`, `#Jensen Huang`, `#Corporate leadership`, `#AI hardware`

---

<a id="item-tech-news-6"></a>
### [美国财长呼吁外部人士领导 Nvidia](https://www.aljazeera.com/news/2026/11/15/us-treasury-chief-calls-for-outsider-to-lead-embattled-tech-firm-nvidia?traffic_source=rss) ⭐️ 7.0/10

据半岛电视台报道，美国财政部长斯科特·贝森特呼吁由外部人士领导 Nvidia，并要求其董事会在 10 天内证明公司遵守美国出口管制规定。现有材料未说明这一要求的具体依据，也未提供 Nvidia 的回应。

rss · Al Jazeera · 11月15日 21:47

**「背景」** 据 CNBC 报道，贝森特提出这一要求之前，英伟达首席执行官黄仁勋已辞职。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cnbc.com/2026/11/15/bessent-nvidia-ceo-lutnick-megaspeed.html">Bessent calls for ‘dramatic shakeup’ at Nvidia , urges outside CEO</a></li>

</ul>
</details>

**标签**: `#Nvidia`, `#US export controls`, `#corporate governance`, `#AI hardware`

---

<a id="item-tech-news-7"></a>
### [cudaMemcpy 调优工具报告 B300 传输速度提升](https://www.reddit.com/r/MachineLearning/comments/1xx2n25/making_cudamemcpy_5x_faster_on_a_b300_p/) ⭐️ 7.0/10

一名开发者发布了 cudaMemcpy 调优工具 cudamemcpy-tuner，用于加速可分页内存传输。作者报告，在 B300 上运行的 PyTorch 测试中，使用“cmt tune”后，1 GB 张量从 CPU 传到 GPU 的吞吐量从 10.2 GB/s 升至 51.5 GB/s，约为原来的 5 倍。这是作者报告的单个测试结果；所提供的内容没有说明其加速机制、适用范围或独立验证情况。

reddit · r/MachineLearning · /u/makneeee · 11月15日 18:20

**「背景」** cudaMemcpy 用于在 CPU 主机和 GPU 设备等位置之间复制数据。可分页内存是操作系统可以换出的主机内存，与锁页内存不同。

**标签**: `#CUDA`, `#GPU memory transfers`, `#performance optimization`, `#PyTorch`, `#B300`

---

<a id="item-tech-news-8"></a>
### [美法官允许 DRAM 价格操纵案继续审理](https://www.tomshardware.com/tech-industry/big-tech/judge-denies-motion-to-dismiss-dram-price-fixing-lawsuit-against-micron-samsung-and-sk-hynix-says-chipmakers-acted-like-hawks-flying-in-formation-finds-evidence-of-dram-collusion-plausible-after-500-percent-price-surge) ⭐️ 7.0/10

美国法官 Noël Wise 驳回了美光、三星和 SK 海力士要求撤销 DRAM 价格操纵集体诉讼的动议，允许案件继续审理。17 名个人及小企业原告指控，三家厂商一年内四次采取平行行动限制 DRAM 供应，价格涨幅最高达 500%；法官认为原告提出了新证据，并将厂商的同步行为比作“编队飞行”。三家公司须在 12 月 7 日前回应，案件管理会议定于 2027 年 1 月；驳回撤诉动议并不等于认定厂商存在价格操纵。

telegram · zaihuapd · 11月15日 16:39

**「背景」** 撤诉动议是被告请求法院在案件进一步审理前终止诉讼的程序。驳回动议意味着案件可以继续推进，并不等于法院已经认定三家厂商操纵价格。

**标签**: `#DRAM`, `#半导体产业`, `#反垄断诉讼`, `#内存价格`

---