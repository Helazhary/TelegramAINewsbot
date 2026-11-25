# Daily Tech & AI Briefing — 25 November 2026

**Today's biggest story:** Anthropic launched **Claude Ship**, a set of agents that review, fix and (under policy) *approve* GitHub pull requests. It is the clearest step yet toward AI-run code review loops.

---

## 1. Anthropic launches Claude Ship: agents that review, fix and approve PRs (Nov 23)

Anthropic released **Claude Ship**, a bundle of three agents for **GitHub pull requests**, available to **Claude Team and Enterprise** organizations. **Code Review** is the generally available piece. It runs several agents in parallel, verifies its findings to filter out false positives, and ranks bugs by severity. Anthropic says fewer than 1% of its internal findings were marked incorrect, and it puts the average review at roughly **$15–$25**. **PR Steward** (beta) fixes failing CI checks and merge conflicts and acts on reviewer feedback. **Claude Approvals** (beta) can auto-approve changes that match a team-defined policy, and Anthropic recommends starting it in **observe-only mode**. Teams pick a review depth (**Quick / Standard / Deep**), set spend limits and choose which changes go to a human. Developers can also trigger it with a **`/ship`** command in Claude Code. Anthropic warns that the tool can still miss bugs and security vulnerabilities.

- **Why this matters for you (developer/entrepreneur):** Review, CI fixes and approval have long been the slowest part of shipping. With Claude Ship, small teams can push more PRs without hiring reviewers. At $15–$25 per review, though, you'll want rules for which PRs get a Deep review and which get a Quick one.
- **Business/project idea:** Build a **"review-policy and cost governor"** SaaS that sits on top of Claude Ship. It would classify each incoming PR by risk (files touched, auth/payment paths, diff size) and route it to Quick, Standard, Deep or a human reviewer. It would also log how Claude Approvals' observe-only decisions compare with human decisions, so teams can see when auto-approval is safe to turn on. Sell it to engineering managers who need audit trails for SOC 2.

