# Tech & AI Daily Briefing — 2 October 2026

**Biggest story:** OpenAI's DevDay (29 Sept) put **always-on agents ("dots")** inside ChatGPT and launched **GPT-6.1 Sol**, a near-frontier agentic-coding model at one-fifth of GPT-6 Astra's token price.

> Reliability note: the web-fetch tool was blocked for outlet front pages (TechCrunch, TLDR, etc.), so this briefing is built from search results only. Items are cross-checked across 2+ independent results unless marked UNVERIFIED. Several items are from the last few days rather than strictly the last 24 hours, because that is where the freshest verifiable news sits.

---

## 1. OpenAI DevDay: "dots" always-on agents, ChatGPT Space, plugin extensions

OpenAI made **20+ announcements** at DevDay on 29 Sept. The headline is **dots**: **always-on agents** inside ChatGPT. Each one reportedly runs on **GPT-6 Astra**, gets its own **cloud computer and browser**, works toward your goals continuously, learns from feedback, and connects to **4,000+ apps**. OpenAI also announced **ChatGPT Space**, a collaborative workspace for dots, pages, presentations and living documents, which puts it in direct competition with Microsoft 365 and Google Workspace. **Plugin extensions** let developers ship full apps that feel native to ChatGPT and are distributed through OpenAI. A new **Pro 500** tier adds an **Ultrafast** speed tier across ChatGPT and Codex.

- **Why this matters for you (developer/entrepreneur):** Plugin extensions are a new distribution channel inside ChatGPT, and the agent-as-coworker pattern is now a mainstream product category. Vertical agent products will have to differentiate on domain depth, not on "an agent that browses".
- **Business/project idea:** Build a niche plugin extension (for example, a bookkeeping or compliance-check app for freelancers) that dots can call as a tool. Expose a clean API with structured outputs, and let each user's dot run the recurring monthly workflow. You charge a subscription for the plugin, and OpenAI handles distribution.

