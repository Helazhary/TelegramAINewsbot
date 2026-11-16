# Daily Tech & AI Briefing — 16 November 2026

**Biggest story:** Nvidia goes into its first earnings report without Jensen Huang (Tuesday, Nov 17). Over the weekend, two large shareholders asked the board to leave the door open for his return, a Reuters report said he misled senior executives, and Congress is lining up testimony. Anthropic's IPO and Microsoft Ignite are also due this week.

> Note: this briefing covers what's new since the 15 November report. Huang's resignation, Gemini 4 Hydrogen, Claude Fable 5.2, Claude Meetings/Sheets, GPT-6 Cyber and ChatGPT Wallet were covered in earlier briefings and aren't repeated here. It was a quiet weekend for launches. Several sites (TechCrunch, creati.ai, some Substack roundups) couldn't be opened from this environment, so cross-checks rely on search results from other outlets.

---

## 1. Nvidia: investors push for a Huang return before Tuesday's earnings (Nov 13–16)

Four days after **Jensen Huang resigned**, the pressure on Nvidia's board is growing. **Two of Nvidia's largest outside shareholders** wrote to the board urging it to consider a **"potential return of Jensen Huang"** (CNBC, Nov 14). A public **"Stand with Jensen" petition** has passed **100,000+ signatures**, with **Elon Musk** among the signers. The signer affiliations are self-reported and unverified. Against that, **Reuters reported (Nov 13)** that Huang **misled Nvidia's general counsel and CMO** in October about his relationship with **Alice Huang**, a businesswoman under US investigation for possible spying. He described their contact as ordinary customer business. Neither Huang nor Nvidia commented. The independent directors' investigation is run by **Wachtell Lipton**. **Senate Banking chair Tim Scott** has asked Huang to testify (reported date **Dec 3**, not yet confirmed), and House committees want a closed-door interview. **Interim CEO Colette Kress** leads the **Q3 FY2027 earnings call on Tue Nov 17** (2 p.m. PT), against August guidance of about **$108B revenue**.