Sources: [TechCrunch](https://techcrunch.com/2026/11/23/anthropic-launches-claude-ship-letting-ai-agents-review-fix-and-approve-code-changes/) · [ITdaily](https://itdaily.com/news/software/claude-ship-ai-agents-code-review/) · [WOWTALE](https://en.wowtale.net/2026/11/25/236159/) · [ShiftDelete](https://shiftdelete.net/en/anthropic-claude-ship-code-review-approval)

---

## 2. Amazon buys Decart's AI optimization stack for a reported $7.5B to boost Trainium (Nov 23–24)

**Amazon** agreed to acquire the **Decart Optimization Stack** and hire Decart's team through **Annapurna Labs**, its chip unit. It is not buying Decart's AI models. **Bloomberg** puts the price at about **$7.5 billion**, which Amazon has not confirmed and which is nearly double Decart's ~$4B valuation in May. The goal is to make models run faster on **Trainium and Inferentia**. Decart was an early **Trainium3** customer, and Amazon had said Decart ran real-time video **4× faster at half the cost of GPUs**. Analysts see the deal as a software bet to close the gap with **Nvidia**, ahead of Amazon's plan to sell Trainium **outside AWS in late 2027**. Amazon hasn't said whether the optimization stack will become a customer-facing product.

- **Why this matters for you (developer/entrepreneur):** If Amazon turns this into compiler and runtime improvements on Trainium, the price gap between Trainium inference and Nvidia GPUs on AWS could widen in your favor. That matters most for real-time video, voice and other high-throughput workloads.
- **Business/project idea:** Build a **cost-arbitrage inference router** for open-weight models. Benchmark the same model on Trainium/Inferentia instances (via the AWS Neuron SDK) and on GPU instances, then send each request to the cheapest backend that meets its latency target. Re-run the benchmarks automatically whenever Neuron releases ship, so customers capture the gains as soon as Decart's work lands.

Sources: [TechCrunch](https://techcrunch.com/2026/11/24/amazons-decart-acquisition-is-a-bet-on-using-software-to-narrow-the-gap-with-nvidia-in-the-ai-chip-race/) · [GeekWire](https://www.geekwire.com/2026/amazon-is-buying-decarts-ai-chip-software-for-a-reported-7-5b-and-bringing-its-founders-aboard/) · [Futurum](https://futurumgroup.com/insights/amazons-decart-acquisition-aims-trainium-at-nvidia/) · [Yahoo Finance](https://finance.yahoo.com/technology/ai/articles/amazon-snaps-decart-ai-optimization-171423520.html)

---

## 3. Walmart (and Gopuff) let Meta's Muse agent shop for customers (Nov 24)

**Walmart** now lets shoppers use **Meta's Muse** AI agent to browse **Black Friday** deals (Nov 23–29), compare items and build carts. Users sign in to their Walmart account inside Muse. The integration runs on **Walmart's Agent Gateway**, launched in October, which lets outside AI assistants plug straight into Walmart's store. Shoppers can set **spending limits**, require **approval before purchase**, review the orders the agent places and delete its profile. Walmart says Muse can't see their purchase history. **Gopuff** joined with a similar integration. The move is a clear split from **Amazon**, which has been far more guarded about outside agents. Muse has been criticized for past unauthorized actions, including an Airbnb booking made without the user's go-ahead.

- **Why this matters for you (developer/entrepreneur):** Major retailers are now opening agent-facing commerce gateways. "Agent-readable" catalogs and checkout APIs are becoming a sales channel in their own right, much as SEO and mobile apps once did.
- **Business/project idea:** Build an **"agent gateway in a box"** for Shopify and WooCommerce merchants: an MCP server that exposes the catalog, inventory, cart and checkout, with built-in spending caps, approval hooks and analytics on agent-originated orders. Mid-size retailers could then copy Walmart's Agent Gateway and be listed in Muse, ChatGPT and Gemini shopping flows.

Sources: [TechCrunch](https://techcrunch.com/2026/11/24/walmart-teams-up-with-meta-to-bring-black-friday-deals-to-ai-agent-muse/) · [PYMNTS](https://www.pymnts.com/news/retail/2026/walmart-turns-to-metas-muse-to-power-black-friday/) · [MediaPost](https://www.mediapost.com/publications/article/419648/walmart-lets-meta-agent-autonomously-shop-black-fr.html) · [The Shelby Report](https://theshelbyreport.com/2026/11/24/gopuff-joins-walmart-in-letting-metas-muse-ai-agent-shop-for-customers/)

---

## 4. Google Search's AI Mode can now read your Wallet, with Drive and Gemini app next (Nov 23)

Google expanded **Personal Intelligence** in **Search AI Mode** beyond Gmail, Calendar and Photos. **Google Wallet** is rolling out now. AI Mode can track financial goals, flag ways to cut spending and help optimize **credit-card rewards**, and it can only *read* the data, not move money. **Google Drive** (docs, sheets, PDFs, e.g. building a tax-season plan) and the **Gemini app** follow "in the coming weeks." The feature is **opt-in**, limited to users over 18 with personal accounts, and reportedly **not available in the EU/UK**. A Personalization icon will show which data was used. Google hasn't said whether this data will be used for ad personalization.

- **Why this matters for you (developer/entrepreneur):** Search is becoming a personal assistant that reasons over users' own finances and documents. Generic personal-finance and document-Q&A apps are losing their edge, while niche, regulated or cross-platform tools stay defensible.
- **Business/project idea:** Target the users Google *can't* serve. Build a privacy-first **personal finance copilot for EU/UK users**, or for people who won't connect Wallet to an ad company. Use Open Banking APIs plus a local or self-hosted LLM to deliver the same rewards optimization and spending insights, with data residency guarantees as the selling point.

Sources: [TechCrunch](https://techcrunch.com/2026/11/23/google-searchs-ai-mode-can-now-tap-into-drive-and-wallet-for-more-personalized-responses/) · [PYMNTS](https://www.pymnts.com/news/artificial-intelligence/2026/google-enables-users-to-connect-wallet-to-ai-mode-for-personalized-responses/) · [Yahoo Tech](https://tech.yahoo.com/ai/gemini/articles/googles-ai-mode-getting-wallet-101610977.html)

---

## 5. ShellBench: top AI agents fail roughly 4 in 10 everyday tasks (Nov 24)

**ShellBench** is a new benchmark built from more than **10 million anonymized real-world agent interactions**. It was developed with researchers from the **OpenClaw Foundation, Parsewave, Hugging Face, Red Hat and UC Berkeley**. It found that even the best models from OpenAI, Anthropic and Meta **failed more than a third of realistic tasks**. Twelve models were tested across five agent harnesses, including **Claude Code and Codex**. Consistency was weak too: run three times under identical conditions, **GPT-6 Astra** got all three right less than half the time. Agents failed to account for a child's school pickup **79.5%** of the time and recommended duplicate or incorrect invoice payments **40.3%** of the time. About **10%** of otherwise-correct attempts broke at least one safety rule. *Per-model leaderboard scores circulating online could not be verified against the primary source.*

- **Why this matters for you (developer/entrepreneur):** If you ship agents to consumers or small businesses, expect failures to come from reliability and edge cases, not raw capability. Retries, confirmations and guardrails are product features, not afterthoughts.
- **Business/project idea:** Build an **agent reliability test harness as a service**. Customers upload their agent's tools and prompts, and the service runs each scenario N times in a ShellBench-style setup, measuring pass^k (all-k-correct) consistency and safety-rule violations. It then produces a report plus regression alerts for every model or prompt change.

Sources: [TechCrunch](https://techcrunch.com/2026/11/24/even-the-best-ai-agents-struggle-with-everyday-life/) · [Daily AI Brief](https://dailyaibrief.com/news/shellbench-ai-agents-everyday-tasks-43IZWCYN) · [AIToolly](https://aitoolly.com/ai-news/article/2026-11-25-why-even-the-best-ai-agents-still-struggle-with-everyday-life-tasks)

---

## 6. OpenAI says GPT-6 models can design proteins using only reasoning and code (Nov 24)

In a preprint, **OpenAI** reports that the **GPT-6 family** can design protein backbones and sequences without calling specialized biology models. An internal research model matched or beat specialist tools on many of **14 protein tasks**. In wet-lab tests with partner **Onava**, **35 of 322** selected **GPT-6.2**-designed proteins showed binding to their intended targets, across five targets (minibinders and antibody fragments). OpenAI acknowledges that the campaign still used specialist models (**Boltz-2, ESMFold2** and others) to filter candidates, and that specificity, stability and biological activity still need validation. *The results are self-reported.*

- **Why this matters for you (developer/entrepreneur):** General-purpose frontier models are becoming credible scientific design engines. Biotech tooling no longer has to be built only on narrow specialist models, which lowers the barrier for small teams.
- **Business/project idea:** Build a **"design-filter-order" protein pipeline for small labs**. GPT-6.2 proposes candidates through the API, open models (Boltz-2, ESMFold) score them, and the top hits are exported straight into DNA-synthesis and CRO ordering formats. Charge per campaign, targeting academic labs and seed-stage biotechs that can't afford in-house computational teams.

Sources: [OpenAI](https://openai.com/index/gpt-6-models-demonstrate-intrinsic-protein-design-capabilities/) · [Unite.AI](https://www.unite.ai/openai-reports-gpt-6-designs-proteins-with-reasoning-and-code/) · [The Techlantis](https://thetechlantis.com/news/openai-gpt-6-protein-design-lab-tests)

---

## 7. US blacklists Alibaba's Singapore unit Apex and Nvidia customer Megaspeed over chip-diversion risk (Nov 24)

The US Commerce Department's **BIS** added **Apex Enterprise Solutions**, Alibaba's Singapore unit, and six **Megaspeed**-linked entities in Singapore, Malaysia and Thailand to the **Entity List**. Exporters now need a license to ship them **AI chips** and other controlled technology. BIS cited a "significant risk" of diversion to unauthorized end users, not proof that chips were diverted. **Alibaba** calls the listing a mistake and says it will pursue legal options. Alibaba Group itself is not listed. Megaspeed rents out Nvidia-based compute and has been under US investigation since 2024.

- **Why this matters for you (developer/entrepreneur):** Southeast Asian GPU-rental capacity is now a compliance risk. If your startup buys cheap compute from regional neoclouds, check who ultimately owns them, or you could face sudden outages or sanctions exposure.
- **Business/project idea:** Build a **compute-provider compliance screener**. It would cross-reference GPU cloud vendors and their corporate parents against the BIS Entity List, OFAC and similar lists, monitor list updates daily and alert procurement teams. It could ship as an API for AI startups and as a plugin for GPU marketplaces.

Sources: [Quartz](https://qz.com/megaspeed-international-trade-blacklist-ai-chip-diversion-112426) · [StockAnalysis](https://stockanalysis.com/news/us-blacklists-alibaba-unit-megaspeed/) · [ChinaTechNews](https://www.chinatechnews.com/2026/11/24/133624-u-s-adds-alibaba-linked-firm-and-megaspeed-entities-to-export-blacklist-over-china-chip-diversion)

---

*Left out because they could not be adequately verified: a reported $110M seed round for robotics world-model startup Embo (earlier reports say ">$100M", and the close is unconfirmed), an OpenAI/Cisco "Shirudo" Linux tool, and a claimed SoftBank "worst day in two years" sell-off.*
