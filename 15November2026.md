# Daily Tech & AI Briefing — 15 November 2026

**Biggest story:** Nvidia's search for a new CEO has started in earnest. The **Financial Times** reports the board **approached Arm CEO Rene Haas** to succeed Jensen Huang. Meanwhile, open-weight frontier models and agent infrastructure kept moving: **Inkling 2 Small's weights are out**, and **Cloudflare open-sourced Kitesurf**, its agent browser engine.

> Note: it's a quiet weekend news day, so most items are from Nov 12–14. Items already covered in the Nov 13–14 briefings (ChatGPT Wallet, Huang's resignation, the nonprofit lawsuit) are not repeated. Benchmarks are vendor-reported unless stated otherwise.

---

## 1. Nvidia board reportedly approached Arm CEO Rene Haas as Jensen Huang's successor (Nov 13–14)

The **Financial Times** reports that Nvidia's board **approached Rene Haas**, who has led **Arm** since 2022 and earlier spent seven years at Nvidia. Nvidia says it is still **choosing a search firm** and has **not formally engaged any candidate**, and that the search will look both inside and outside the company. Sources say an offer to Haas is not guaranteed, nor is his acceptance. **Colette Kress** remains interim CEO. Internally, an employee post urging the board to bring Huang back has drawn more than **1,600 comments**. Analysts have also floated AMD's **Lisa Su** and Micron's **Sanjay Mehrotra**.

