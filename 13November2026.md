# Daily Tech & AI Briefing — 13 November 2026

**Biggest story:** **Jensen Huang has resigned as CEO and board member of Nvidia**, effective immediately. CFO **Colette Kress** is interim CEO. Nvidia supplies most of the chips that AI runs on, and it now has no permanent leader.

> Notes: Covers roughly 9–13 November 2026. Benchmarks are vendor-reported unless stated. Several primary pages (Nvidia newsroom, SEC EDGAR, Al Jazeera) could not be opened from this environment, so cross-checks rely on search-indexed coverage from several outlets.

---

## 1. Jensen Huang resigns as Nvidia CEO; CFO Colette Kress is interim CEO (Nov 11–12)

Nvidia announced a **CEO transition** in a press release and an **SEC 8-K**. **Jensen Huang** resigned as president, CEO and director, effective immediately, ending a 33-year run. The 8-K dates the resignation to Nov 11. CFO **Colette Kress** becomes **interim CEO** and stays CFO. Longtime director **Harvey C. Jones** becomes Nvidia's **first-ever board chair**. The board will look at internal and external candidates for a permanent CEO. Nvidia's filings give **no reason**. CNBC and Yahoo Finance report the exit followed **reports of extramarital affairs**, one allegedly with a woman US officials believe is a **Chinese intelligence asset**. This came after Nvidia opened an internal probe on Nov 9, and the stock fell more than 4% that day.