- **Why this matters for you (developer/entrepreneur):** If you build on CUDA or rent GPUs, watch the call for any change to roadmap, supply-allocation or China guidance. A leadership crisis at the main AI compute supplier can move GPU prices and cloud capacity. Earnings day will also move AI stocks and the funding mood, a day before Anthropic prices.
- **Business/project idea:** Build a **"key-person risk" monitor for AI infrastructure**: a dashboard that tracks leadership changes, regulatory hearings, export-control moves and earnings-call wording at your critical vendors (Nvidia, hyperscalers, model labs), and sends alerts with a suggested hedge, such as "reserve AMD/TPU capacity" or "test an open model fallback". Use a frontier LLM to summarize SEC filings, transcripts and news feeds into risk scores for CTOs and procurement teams.
- Sources: [CNBC (investor letter, Nov 14)](https://www.cnbc.com/2026/11/14/nvidia-investors-jensen-huang-return-board-letter.html) · [CNBC (Nov 16)](https://www.cnbc.com/2026/11/16/nvidia-jensen-huang-return-tech.html) · [Arab News (Reuters report)](https://www.arabnews.com/world/musk-tech-leaders-back-jensen-huang-as-reuters-report-alleges-he-misled-nvidia-lawyer-over-affair-3012134) · [HuffPost](https://www.huffpost.com/entry/nvidia-ceo-affair-jensen-huang_n_6af7dca9e4b0016f2eb7c888) · [TechSpot (petition)](https://www.techspot.com/news/114563-nearly-150000-people-sign-petition-requesting-jensen-huang.html) · [SCMP (Congress)](https://www.scmp.com/news/china/diplomacy/article/3374412/us-congress-widens-nvidia-probe-seeking-testimony-jensen-huang-and-trump-officials) · [Investing.com (earnings date)](https://www.investing.com/news/company-news/nvidia-schedules-q3-fiscal-2027-earnings-call-for-nov-17-93CH-4980909)

---

## 2. US and eight allies sign the "San Francisco Declaration" to protect AI supply chains from China (Nov 15)

According to the **Financial Times** (relayed by Bloomberg and others), the US and its partners signed a **declaration under the US-led Pax Silica initiative**. They will **jointly identify and protect AI technologies and supply chains** they see as vulnerable to China. Under Secretary of State **Jacob Helberg** said **Japan, Australia, Israel, the UK, South Korea, India, Qatar and the UAE** have signed, and that **Germany, Sweden, the Netherlands and the European Commission** are expected to sign **next week**. The plan includes a **shared list of critical technologies**, **working groups** on supply-chain weak points, and **investment hubs** for related industries. It comes just before the expected **Trump–Xi meeting at APEC**.

- **Why this matters for you (developer/entrepreneur):** "Critical AI technology" lists usually turn into procurement rules, export controls and investment screening. If you sell AI infrastructure, chips, data-center gear or models abroad, or take capital from the Gulf or Asia, your compliance work is about to grow, and so are government-funded opportunities in allied countries.
- **Business/project idea:** Build an **AI supply-chain compliance copilot**: upload a bill of materials or cloud/model stack, and it maps each component (GPUs, HBM, model weights, data centers, investors) to its country of origin, applicable export controls and Pax Silica lists, then flags risks. Use an LLM with retrieval over government lists and regulations, and sell it to AI hardware startups and sovereign-AI projects.
- Sources: [Bloomberg (citing FT)](https://www.bloomberg.com/news/articles/2026-11-15/us-allies-agree-to-guard-ai-supply-chains-from-china-ft-says) · [Yahoo News](https://www.yahoo.com/news/politics/articles/report-us-allies-sign-accord-181215730.html) · [ANI (India signs)](https://aninews.in/news/world/us/india-signs-us-led-declaration-to-safeguard-ai-supply-chains-report20261116061901/)

---

## 3. SpaceX catches a Starship upper stage with the launch tower for the first time (Nov 14)

On **Starship Flight 15**, **Ship 42** flew **14 orbits**, deployed **26 Starlink V3 satellites**, then came back after about **22.5 hours** and was **caught by the tower's "chopstick" arms** at Starbase. That had never been done with the upper stage. Booster catches had been done before. The **Super Heavy booster was not caught**: it diverted to a Gulf of Mexico splashdown after a **low-fuel alarm**, so the planned double catch fell short. SpaceX plans to try again on an upcoming flight.

- **Why this matters for you (developer/entrepreneur):** A fully reusable heavy launcher is how launch costs fall sharply. That means more and cheaper Starlink capacity, and over time, cheaper rides for satellites and orbital compute. Space-based connectivity and data are becoming a commodity to build on.
- **Business/project idea:** Build an **AI analytics layer for the next wave of low-cost Earth observation**: an API that takes imagery from new small-satellite constellations and returns structured answers ("how many trucks at this depot this week?", "crop stress in field X"), using vision-language models fine-tuned for each vertical. Lower launch costs mean more providers and lower data prices, so the value moves to interpretation.
- Sources: [Space.com](https://www.space.com/space-exploration/launches-spacecraft/spacex-chopsticks-catch-starship-upper-stage-flight-14) · [UPI](https://www.upi.com/Top_News/US/2026/11/14/spacex-starship-upper-stage/1201794703333) · [Interesting Engineering](https://interestingengineering.com/space/spacex-starship-ship-42-first-upper-stage-catch) · [Teslarati](https://www.teslarati.com/spacex-catches-starship-first/)

---

## 4. Salesforce releases SOV-Transcribe-1, now the top open-weights speech-to-text model (Nov 12)

**Salesforce** released **SOV-Transcribe-1** on **Hugging Face under Apache 2.0**. It is a **non-streaming ASR model** with about **26.6B total / ~4.6B active parameters (MoE)**. It reportedly pairs a **Whisper large-v3 encoder** with a **Gemma-family MoE decoder**. On the **Artificial Analysis non-streaming WER benchmark** it scores about **2.3% word error rate**: **#1 among open-weights models** and about **#7 overall**. It accepts **natural-language instructions** for formatting and custom vocabulary. **Caveats:** the BF16 checkpoint is about **53 GB**, so it won't fit on a single 48 GB GPU without quantization. It is **batch-only, not real-time**, and the accuracy figures come from Salesforce and benchmark trackers, not independent audits.

- **Why this matters for you (developer/entrepreneur):** Near-frontier transcription accuracy you can **self-host** means you can process sensitive audio (medical, legal, financial calls) without sending it to a third-party API, and with no per-minute fees at scale.
- **Business/project idea:** Build a **private, on-prem transcription and minutes appliance** for law firms or clinics: SOV-Transcribe-1 (quantized, on one or two GPUs) for batch transcription, with prompts that inject client names and jargon as custom vocabulary, then a small local LLM that turns transcripts into structured notes, billing entries or SOAP notes. Sell it as a box or VPC deployment with a "no audio leaves your premises" guarantee.
- Sources: [Hugging Face model card](https://huggingface.co/salesforce-sovereign-intelligence/SOV-Transcribe-1) · [CASRAI](https://casrai.org/news/salesforce-sov-transcribe-1-open-weight-asr-2026) · [AlphaSignal](https://alphasignal.ai/news/salesforce-s-sov-transcribe-1-beats-every-open-weight-speech-model-at-2-3-error) · [BenchLM](https://benchlm.ai/models/sov-transcribe-1)

---

## 5. Anthropic's IPO shuts out mainland China and Hong Kong investors; pricing due Wed (Nov 13–18)

**Bloomberg** reports that underwriters are **rejecting share orders from mainland China and Hong Kong institutions** in **Anthropic's IPO**. This mirrors how the SpaceX IPO was handled. Reports differ on the reason: some cite **ITAR/national-security concerns**, while others describe it as **allocation policy** rather than a legal ban on owning shares later. The prospectus doesn't spell it out. The deal is reportedly targeting a valuation of **up to about $1.4T**, with **pricing expected Wed Nov 18** and **Nasdaq trading as "ANT" on Thu Nov 19**. Orders are reportedly about **6x the shares available**.

- **Why this matters for you (developer/entrepreneur):** A successful listing at this valuation sets the benchmark for AI-lab and AI-app fundraising in 2027. It also means Anthropic will report quarterly as a public company, so expect more visibility into API pricing, capacity and roadmap. The China carve-out also shows frontier AI is being handled as national-security infrastructure.
- **Business/project idea:** Build an **"IPO-era" LLM vendor tracker**: it parses each public AI lab's filings and earnings calls (Anthropic, and others as they list) for signals about pricing, compute commitments, gross margin and deprecations, then tells API customers how likely price or model changes are. This is useful for teams deciding which provider to bet a product on.
- Sources: [Bloomberg](https://www.bloomberg.com/news/articles/2026-11-13/anthropic-ipo-share-orders-from-china-are-said-to-be-rebuffed) · [Investing.com](https://in.investing.com/news/stock-market-news/anthropic-ipo-shuts-out-chinese-investors-amid-uschina-tensions-5703680) · [Stocktwits](https://stocktwits.com/news-articles/markets/equity/anthropic-ipo-reportedly-closed-to-china-hong-kong-buyers-mirroring-space-x-playbook/cNbRBAoR9ft) · [Roic.ai](https://www.roic.ai/news/anthropics-ipo-said-to-exclude-china-and-hong-kong-investors-11-13-2026)

---

## 6. GitHub Copilot removes Claude Opus 5, Opus 4.8 and GPT-5.6 Terra today (Nov 16)

The deprecation **GitHub announced on Oct 15** takes effect **today**. **Claude Opus 5**, **Claude Opus 4.8** and **GPT-5.6 Terra** are removed from **every Copilot surface**: Chat, inline edits, ask/agent modes and code completions. GitHub points users to **Claude Opus 5.5** as the replacement for the Opus models. Secondary write-ups list **GPT-6.x** models as the OpenAI replacements, so check GitHub's changelog table for the exact mapping. **Individual annual-plan subscribers keep Opus 4.8.** Deprecated models drop out of Business/Enterprise policy lists automatically.

- **Why this matters for you (developer/entrepreneur):** Any **agent definitions, scripts, `.github` configs or CI jobs that hard-code these model IDs** may fail or silently fall back starting today. Check them now. Model churn is also a real maintenance cost to plan for.
- **Business/project idea:** Build a **"model-deprecation linter"**: a GitHub Action or CLI that scans repos for hard-coded model IDs (Copilot configs, SDK calls, agent YAML, prompt files), checks them against provider deprecation feeds (GitHub, Anthropic, OpenAI, Google) and opens PRs that migrate to the recommended replacements, with an eval run attached. Sell it per repo to platform teams.
- Sources: [GitHub Changelog](https://github.blog/changelog/2026-10-15-upcoming-deprecation-of-selected-github-copilot-models-in-mid-november) · [Classmethod](https://dev.classmethod.jp/en/articles/github-copilot-model-deprecation-nov-2026/) · [SmartScope](https://smartscope.blog/en/blog/github-copilot-claude-opus-5-deprecation-november-16-2026/)

---

## 7. IBM + Microsoft launch "Imagine Enterprise" with 6,000+ prebuilt agents, ahead of Ignite (Nov 10; Ignite Nov 17–20)

**IBM and Microsoft** launched **Imagine Enterprise**, a joint platform for **building, running and governing AI agents** tied to industry processes. **IBM** provides **6,000+ prebuilt agents and assets** from IBM Consulting Advantage, plus consultants. **Microsoft** provides the **cloud, identity and security stack**. Both put in **forward-deployed engineers**. It is designed to sit on top of existing systems rather than replace them. The first targets are **financial services, insurance and retail**. **Pricing, general availability and production customers have not been disclosed.** **Microsoft Ignite** opens **tomorrow (Nov 17)** in San Francisco, where agents, Copilot and agent governance are expected to lead. No announcements are public yet.

- **Why this matters for you (developer/entrepreneur):** The big integrators are bundling agent catalogs with cloud identity and governance, aiming at the "agent platform" budget startups also chase. If you sell agents to enterprises, plan to **plug into Microsoft identity and governance (Entra, Purview, Agent 365)** rather than compete with it.
- **Business/project idea:** Build **independent evaluation and certification for prebuilt enterprise agents**: a harness that runs catalog agents (IBM's, Microsoft's, Salesforce's) against a customer's real but anonymized workflows and data, scoring accuracy, cost, permission scope and audit trail before rollout. The vendors haven't published independent governance test results, so a neutral "agent QA" layer fills a gap.
- Sources: [CIO Dive](https://www.ciodive.com/news/microsoft-ibm-team-up-ai-agent-platform/874152/) · [Petri](https://petri.com/?p=781344) · [Analytics India Magazine](https://analyticsindiamag.com/ai-news/ibm-microsoft-launch-agentic-ai-platform-with-over-6000-ai-agents) · [Ignite preview (Crypto Briefing)](https://cryptobriefing.com/microsoft-ignite-2026-copilot-updates/)

---

## This week's calendar
- **Tue Nov 17:** Nvidia Q3 FY27 earnings (first without Huang); Microsoft Ignite keynote (Nadella).
- **Wed Nov 18:** Anthropic IPO pricing (expected).
- **Thu Nov 19:** Anthropic expected to start trading as ANT; Claude Data turns on by default for Enterprise plans.
- **Next week:** Germany, Sweden, the Netherlands and the EC expected to sign the San Francisco Declaration.

## UNVERIFIED / excluded (not presented as fact)
- **"Italy fines Meta €805M over Android photo access":** appeared in one morning brief; no matching report found elsewhere. Dropped.
- **"AT&T has ~500 autonomous AI workflows in production":** the **45B tokens/day** figure is confirmed by AT&T's own blog, but the 500-workflow number wasn't found in any second source.
- **Malaysia law requiring data centers to disclose AI chip imports and power use:** one roundup only; not confirmed.
- **Claude Code "Code Mode" (v2.1.323) and other weekly tool changelog items:** from a single dev.to roundup; check the official changelogs.
- **FAA ground-stop cause:** sources conflict (router/telecom maintenance vs. the new AI tool, and wildly different cancellation counts). See the 14 November briefing; no new confirmed findings.