- **Why this matters for you (developer/entrepreneur):** A CEO from Arm would suggest a stronger push into Arm-based CPUs and power-efficient inference. That would affect where CUDA and the Grace/Arm server stack go next. Until a leader is named, expect roadmap and pricing uncertainty in GPU supply deals.
- **Business/project idea:** Build a "compute-portability audit" tool. It scans a team's ML code for CUDA-only dependencies (custom kernels, NCCL, TensorRT) and estimates the effort to run on AMD ROCm, TPUs or Arm CPUs. Sell it to startups that want leverage on hardware while Nvidia's leadership is unsettled.
- Sources: [Yahoo Finance](https://finance.yahoo.com/technology/articles/nvidia-approached-arm-ceo-rene-195019281.html) · [The Japan Times](https://www.japantimes.co.jp/business/2026/11/14/companies/nvidia-arm-ceo-haas-huang/) · [Tom's Hardware](https://www.tomshardware.com/pc-components/gpus/nvidia-board-reportedly-approached-arm-ceo-rene-haas-during-replacement-search-jensen-huangs-transgressions-leave-nvidia-scrambling-to-fill-a-massive-void) · [Decrypt](https://decrypt.co/383276/nvidia-arm-ceo-rene-haas-replace-jensen-huang)

## 2. Thinking Machines releases Inkling 2 Small weights under Apache 2.0 (Nov 12, now confirmed)

Yesterday's briefing marked this unverified. It is now confirmed by the official **model card** and several outlets. **Inkling 2 Small** is a sparse **mixture-of-experts** model with **594B total / 17B active parameters**, **image input** and a **1M-token context window**. It launched closed on **Tinker** on Nov 5, and the weights followed on **Hugging Face** after external red-teaming, under **Apache 2.0**. It scores **31 on the Artificial Analysis Intelligence Index** and is described as the strongest open model built outside China. The main **NVFP4** checkpoint needs about **500GB of total VRAM**. A larger **MXFP8** checkpoint is also available.

- **Why this matters for you (developer/entrepreneur):** You now have a commercially licensed, Western-built open model that can run on your own hardware. That matters for regulated customers who can't send data to closed APIs or use Chinese-origin weights. Only 17B parameters are active per token, so serving costs are much lower than the total size suggests.
- **Business/project idea:** Offer "sovereign Inkling" deployments. Package Inkling 2 Small (NVFP4 on one 8×B200-class node) together with a fine-tuning pipeline that runs through Tinker. Sell it to healthcare, legal or government customers as a private, fine-tuned assistant running on-prem or in their own cloud account, with the license as the compliance pitch.
- Sources: [Thinking Machines model card](https://thinkingmachines.ai/model-card/inkling-2-small/) · [AlphaSignal](https://alphasignal.ai/news/thinking-machines-opens-inkling-2-small-s-594b-weights-to-developers) · [Trending Topics](https://www.trendingtopics.eu/inkling-2-thinking-machines-mistral-open-weight-en/) · [Crypto Briefing](https://cryptobriefing.com/thinking-machines-inkling-2-small-release/)

## 3. Cloudflare open-sources Kitesurf, a lightweight browser engine for AI agents (Nov 12–13)

Cloudflare released **Kitesurf** under **Apache 2.0**. It is a **Rust + WebAssembly** engine that loads pages and runs JavaScript **without a Chromium container**, and it is designed to use much less CPU and memory than headless Chrome. Clients connect over the **Chrome DevTools Protocol**, so existing **Puppeteer** scripts should work largely unchanged. You can run it locally with **Wrangler** or deploy it on your own **Workers** account. Cloudflare's hosted Browser Run APIs remain available. Caveats: Cloudflare says it is under heavy development, web-platform compatibility is incomplete, and extensions are not supported. (A "7x less memory" figure appears in only one outlet and is not verified.)

- **Why this matters for you (developer/entrepreneur):** Headless Chrome is usually the most expensive part of a web agent or scraper. A CDP-compatible engine that runs on Workers could cut per-session costs and cold starts sharply, as long as your target sites render correctly in it.
- **Business/project idea:** Build an "agent browsing cost optimizer" proxy. It sends each CDP session to Kitesurf first, checks the render (DOM completeness, screenshot diff), and automatically falls back to Chromium for sites Kitesurf can't handle yet. Charge per session and share the savings with agent startups that run thousands of browsing tasks a day.
- Sources: [Cloudflare changelog](https://developers.cloudflare.com/changelog/post/2026-11-12-kitesurf-open-source/) · [Phoronix](https://www.phoronix.com/news/Cloudflare-Kitesurf-Open-Source) · [Linuxiac](https://linuxiac.com/cloudflare-open-sources-kitesurf-its-lightweight-browser-engine-for-ai-agents/) · [Unite.AI](https://www.unite.ai/cloudflare-open-sources-kitesurf-browser-engine-for-ai-agents/)

## 4. LangChain raises a $300M Series C at a $3B valuation, led by CapitalG (Nov 13)

**LangChain** raised **$300M** at a **$3B valuation**, 2.4x its $1.25B Series B in late 2025, bringing total funding to about **$460M**. Alphabet's **CapitalG** led, with **GIC, DFJ Growth, IVP and Sapphire** participating (some outlets also list Salesforce and MongoDB Ventures). The pitch centers on **LangSmith** as a **model-neutral platform for running and governing agents**. It can be deployed in LangChain's cloud, on-prem, or inside a customer's AWS, Azure or GCP account.

- **Why this matters for you (developer/entrepreneur):** Investors are betting on vendor-neutral agent infrastructure (observability, evals, governance) rather than lock-in to one model lab. Expect LangSmith to keep adding enterprise features, so niche tools need to build on it or go deeper in one area.
- **Business/project idea:** Build vertical eval packs on LangSmith. Examples: a pre-built dataset, scorers and dashboards for "insurance claims agent" or "SOC triage agent", sold as a LangSmith add-on to enterprises that bought the platform but have no domain-specific way to measure agent quality.
- Sources: [LangChain blog](https://www.langchain.com/blog/series-c) · [WebProNews](https://www.webpronews.com/langchain-300-million-series-c-3-billion-valuation-langsmith) · [Trending Topics](https://www.trendingtopics.eu/langchain-series-c-300-million-dollars/) · [NewsBytes](https://www.newsbytesapp.com/news/business/langchain-raises-300m-at-3b-valuation-to-manage-ai-agents/story)

## 5. OpenAI disbands its stand-alone robotics team as general models start running robots (Nov 13)

According to **Fortune**, with OpenAI confirming the change, OpenAI has **dissolved its dedicated robotics team**. Researchers are moving into core research under **Mark Chen**, and applied/hardware staff into **Greg Brockman's Applied** org. OpenAI's reasoning is that its **general-purpose models can now control robots** directly, so a separate robotics model effort is less necessary. The company calls this a sign of commitment, not a retreat. It is OpenAI's second time winding down robotics (the first was 2020), after rebuilding the team in 2024.

- **Why this matters for you (developer/entrepreneur):** This supports the idea that robot control is becoming one more capability of foundation models, reached through the same APIs, rather than a separate model category. For robotics startups, the advantage shifts toward hardware, data collection and integration.
- **Business/project idea:** Build a "foundation model to robot" adapter layer: a ROS 2 bridge that turns a robot's camera feeds and joint state into tool-calling inputs for general multimodal APIs and runs safety-checked action outputs. Sell it to warehouse and lab-automation integrators who want to try general models without training their own policies.
- Sources: [Yahoo Tech (Fortune exclusive)](https://tech.yahoo.com/ai/articles/exclusive-openai-disbands-stand-alone-170530559.html) · [Seeking Alpha](https://seekingalpha.com/news/4672622-openai-dissolves-stand-alone-robotics-team-report?feed_item_type=news) · [OfficeChai](https://officechai.com/ai/openai-disbands-robotics-team-after-general-purpose-models-begin-running-robots/)

## 6. Anthropic IPO week: pricing expected Wed Nov 18, trading as ANT on Thu Nov 19

No change to the terms. The amended S-1 sets **$70–$78 per share** for **825M Class A shares** on Nasdaq, which would raise up to about **$64B**. About **20% is earmarked for retail**, and about **$26B** in concurrent strategic purchases is expected from **Microsoft, Nvidia, Alphabet and Micron**. Valuation estimates range from about **$1T to $1.3T**, depending on how shares are counted. Dates are "subject to regulatory clearance."

- **Why this matters for you (developer/entrepreneur):** A public Anthropic will report quarterly, which gives you real data on API demand, margins and pricing pressure. Expect pricing and enterprise-plan changes to be shaped by public-market expectations.
- **Business/project idea:** Build an "AI vendor health" dashboard for CTOs. It combines public filings (Anthropic, plus OpenAI's reported numbers), status-page uptime and price-change history to score vendor risk, and alerts procurement teams before contract renewals.
- Sources: [CNBC](https://www.cnbc.com/2026/11/10/anthropic-sets-price-range-of-70-to-78-in-upcoming-ipo.html) · [FinanceFeeds](https://financefeeds.com/anthropic-ipo-date-price-range-70-78-trading-19-november/) · [Investinglive](https://investinglive.com/stocks/anthropic-ipo-targets-around-1-trillion-valuation-half-the-2-trillion-once-whispered/)

---

## UNVERIFIED / excluded (not presented as fact)

- **Agile Robots raises $500M at an $8.5B valuation, led by SoftBank (Nov 12):** reported only by SiliconANGLE. Other coverage refers to earlier talks about an $800M round.
- **SGLang Consortium for cross-hardware open-source inference:** appears in only one newsletter.
- **Microsoft Ignite 2026 (expected ~Nov 17–20) agent announcements:** I found no confirmed 2026 previews, only recaps of Ignite 2025.
- **Corewell Health ambient-AI pilot cutting nursing documentation time by 52%:** single newsletter mention.
