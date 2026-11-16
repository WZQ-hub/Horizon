---
layout: default
title: "Horizon Summary: 2026-11-16 (EN)"
date: 2026-11-16
lang: en
---

> From 152 items, 8 important content pieces were selected

---

**Technology News**
1. [Meta FAIR and NYU Study Tests Whether Vision Encoders Need Pretraining](#item-tech-news-1) ⭐️ 8.0/10
2. [Meituan Releases LongCat-2.5 Weights, Citing Huawei-Only Training](#item-tech-news-2) ⭐️ 8.0/10
3. [Protomaps Article Explores Self-Hosting Map Tiles](#item-tech-news-3) ⭐️ 7.0/10
4. [Hotel Chlorine Dosing Defect Coincided With Microsoft 365 Alert Failure](#item-tech-news-4) ⭐️ 7.0/10
5. [Musk Joins Open Letter Calling for Jensen Huang’s Return to Nvidia](#item-tech-news-5) ⭐️ 7.0/10
6. [US Treasury Chief Calls for Outsider to Lead Nvidia](#item-tech-news-6) ⭐️ 7.0/10
7. [cudaMemcpy Tuner Claims 5× Faster Pageable Transfers on B300](#item-tech-news-7) ⭐️ 7.0/10
8. [Judge Allows DRAM Price-Fixing Lawsuit Against Micron, Samsung and SK Hynix to Proceed](#item-tech-news-8) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Meta FAIR and NYU Study Tests Whether Vision Encoders Need Pretraining](https://www.reddit.com/r/MachineLearning/comments/1xx1k2o/meta_fair_nyu_unbundling_multimodal_vision/) ⭐️ 8.0/10

A reported Meta FAIR and NYU study trained more than 200 multimodal models to separate the effects of vision encoder pretraining, vision-only parameters, and encoder placement. The authors report that, at matched compute, separately pretrained encoders at best tied an encoder trained from scratch alongside the language model, while models without vision-only parameters needed about three times the compute to catch up. Their alternative placed vision-only weights in the language model’s first eight layers and reportedly matched a separate encoder at 1.7B–6.4B backbone sizes, with about 13% lower time to first token.

reddit · r/MachineLearning · /u/trungh98 · Nov 15, 17:38

**「What the comparison isolates」** A conventional vision encoder combines several design choices: separate pretraining, parameters used only by vision tokens, and placement before the language model. The study trained models on the same data and counted encoder pretraining against the multimodal training budget; its main comparisons used Qwen3 1.7B and 4B configurations with 0.4B parameters of vision capacity.

**「Implications for developers」** For developers designing multimodal models, the results suggest that a separate pretrained vision encoder is not the only way to achieve comparable visual question-answering performance, provided the model retains vision-only parameters. The reported evaluation covered 16 visual question-answering benchmarks at 448-pixel resolution and 12 language benchmarks, so the findings should be interpreted within that tested setup.

**Tags**: `#multimodal-llms`, `#vision-encoders`, `#model-pretraining`, `#compute-budget`

---

<a id="item-tech-news-2"></a>
### [Meituan Releases LongCat-2.5 Weights, Citing Huawei-Only Training](https://the-decoder.com/meituan-releases-a-1-6-trillion-parameter-agent-model-that-never-touched-an-nvidia-gpu/) ⭐️ 8.0/10

Meituan’s LongCat team has released the weights for LongCat-2.5 under the MIT license, one week after the model’s formal launch. Designed for agents carrying out lengthy, multistep tasks, particularly coding, the model accepts text, image and video inputs and activates approximately 48 billion parameters per token. The team says it trained the model entirely on Huawei Ascend accelerators without Nvidia GPUs, and reports a score of 88.4 on Terminal Bench v2.1, compared with 89.1 for Claude Opus 5; the supplied account provides no benchmark methodology.

telegram · zaihuapd · Nov 15, 11:08

**「Background」** Model weights are the learned parameters needed to run a trained model. LongCat-2.5 is a mixture-of-experts model, meaning it activates only a subset of its parameters for each token rather than using all of them at once.

**「Who can use it」** The MIT-licensed weights allow developers to use LongCat-2.5 commercially, including for agent applications that process multimodal inputs.

<details><summary>References</summary>
<ul>
<li><a href="https://af.net/realtime/meituan-releases-open-weight-1-6t-moe-model-longcat-2-5/">Meituan Releases Open-Weight 1.6T MoE Model LongCat-2.5</a></li>

</ul>
</details>

**Tags**: `#LongCat-2.5`, `#open-weight models`, `#AI agents`, `#Huawei Ascend`, `#AI benchmarks`

---

<a id="item-tech-news-3"></a>
### [Protomaps Article Explores Self-Hosting Map Tiles](https://bruceroettgers.eu/blog/protomaps/) ⭐️ 7.0/10

An article about Protomaps discusses self-hosting map tiles as a cheaper, easier option for developers. The article text and its technical details are not available in the supplied material, so its cost claims cannot be assessed.

hackernews · bcye · Nov 15, 19:26 · [Discussion](https://news.ycombinator.com/item?id=50509837)

**「Background」** PMTiles is a single-file archive format for tiled map data. Protomaps uses HTTP range requests to retrieve specific tiles from an archive hosted on storage such as Amazon S3, without requiring a custom tile-serving backend.

**「Community discussion」** One commenter said Protomaps made a map-based walking game affordable as a side project, while another described hosting map infrastructure behind Cloudflare R2 for privacy and access control. A third cautioned that high-resolution satellite imagery can require substantial storage, reporting that they limited an offline North American mosaic to zoom level 17 because of projected storage needs.

<details><summary>References</summary>
<ul>
<li><a href="https://protomaps.com/">Protomaps - The open source map in a file</a></li>
<li><a href="https://github.com/protomaps/PMTiles">GitHub - protomaps / PMTiles : Pyramids of map tiles in a single file on...</a></li>
<li><a href="https://awesome-repositories.com/repository/protomaps-pmtiles">PMTiles - serve map tiles from cloud storage | Awesome Repos</a></li>

</ul>
</details>

**Tags**: `#Protomaps`, `#map tiles`, `#self-hosting`, `#geospatial infrastructure`

---

<a id="item-tech-news-4"></a>
### [Hotel Chlorine Dosing Defect Coincided With Microsoft 365 Alert Failure](https://www1.wdr.de/nrw/rheinland/rhein-erft-kreis/technischer-defekt-chlor-phantasialand-100.html) ⭐️ 7.0/10

A reported chlorine-dosing defect at a hotel coincided with a failure of its Microsoft 365 email monitoring alert. A commenter translating the German report said 15 guests experienced airway irritation and four were taken to hospital. The source article was not available in the supplied material, and the evidence does not establish that the Microsoft 365 failure caused the dosing defect.

hackernews · DeepLogin · Nov 15, 18:36 · [Discussion](https://news.ycombinator.com/item?id=50509411)

**「Background」** Chlorination systems use dosing controls to regulate chlorine levels; monitoring and alerts can warn operators when those controls malfunction. Separately, WDR reported disruption to Microsoft services including Outlook and Teams, though the available report does not establish whether it was the same disruption involved in the hotel incident.

**「Community discussion」** Commenters argued that hazardous chemical monitoring should not rely solely on email alerts and should have redundant safeguards. One commenter who operates a chlorination system said dosing systems can fail in ways that cause excessive chlorine dispensing, making independent safety checks important.

<details><summary>References</summary>
<ul>
<li><a href="https://www1.wdr.de/nrw/microsoft-stoerung-teams-outlook-100.html">Microsoft -Störung: Probleme bei Teams und Outlook</a></li>

</ul>
</details>

**Tags**: `#safety-critical systems`, `#cloud reliability`, `#monitoring and alerting`, `#industrial control systems`

---

<a id="item-tech-news-5"></a>
### [Musk Joins Open Letter Calling for Jensen Huang’s Return to Nvidia](https://www.theguardian.com/technology/2026/nov/16/elon-musk-tech-execs-open-letter-jensen-huang-return-nvidia-ceo) ⭐️ 7.0/10

Elon Musk and other technology executives are among more than 158,000 signatories calling for Nvidia to reinstate Jensen Huang as CEO, days after his resignation. The letter asks the board to bring Huang back while an independent investigation establishes the facts. The Guardian reports that his departure followed revelations of an affair with a suspected Chinese spy, but the supplied excerpt does not provide further details of the allegations.

rss · The Guardian World · Nov 16, 01:01

**「Background」** Huang resigned as Nvidia’s CEO days before the letter, following revelations of an affair with a suspected Chinese spy, according to the Guardian. The supplied excerpt does not detail the allegations or the proposed investigation.

**Tags**: `#Nvidia`, `#Jensen Huang`, `#Corporate leadership`, `#AI hardware`

---

<a id="item-tech-news-6"></a>
### [US Treasury Chief Calls for Outsider to Lead Nvidia](https://www.aljazeera.com/news/2026/11/15/us-treasury-chief-calls-for-outsider-to-lead-embattled-tech-firm-nvidia?traffic_source=rss) ⭐️ 7.0/10

US Treasury chief Scott Bessent called for an outsider to lead Nvidia, according to Al Jazeera. He also gave the company’s board 10 days to demonstrate compliance with US export controls. The supplied report does not explain the basis for his demands or provide further details about the compliance concerns.

rss · Al Jazeera · Nov 15, 21:47

**「Background」** CNBC reported that Bessent’s call for an outside CEO followed Jensen Huang’s resignation from Nvidia.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cnbc.com/2026/11/15/bessent-nvidia-ceo-lutnick-megaspeed.html">Bessent calls for ‘dramatic shakeup’ at Nvidia , urges outside CEO</a></li>

</ul>
</details>

**Tags**: `#Nvidia`, `#US export controls`, `#corporate governance`, `#AI hardware`

---

<a id="item-tech-news-7"></a>
### [cudaMemcpy Tuner Claims 5× Faster Pageable Transfers on B300](https://www.reddit.com/r/MachineLearning/comments/1xx2n25/making_cudamemcpy_5x_faster_on_a_b300_p/) ⭐️ 7.0/10

A developer has published cudamemcpy-tuner, a tool intended to speed up pageable CPU-to-GPU transfers. In a PyTorch benchmark copying a 1 GiB tensor to an NVIDIA B300, the developer reports throughput rising from 10.2 GB/s to 51.5 GB/s when running the script through \`cmt tune\`. The result is a single author-reported example; the supplied material does not establish independent validation or broader applicability.

reddit · r/MachineLearning · /u/makneeee · Nov 15, 18:20

**「Background」** Pageable host memory can be moved by the operating system, unlike pinned memory, which remains resident. CUDA applications use memory-copy operations to transfer data between host memory and GPU memory.

**Tags**: `#CUDA`, `#GPU memory transfers`, `#performance optimization`, `#PyTorch`, `#B300`

---

<a id="item-tech-news-8"></a>
### [Judge Allows DRAM Price-Fixing Lawsuit Against Micron, Samsung and SK Hynix to Proceed](https://www.tomshardware.com/tech-industry/big-tech/judge-denies-motion-to-dismiss-dram-price-fixing-lawsuit-against-micron-samsung-and-sk-hynix-says-chipmakers-acted-like-hawks-flying-in-formation-finds-evidence-of-dram-collusion-plausible-after-500-percent-price-surge) ⭐️ 7.0/10

U.S. Judge Noël Wise denied Micron, Samsung and SK Hynix’s motion to dismiss a class-action lawsuit alleging DRAM price fixing, allowing the case to proceed. The 17 plaintiffs, comprising individuals and small businesses, allege that the companies took four parallel actions to restrict DRAM supply within a year and that prices rose by as much as 500%. Wise found that the plaintiffs had presented new evidence supporting a plausible claim, but the ruling does not establish that the companies fixed prices. The companies must respond by December 7, and a case management conference is scheduled for January 2027.

telegram · zaihuapd · Nov 15, 16:39

**「Background」** DRAM is the memory used in computers and other devices to hold data while they operate. The lawsuit alleges that the three manufacturers coordinated to restrict its supply; a decision allowing the case to proceed is not a finding that they did so.

**Tags**: `#DRAM`, `#半导体产业`, `#反垄断诉讼`, `#内存价格`

---