Sources: [Axios](https://www.axios.com/2026/09/29/openai-dev-day-2026-dots-space-sol) · [CNBC](https://www.cnbc.com/2026/09/29/openai-devday-2026-live-updates.html) · [BGR](https://www.bgr.com/2272332/openai-devday-2026-announcements/) · [9to5Mac](https://9to5mac.com/2026/09/29/openai-teases-20-announcements-at-devday-watch-live/)

## 2. GPT-6.1 Sol: near-Astra agentic coding at ~1/5 the price

OpenAI introduced **GPT-6.1 Sol**, an upgrade to GPT-6 Sol that nearly matches **GPT-6 Astra** on **agentic coding, computer use and professional work** at **one-fifth of Astra's input and output token prices**. Its predecessors, GPT-6 Sol and the smaller GPT-6 Luna, were already rolling out to **GitHub Copilot** (Sol on Pro+/Max/Business/Enterprise, Luna on Pro and up) with usage-based billing. Whether 6.1 Sol itself is in Copilot yet is **UNVERIFIED**. Sources use "GPT-6 Sol" and "GPT-6.1 Sol" inconsistently, so check OpenAI's docs for exact model IDs.

- **Why this matters for you (developer/entrepreneur):** Frontier-class agentic quality at a fifth of the price changes the unit economics of long-running coding and computer-use agents. Re-benchmark your current model choice.
- **Business/project idea:** Run an "overnight maintenance agent" service for small dev teams. It uses Sol via the API to triage dependency updates, fix failing tests and open PRs on a schedule. At ~1/5 Astra pricing you can offer flat per-repo monthly pricing with healthy margins. Route hard tasks to Astra and routine ones to Sol/Luna.

Sources: [BenchLM DevDay recap](https://benchlm.ai/blog/posts/openai-devday-2026) · [Axios](https://www.axios.com/2026/09/29/openai-dev-day-2026-dots-space-sol) · [Technobezz (Copilot rollout, GPT-6 Sol/Luna)](https://www.technobezz.com/news/openai-gpt-6-sol-luna-github-copilot) · [aipicks.jp](https://aipicks.jp/news/20260923-github-copilot-gpt-6-2-luna-sol)

## 3. Anthropic's Claude Opus 5.5: cheaper, faster, 1M context (released 22 Sept)

Anthropic's **Claude Opus 5.5** shipped 22 Sept on the Claude Platform, **AWS, Google Cloud and Azure**. It is priced at **$4 / $20 per million tokens**, down 20% from Opus 5, and Anthropic says typical workloads cost about **40% less**. Cache reads are down 60%. Output is **30%+ faster**, with a **1M-token context** and up to **128K output**. A **fast mode** doubles speed at $8 / $40. Anthropic cites a **680,000-line code migration finished in under a day**, which is a vendor claim. It reportedly beats Claude Fable 5.1 on agentic coding, computer use and knowledge-work benchmarks. This is not from the last 24 hours, but it is the other half of the current price-performance race.

- **Why this matters for you (developer/entrepreneur):** Cheaper cache reads and a 1M context make whole-repo or whole-corpus agents economically viable. Prompt-caching-heavy designs get a big cost cut.
- **Business/project idea:** A legacy-code migration service (COBOL/Java 8/AngularJS to modern stacks). Load the whole codebase into the 1M context with cached reads, plan the migration, then run tests in a loop. Sell it as a fixed-price migration with a human review gate.

Sources: [Datanorth](https://datanorth.ai/news/anthropic-releases-claude-opus-5-5) · [Inc42](https://inc42.com/buzz/anthropic-launches-claude-opus-5-5-touts-40-lower-running-costs/) · [BetaNews](https://betanews.com/article/claude-opus-5-5-launch-price-cut/) · [Free Press Journal](https://www.freepressjournal.in/tech/anthropic-launches-claude-opus-55-its-most-powerful-model-yet-at-40-lower-cost)

## 4. Meta's Muse agent and Business Agent Platform

Meta launched **Muse** on 8 Sept as a **personal AI agent** in the US (iOS, Android, web, WhatsApp). It can send emails, book travel, fill forms, lower bills and make purchases, and it integrates with **Shopify's catalogue**, Shop Pay/PayPal and retailers such as Walmart and Best Buy. Meta's Alexandr Wang said Meta wants Muse to connect with **small businesses**, and the **Business Agent Platform** lets businesses connect hundreds of systems (Shopify, Zendesk, etc.) so agents can act on their behalf. A report of a further expansion to small businesses with 14+ integrations, including Slack and Dropbox, appeared in only one source, so it is **UNVERIFIED**.

- **Why this matters for you (developer/entrepreneur):** Consumer agents from Meta and OpenAI will increasingly transact with merchants. Your storefront or service needs to be agent-readable and agent-actionable.
- **Business/project idea:** An "agent-readiness" service for SMB e-commerce. It audits product feeds, availability and policies, then publishes structured, agent-friendly endpoints for Muse-style shoppers, with monitoring of how often agents succeed in checkout.

Sources: [TechRepublic](https://www.techrepublic.com/article/news-meta-muse-ai-agent-us-launch/) · [Engadget](https://engadget.com/2253133/meta-reveals-its-ai-agent-that-can-shop-send-emails-and-plan-trips-on-your-behalf/)

## 5. Instinct (invite-only AI assistant) reportedly raising $1B at ~$10B valuation

**Instinct**, an invite-only personal AI assistant (founder Noah Shinn, ex-Sierra) with 100K+ users, is **reportedly raising $1B at about a $10B valuation**, up from $2.5B at its Series B in late August. Sequoia and Benchmark are said to be leading. Sources differ on whether the round has closed: a TechCrunch headline says it **raised**, while other reports say **in talks** with terms not final. Treat the round as **partially unverified**.

- **Why this matters for you (developer/entrepreneur):** Investors are paying large premiums for consumer agents that execute tasks (shopping, travel, cancellations), and demand is outrunning capacity.
- **Business/project idea:** Build a narrow "execution agent" for one painful chore, such as subscription cancellation and bill negotiation for a specific market or language. Use a computer-use model plus a human-fallback queue, and charge a percentage of savings.

Sources: [TechCrunch headline (via search)](https://techcrunch.com/2026/09/28/viral-ai-agent-instinct-raises-1b-series-c-at-a-10b-valuation/) · [AI Weekly](https://aiweekly.co/alerts/business-insider-profiles-noah-shinn-as-instinct-ai-talks-10b-valuation-invite) · [Digg/The Information](https://digg.com/tech/ee37a030-fd03-419b-94cd-0c93c57cfafe)

---

**Dropped as unverified or conflicting:** a claim that GPT-6.1 Astra was cancelled over safety tests (sources conflict on Astra's status); Reddit shutting RSS feeds (only unrelated or old results); Reco's "$55M Series B" and Doxx.net's "$38M" (not corroborated by independent sources).