- **Why this matters for you (developer/entrepreneur):** Nvidia's products (CUDA, GPU allocation, Blackwell/Rubin roadmaps) aren't changing yet, but a leadership gap at the main AI chip supplier adds risk to **GPU pricing, supply and US–China export policy**. Keep your inference stack portable across chips.
- **Business/project idea:** A **"compute portability" toolkit or consultancy**. Package workloads so they can move between Nvidia GPUs, Google TPUs, AMD and Trainium (for example vLLM/JAX/Triton deployment templates plus a cost dashboard). Sell it to startups that want a hedge against supply or price shocks.
- Sources: [Nvidia IR press release](https://investor.nvidia.com/news/press-release-details/2026/NVIDIA-Announces-CEO-Transition/) · [SEC 8-K](https://www.sec.gov/Archives/edgar/data/0001045810/000104581026000082/nvda-20261111.htm) · [CNBC](https://www.cnbc.com/2026/11/12/colette-kress-nvidia-cfo-interim-ceo-candidate.html) · [Benzinga](https://www.benzinga.com/markets/tech/26/11/63186620/nvidia-ceo-jensen-huang-resigns-cfo-collette-kress-in-as-interim-ceo) · [Al Jazeera](https://www.aljazeera.com/news/2026/11/12/why-did-nvidia-ceo-jensen-huang-resign-and-who-is-colette-kress)

## 2. Google launches Gemini 4 Hydrogen and retires the "Flash" name (Nov 12)

**Gemini 4 Hydrogen** replaces **Gemini 3.8 Flash** as Google's fast, cheap tier. It now powers **Search** and the **Gemini app**, free users included. Google says it finishes tasks **2.5x faster than 3.8 Flash**, scores **57% on Terminal-Bench 4.1** (vs 18.2% for 3.8 Flash; Sonnet 5.5 is reported at 63.9%), and makes **5x fewer fabricated claims**. Google also says it beats Gemini 4 Argon on the Artificial Analysis index. API pricing is reported at **$1.50 input / $7.50 output per million tokens**. That is about **twice** the old Flash rate. It has a **1M-token context** and a new **"xhigh" thinking level**. It is available on all **Gemini API / AI Studio** tiers, including free, and in **Antigravity** for paid AI Pro/Ultra users.

- **Why this matters for you (developer/entrepreneur):** Hydrogen is aimed at high-volume agent and coding loops. If you run on 3.8 Flash, re-check your costs before switching: the per-token price doubles, though fewer tokens per task may close part of the gap.
- **Business/project idea:** A **"cheap planner, smart executor" coding agent**. Hydrogen (low/medium thinking) handles routing, file search and test runs, and escalates only hard diffs to Argon or Sonnet 5.5. Sell it as a CI bot that fixes failing tests. Use Hydrogen's free API tier for your own prototyping and its 1M context to load whole repos.
- Sources: [Google blog](https://blog.google/innovation-and-ai/models-and-research/gemini-models/introducing-gemini-4-hydrogen/) · [9to5Google](https://9to5google.com/2026/11/12/gemini-4-hydrogen-launch/) · [Interesting Engineering](https://interestingengineering.com/ai-robotics/google-gemini-4-hydrogen-coding-benchmark) · [Digital Trends](https://www.digitaltrends.com/cool-tech/googles-next-gen-gemini-4-hydrogen-ai-model-is-here-touting-faster-intelligence-for-all/) · [DataStudios (pricing)](https://www.datastudios.org/post/google-gemini-4-hydrogen-launch-api-pricing-gemini-app-search)

## 3. Anthropic IPO: $70–78 range, reportedly about 6x oversubscribed, trading expected Nov 19

Anthropic set a **price range of $70–78** for about **825M Class A shares** on the **Nasdaq (ticker: ANT)**. Pricing is expected **Nov 18** and trading **Nov 19**, though neither date is final. Bloomberg reports orders at about **6x the shares available**. Estimated valuations range from about **$1T** to **$1.4T fully diluted**. The S-1, filed Oct 26, shows **H1 2026 revenue of about $16.3B** and compute commitments that include about **$3.1B/month** to SpaceX for Nvidia-GPU capacity.

- **Why this matters for you (developer/entrepreneur):** As a public company, Anthropic will report revenue, margins and pricing every quarter. That makes the economics of building on Claude easier to see. Expect more focus on enterprise revenue: channel partners, Claude for Workspace and deployment engineers.
- **Business/project idea:** An **"AI-vendor disclosure tracker"**. Parse S-1/10-Q filings from Anthropic (and later OpenAI) with an LLM, pull out per-token unit economics, capacity commitments and risk factors, and sell a monthly brief to CTOs and procurement teams negotiating AI contracts.
- Sources: [CNBC](https://www.cnbc.com/2026/11/10/anthropic-sets-price-range-of-70-to-78-in-upcoming-ipo.html) · [Anthropic](https://www.anthropic.com/news/s1-sec) · [TradingView/Stocktwits](https://www.tradingview.com/news/stocktwits:0dc81ad1f094b:0-ai-trade-barometer-anthropic-s-ipo-is-reportedly-six-times-oversubscribed/) · [investingLive](https://investinglive.com/stocks/anthropic-ipo-six-times-oversubscribed-what-retail-investors-can-realistically-expect/)

## 4. OpenAI reportedly raises $15B at a $1.25T valuation, half its original target (Nov 12, per CNBC)

**CNBC** reports that OpenAI raised **$15B at a $1.25T pre-money valuation**, against an original target of **$30B** at about **$1.4T**. The round has **not formally closed**, and **OpenAI has not confirmed the figures**. Q3 revenue reportedly crossed **$10B** (up about 50% from Q2), with an operating loss of about **$10.9B** (WSJ). Coverage frames the round as a bridge to a possible **2027 IPO**.

- **Why this matters for you (developer/entrepreneur):** A smaller-than-planned round alongside large losses suggests pressure on OpenAI to raise **API prices or cut subsidized tiers**. Build abstraction layers now so a price change doesn't break your margins.
- **Business/project idea:** A **"price-shock simulator"** for AI-native SaaS. Connect usage logs from OpenAI, Anthropic and Gemini, then model margin under scenarios ("+30% GPT price", "move 40% of traffic to Hydrogen"). Recommend routing changes automatically and charge a percentage of the savings.
- Sources: [Dealroom](https://dealroom.co/news/172395-openai-raises-15b-at-a-1-25t-valuation-half-its-original-target-as-it-br/) · [Benzinga](https://www.benzinga.com/markets/private-markets/26/11/63213967/openai-raises-15b-at-1-25t-valuation-in-latest-funding-round-amid-ipo-plans) · [Crypto Briefing (citing CNBC)](https://cryptobriefing.com/openai-raises-15-billion-at-125-trillion-valuation-cnbc-reports/) · [Futu News](https://news.futunn.com/en/post/1004345040/new-evidence-of-a-funding-shortfall-at-openai-the-latest)

## 5. A state-linked hacking group used the open-source Hermes agent to steal 2,000+ Tajik government documents (Nov 11–12)

**CloudSEK** researchers, reported by **Reuters**, say the Kazakhstan-linked group **Silent Lynx** used **Hermes**, an **open-source autonomous AI agent framework**. The agent did reconnaissance, planned the intrusion, wrote and ran the attack steps, kept notes and wrote reports. It also **built its own tool** to download, sort and chunk more than **2,000 national-security documents**. The operation was found because the group left a server exposed to the internet. Tying the group to the Kazakh *government* is **not proven**. This follows last week's CrowdStrike report on VAPOR PANDA's ARTEX agent, so open agent frameworks now appear in at least two documented state-linked campaigns.

- **Why this matters for you (developer/entrepreneur):** Attackers are now running full intrusions with AI agents, so attacks get faster and need fewer people. Assume anything exposed to the internet will be scanned and attacked by agents around the clock. If you ship an agent framework, abuse-detection and logging features are becoming a selling point.
- **Business/project idea:** An **"agentic-attack honeypot" SaaS**. Deploy decoy document systems and APIs that detect agent-like behavior (tool-call cadence, LLM-style reconnaissance prompts, automatic chunking) and send alerts. Use an LLM to classify attacker transcripts and produce threat-intel reports for mid-size government contractors.
- Sources: [AKIpress](https://akipress.com/news:930912) · [Caspian Post](https://caspianpost.com/regions/kazakhstan-linked-hackers-used-ai-to-steal-tajik-government-documents-report) · [InfotechLead](https://infotechlead.com/security/kazakhstan-linked-hackers-use-autonomous-ai-agent-hermes-to-steal-2000-tajikistan-government-documents-99566) · [SRN News (Reuters)](https://srnnews.com/kazakhstan-linked-hackers-used-ai-to-steal-tajik-government-documents-researchers-say/)

## 6. Microsoft 365 outage takes down Outlook, Teams, Copilot and AI connectors for 5+ hours (Nov 12)

A major **Microsoft 365 outage** disrupted **Exchange Online, Teams, SharePoint, Microsoft 365 Copilot and Defender XDR** for more than five hours. Downdetector reports peaked at about **130–138K**. Microsoft blamed servers that became **unexpectedly unavailable under elevated load**, not a cyberattack. Recovery came from restarting servers and was still only partial in the evening. The outage also broke **connectors that OpenAI and Anthropic services use** to reach M365 data.

- **Why this matters for you (developer/entrepreneur):** If your agents read email, calendars or SharePoint through M365 connectors, a single vendor outage stops them. Design for **graceful degradation**: cache context, queue actions and show clear status to users.
- **Business/project idea:** A **"connector health" layer for AI agents**. Monitor MCP and SaaS connector endpoints (M365, Google Workspace, Slack), switch agents to cached or read-only mode during outages, and replay queued actions afterward. Offer it as an MCP proxy that teams can drop in.
- Sources: [BleepingComputer](https://www.bleepingcomputer.com/news/microsoft/massive-microsoft-365-outage-disrupts-outlook-teams-copilot-worldwide/) · [SecurityWeek](https://www.securityweek.com/microsoft-365-outage-disrupts-outlook-exchange-online-and-teams/) · [TechRepublic](https://www.techrepublic.com/article/news-microsoft-outlook-outage-130000-reports-2026/) · [The Tribune](https://www.tribuneindia.com/news/business/microsoft-outage-disrupts-outlook-teams-and-ai-services-for-over-five-hours)

## 7. Google adds two specialized TPUs: TPU 8tx (confidential inference, co-developed with AMD) and TPU 8i Max (Nov 9–10)

Google announced **TPU 8tx**, built on TPU 8t with **hardware-level security** that protects data and **model weights while they are in use**. TechCrunch and Dataconomy report it was co-developed with **AMD**. It also announced **TPU 8i Max**, which puts **two TPU 8i chips in one package** for roughly double the memory, compute and bandwidth, aimed at **long-context** inference. Both are due in **2027**. Several outlets describe them as reconfigured versions of existing silicon rather than new designs.

- **Why this matters for you (developer/entrepreneur):** Confidential inference on Google Cloud would make it easier to sell AI into healthcare, finance and government, where data-in-use protection is often required. More memory per package makes very long-context serving cheaper.
- **Business/project idea:** A **"confidential AI" offering for regulated SMBs**. Start now on current confidential-computing VMs, then move to TPU 8tx. Run fine-tuned models on client data with attestation reports you can show auditors, and sell to clinics, law firms or insurers that can't send data to standard APIs.
- Sources: [TechCrunch](https://techcrunch.com/2026/11/10/google-broadens-its-ai-hardware-portfolio-with-two-new-specialized-chips/) · [Quartz (Bloomberg)](https://qz.com/google-specialized-ai-chips-tpu-nvidia-110926) · [Dataconomy](https://dataconomy.com/2026/11/11/google-unveils-two-specialized-ai-chips-including-amd/)

## 8. OpenAI rolls out GPT-6 Cyber to vetted Daybreak Red customers (Nov 5–6, wider access over coming weeks)

**GPT-6 Cyber** is a restricted, security-focused model available through the **API and Codex** to approved **Daybreak Red** customers. Requirements reportedly include identity verification, multifactor authentication and IP allowlisting. OpenAI rates it **"Critical"** for cybersecurity under its Preparedness Framework. It reports **48.5% on ExploitGym** (vs 32.1% for GPT-5.6 Cyber), working exploits for **948 Linux kernel vulnerabilities** and **81 previously unknown high-severity Firefox flaws**. These are vendor numbers, and one outlet notes independent tests show gaps.

- **Why this matters for you (developer/entrepreneur):** Defensive vulnerability research with frontier models is now a gated, application-only product. Security firms that get access early will have a real advantage in AI-assisted pentesting and patching.
- **Business/project idea:** Apply for Daybreak Red and build a **"continuous exploitability triage" service**. Feed a client's SBOM and CVE feed to GPT-6 Cyber, which checks which vulnerabilities can actually be exploited in their build, and open prioritized patch PRs through Codex. This pairs well with the agent-driven attacks in item 5.
- Sources: [Security Boulevard](https://securityboulevard.com/2026/11/openai-launches-gpt-6-cyber-to-find-security-flaws-limits-access-over-hacking-risks/) · [Yahoo Finance](https://finance.yahoo.com/news/openai-launches-gpt-6-cyber-084819971.html) · [TestingCatalog](https://www.testingcatalog.com/openai-launches-gpt-6-cyber-for-daybreak-red-customers.md) · [OpenAI](https://openai.com/et-EE/index/introducing-gpt-6-cyber/)

---

## Also noted (lower significance)

- **Apple HomeView** ($299 smart display with Siri AI) goes on sale **today, Nov 13**. It is not sold in the EU, and full independent reviews aren't out yet. ([MacRumors](https://www.macrumors.com/2026/11/09/apple-launching-two-new-products-on-november-13/) · [Macworld](https://www.macworld.com/article/676817/apple-homeview-guide-specs-features-release-date.html))
- **Google's November Pixel Drop** brings Gemini Intelligence to the Pixel 10 line and adds **Pixel Tag**, Google's first item tracker. ([Business Standard](https://business-standard.com/technology/tech-news/google-november-2026-pixel-drop-gemini-intelligence-pixel-tag-features-126111200342_1.html))

## UNVERIFIED / excluded (not presented as fact)

- **Agile Robots $500M Series F led by SoftBank at $8.5B**: found in one outlet only (SiliconANGLE). Earlier reports described an $800M round still in talks.
- **Huang summoned to testify before Congress**: seen only in a CNN headline, not confirmed.
- **Gemini 4 Hydrogen price cut of 62.5% on Dec 1**: single source.
- **Anthropic "$100M to train 10,000 engineers"** appeared in some Nov 13 roundups, but it is an **Oct 2** announcement (Claude Frontier Academy), so it is not new.
