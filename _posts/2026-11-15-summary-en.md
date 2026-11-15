---
layout: default
title: "Horizon Summary: 2026-11-15 (EN)"
date: 2026-11-15
lang: en
---

> From 138 items, 12 important content pieces were selected

---

**Technology News**
1. [Project Zero disclosure deadlines reportedly moving from 90 to 30 days](#item-tech-news-1) ⭐️ 8.0/10
2. [Italy Fines Meta €805 Million Over Facebook Photo Access](#item-tech-news-2) ⭐️ 8.0/10
3. [SpaceX Reportedly Catches Starship After Flight 15](#item-tech-news-3) ⭐️ 7.0/10
4. [Lovable-Built Apps Reportedly Expose Passport Details and Private Messages](#item-tech-news-4) ⭐️ 7.0/10
5. [PyPI launches redesigned project pages with clearer security signals](#item-tech-news-5) ⭐️ 7.0/10
6. [EFF Questions Tech Companies’ Changing Concept of Privacy](#item-tech-news-6) ⭐️ 7.0/10
7. [Microsoft Says Global Outage Lasting Over 24 Hours Has Ended](#item-tech-news-7) ⭐️ 7.0/10
8. [TimeCues Studio offers open-source, beat-aligned music annotation](#item-tech-news-8) ⭐️ 7.0/10
9. [OpenAI Reportedly Disbands Dedicated Robotics Team](#item-tech-news-9) ⭐️ 7.0/10
10. [Cloudflare Open-Sources Kitesurf Browser for AI Agents](#item-tech-news-10) ⭐️ 7.0/10
11. [Tesla Cybercab Reportedly Requires $299 Monthly Autonomy Subscription](#item-tech-news-11) ⭐️ 7.0/10
12. [FAA Ground Stop Linked to Router Problem After Fiber Upgrade](#item-tech-news-12) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Project Zero disclosure deadlines reportedly moving from 90 to 30 days](https://projectzero.google/2026/11/disclosure-policy.html) ⭐️ 8.0/10

A community comment reports that Project Zero will disclose vulnerabilities 90 days after notifying the affected vendor under a policy called “Full 90.” The comment says the deadline will fall to 60 days on February 2, 2027, and 30 days on January 3, 2028. The linked policy text was not supplied, so the timeline could not be independently verified here.

hackernews · hacb · Nov 14, 11:13 · [Discussion](https://news.ycombinator.com/item?id=50496051)

**「Background」** Project Zero previously trialed a “Full 90” policy in 2020, disclosing vulnerabilities 90 days after reporting regardless of when they were fixed. Its 2021 trial added a 30-day period intended to give users time to adopt patches.

**「Community discussion」** One commenter argued that immediate disclosure would better pressure companies to fix vulnerabilities, while another suggested Ubuntu would need substantially more time than the proposed deadlines.

<details><summary>References</summary>
<ul>
<li><a href="https://projectzero.google/2021/04/policy-and-disclosure-2021-edition.html">Policy and Disclosure : 2021 Edition - Project Zero</a></li>
<li><a href="https://projectzero.google/2020/01/policy-and-disclosure-2020-edition.html">Policy and Disclosure : 2020 Edition - Project Zero</a></li>

</ul>
</details>

**Tags**: `#vulnerability disclosure`, `#Project Zero`, `#software security`, `#patch management`

---

<a id="item-tech-news-2"></a>
### [Italy Fines Meta €805 Million Over Facebook Photo Access](https://www.garanteprivacy.it/home/docweb/-/docweb-display/docweb/10321080) ⭐️ 8.0/10

Italy’s privacy regulator fined Meta €805 million over a Facebook Android photo recommendation feature that accessed the photos, videos and metadata of about 20 million Italian users without specific consent. The feature, introduced in 2023, was enabled by default and used a broadly worded permission prompt. The regulator ordered Meta to turn it off by default and obtain separate consent within 60 days; otherwise, it must not enable the feature for users who have not validly authorized it.

telegram · zaihuapd · Nov 14, 14:37

**「Background」** Facebook introduced the photo recommendation feature in 2023. The reported privacy issue concerns whether users were adequately informed and gave specific consent, rather than establishing that Meta bypassed Android’s device-permission system.

**「Community discussion」** Commenters questioned how Facebook could access photos without consent, with one pointing out that users must grant device-level permission for the feature to work. The supplied report does not explain the relationship between Android’s permission prompt and the regulator’s requirement for specific consent.

**Tags**: `#Meta`, `#data privacy`, `#Italy`, `#Android`, `#regulation`

---

<a id="item-tech-news-3"></a>
### [SpaceX Reportedly Catches Starship After Flight 15](https://www.spacex.com/launches/starship-flight-15) ⭐️ 7.0/10

SpaceX reportedly caught the Starship spacecraft with launch-tower arms at the end of Flight 15, following its return from orbit. The flight did not achieve the planned catch of both vehicles: the booster aborted its return and exploded after a controlled splashdown in the Gulf of Mexico; the cause was not disclosed. A supplied report says the spacecraft deployed 26 Starlink V3 satellites, three of which carried cameras to inspect its heat-shield tiles.

hackernews · ls612 · Nov 14, 21:22 · [Discussion](https://news.ycombinator.com/item?id=50500963)

**「Background」** Starship consists of a Super Heavy booster and an upper-stage spacecraft, both intended for reuse. SpaceX had planned to catch both stages with the launch tower’s mechanical arms on Flight 15, but the booster’s catch attempt was aborted and it was diverted to the Gulf of Mexico.

**「Community discussion」** Commenters saw the catch as a step toward reusability, but one argued that the heat shield must hold up and that SpaceX still needs to catch and refly the same vehicles before substantially cheaper orbital payload delivery can be demonstrated. Another noted that Starship’s eventual mass fraction to orbit remains unclear.

**Tags**: `#SpaceX`, `#Starship`, `#reusable spacecraft`, `#spaceflight engineering`

---

<a id="item-tech-news-4"></a>
### [Lovable-Built Apps Reportedly Expose Passport Details and Private Messages](https://www.crissyfield.de/research/lovable-en/) ⭐️ 7.0/10

A research post reports that apps built with Lovable exposed passport details and more than 200,000 private messages. The research details were not supplied, so the scope and circumstances of the exposure cannot be independently assessed from the available material.

hackernews · armcat · Nov 14, 17:43 · [Discussion](https://news.ycombinator.com/item?id=50499017)

**「Background」** Row-level security controls which database records a user can access. A commenter identifying as Lovable’s head of security attributed the exposures in these apps to insufficient row-level security.

**「Security defaults debated」** A commenter identifying as Lovable’s head of security attributed the exposure to insufficient row-level security and said Lovable automatically scans apps before publication, with free tools to help fix findings. Other commenters argued for safer database defaults; one also questioned Supabase’s role, though their claims about its defaults were not independently verified in the supplied material.

**Tags**: `#AI app builders`, `#data exposure`, `#row-level security`, `#Supabase`, `#application security`

---

<a id="item-tech-news-5"></a>
### [PyPI launches redesigned project pages with clearer security signals](https://blog.pypi.org/posts/2026-11-06-ui-updates-complete/) ⭐️ 7.0/10

PyPI’s redesigned project pages are now live, making security and provenance information more visible to people evaluating Python packages. The available source details do not establish the full scope of the redesign.

hackernews · rbanffy · Nov 14, 15:40 · [Discussion](https://news.ycombinator.com/item?id=50497892)

**「Background」** PyPI announced the interface changes in July, saying they would be staged on TestPyPI and deployed to production in phases. The plan focused on making security signals and package details easier to find.

**「Community discussion」** Commenters welcomed greater visibility for provenance but disagreed about reliance on major cloud and CI providers: one worried about lock-in, while another hoped for broader support for keyless signing. Another commenter said trusted publishing still lacks reusable workflow support, and a further commenter cautioned that provenance can help detect some compromised packages but does not identify malicious projects.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.pypi.org/posts/2026-07-22-ui-updates/">Planned Updates to the PyPI User Interface</a></li>

</ul>
</details>

**Tags**: `#PyPI`, `#Python packaging`, `#software supply chain security`, `#package provenance`, `#trusted publishing`

---

<a id="item-tech-news-6"></a>
### [EFF Questions Tech Companies’ Changing Concept of Privacy](https://www.eff.org/deeplinks/2026/11/tech-companies-are-trying-shift-entire-concept-privacy-again) ⭐️ 7.0/10

An Electronic Frontier Foundation article challenges technology companies’ changing conception of privacy. The article’s text was not supplied, so its specific claims and any proposed changes cannot be assessed.

hackernews · gslin · Nov 14, 12:45 · [Discussion](https://news.ycombinator.com/item?id=50496602)

**「Background」** AI transcription can turn spoken conversations into text, including in meetings and accessibility tools. As one commenter noted, a transcription system could process speech locally without saving or exporting it, though the same system could also be designed to retain the text.

**「Community discussion」** One commenter said AI notetakers record and upload even one-on-one workplace conversations, and questioned whether employees can realistically opt out. Another argued that live transcription could be transformative for deaf and nearly deaf people, while noting that even local systems could be modified to retain data.

**Tags**: `#digital-privacy`, `#ai-transcription`, `#workplace-surveillance`, `#accessibility`, `#data-retention`

---

<a id="item-tech-news-7"></a>
### [Microsoft Says Global Outage Lasting Over 24 Hours Has Ended](https://www.dw.com/zh/%E5%81%9C%E6%91%86%E8%B6%85%E8%BF%8724%E5%B0%8F%E6%97%B6%EF%BC%9A%E5%BE%AE%E8%BD%AF%E5%85%A8%E7%90%83%E5%A4%A7%E5%AE%95%E6%9C%BA%E7%BB%93%E6%9D%9F/a-79948266?maca=chi-rss-chi-all-1127-rdf) ⭐️ 7.0/10

Microsoft announced that a global service outage lasting more than 24 hours had ended. The disruption affected applications including Teams, Outlook, and Copilot, and prevented government agencies and businesses in multiple countries from sending or receiving email or holding online meetings. The source did not provide a technical cause.

rss · DW 中文 · Nov 14, 13:02

**「Background」** Organizations use Microsoft’s online services for routine communications, including email through Outlook and meetings through Teams. An outage affecting both can disrupt these activities at the same time.

**「Healthcare disruption」** The outage forced the UK National Health Service to switch to paper records.

**Tags**: `#Microsoft`, `#Service outages`, `#Cloud services`, `#Microsoft Teams`, `#Outlook`

---

<a id="item-tech-news-8"></a>
### [TimeCues Studio offers open-source, beat-aligned music annotation](https://www.reddit.com/r/MachineLearning/comments/1xwh3mw/acm_multimedia_2026_timecues_studio_a_free/) ⭐️ 7.0/10

TimeCues Studio is a free, MIT-licensed web app for annotating music structure on a beat-locked timeline and comparing analysis algorithms against those labels. Its creator says it displays separated stems, a spectrogram and a three-band waveform, and scores detectors such as allin1 and MSAF against user annotations. Individuals or teams can export annotations as Audacity labels, MIDI or JSON; the app can be run with Docker Compose or tried in a demo without signing in.

reddit · r/MachineLearning · /u/SapirCa · Nov 14, 23:59

**「Background」** Music-analysis models need labeled examples for training and evaluation, but annotated data is scarce for many tasks. Music annotations can identify positions, segments, or loops that algorithms are expected to detect.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2609.10338">[2609.10338] TimeCues Studio: A Workspace for Music ...</a></li>
<li><a href="https://www.emergentmind.com/papers/2609.10338">TimeCues Studio: A Workspace for Music Annotation and ...</a></li>

</ul>
</details>

**Tags**: `#music structure annotation`, `#music information retrieval`, `#open-source tools`, `#audio machine learning`

---

<a id="item-tech-news-9"></a>
### [OpenAI Reportedly Disbands Dedicated Robotics Team](https://fortune.com/2026/11/13/openai-disbands-robotics-team-as-its-general-models-start-running-robots/) ⭐️ 7.0/10

OpenAI has disbanded its dedicated robotics team and reassigned its researchers to broader research teams, according to a Telegram post citing Fortune. The post says OpenAI considers robotics central to its long-term vision and attributes the change to general-purpose models, including one it calls GPT-6 Astra, being able to control robots directly. It also claims OpenAI is still developing a humanoid robot with a goal of demonstrating it publicly in 2027; the short secondhand account provides no technical evidence for those claims.

telegram · zaihuapd · Nov 14, 04:00

**「Background」** OpenAI previously disbanded a robotics team in 2020, then rebuilt its robotics efforts in 2024 and partnered with humanoid robot developer Figure, according to the source. That partnership ended in February 2025.

**Tags**: `#OpenAI`, `#Robotics`, `#General-purpose AI models`, `#AI industry`

---

<a id="item-tech-news-10"></a>
### [Cloudflare Open-Sources Kitesurf Browser for AI Agents](https://www.phoronix.com/news/Cloudflare-Kitesurf-Open-Source) ⭐️ 7.0/10

Cloudflare has open-sourced Kitesurf, a stateless browser for AI agents, under the Apache 2.0 license. Built on Cloudflare Workers, it parses HTML, handles CSS, and executes JavaScript without browser containers; the code is available on GitHub. Cloudflare says it aims to use less CPU and memory than Chromium and scale on demand across the Workers network, but the source provides no benchmarks to substantiate the resource comparison.

telegram · zaihuapd · Nov 14, 09:33

**「Background」** AI agents can use browser engines to interact with web pages, including pages that rely on JavaScript. Cloudflare describes Kitesurf as an experimental browser engine that can also be run locally or deployed on Workers.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.cloudflare.com/kitesurf-open-source/">Kitesurf is now open source | Cloudflare Blog</a></li>

</ul>
</details>

**Tags**: `#AI agents`, `#browser automation`, `#Cloudflare Workers`, `#open source`

---

<a id="item-tech-news-11"></a>
### [Tesla Cybercab Reportedly Requires $299 Monthly Autonomy Subscription](https://www.tesla.com/configurator/api/v4/terms?category=autonomy_subs&amp;amp;locale=en_US&amp;amp;model=cc&amp;amp;saleType=Sale) ⭐️ 7.0/10

Tesla&\#x27;s reported Cybercab subscription terms say owners must pay $299 per month for autonomous driving or the vehicle cannot operate, on top of a stated vehicle price of $29,990. Tesla could change the subscription price with one month&\#x27;s notice and suspend or cancel it for nonpayment or prohibited use; three warnings would disable autonomous driving for one week. The report says Cybercab is restricted to designated operating areas and cannot be connected to ride-hailing, delivery or rental platforms without authorization. The agreement text was not supplied, so these reported terms could not be independently verified.

telegram · zaihuapd · Nov 15, 01:10

**「Background」** According to Electrek, the Cybercab and the Model Y used for Robotaxi service share Tesla’s AI4 hardware and run the same self-driving software. Tesla’s FSD system for ordinary owners, by contrast, still requires human supervision.

**「Owner restrictions」** If the reported terms apply, owners would face an ongoing payment requirement to operate the vehicle and would need authorization before using it on third-party ride-hailing, delivery or rental platforms.

**Tags**: `#特斯拉 Cybercab`, `#自动驾驶`, `#汽车订阅`, `#车主权利`, `#Robotaxi`

---

<a id="item-tech-news-12"></a>
### [FAA Ground Stop Linked to Router Problem After Fiber Upgrade](https://www.theverge.com/transportation/1033898/faa-ground-stop-sean-duffy-faa-copper-wire) ⭐️ 7.0/10

U.S. Transportation Secretary Sean Duffy said a router problem following a copper-to-fiber upgrade at a remote facility disrupted FAA radar signals and aircraft communications, prompting a nationwide ground stop that affected thousands of flights. Duffy said the newly installed router sent more than 1,000 connection requests to other routers every four to five seconds. The root cause remains unclear; he cited possible hardware failure, misconfiguration, or an error by contractor L3Harris.

telegram · zaihuapd · Nov 15, 02:10

**「Background」** FAA communications infrastructure includes legacy copper links that are being replaced with fiber-optic connections. Routers direct network traffic between connected systems, so a malfunctioning router can disrupt communications beyond the facility where it is installed.

**Tags**: `#FAA`, `#aviation infrastructure`, `#network routing`, `#system outages`, `#infrastructure modernization`

---