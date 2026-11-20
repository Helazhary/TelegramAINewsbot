# Daily Tech & AI Briefing — 20 November 2026

**Biggest story:** **Anthropic** is now a public company. It priced at **$83 a share**, raised **$81.3B** (the largest IPO on record), and closed its first Nasdaq day as **ANT** at about **$97**, up roughly 17%.

> Note: covers about 17–19 November. Figures are as reported. Benchmarks and cost claims are vendor numbers unless stated. Several primary sites (TechCrunch, The Neuron, aienews.org) could not be opened from this environment, so cross-checks rely on search results from independent outlets.

---

## 1. Anthropic's record IPO: ANT closes up ~17% on day one

**Anthropic** priced its IPO at **$83**, above the **$70–78** range. It sold **980M Class A shares** for **$81.3B**, beating **SpaceX's** June listing (~$75B) as the largest IPO ever. At pricing it was valued at about **$1.5T** fully diluted. The stock **opened at $111.50**, up 34%, then faded to close at **$97.17**. Reported closing market caps (~$1.25–1.27T) are on a different share basis from the $1.5T valuation, so don't compare the two directly. At the opening bell, CEO **Dario Amodei** said the company still intends to **pace AI development**.

- **Why this matters for you (developer/entrepreneur):** A public Anthropic has to report quarterly, so expect clearer disclosure on pricing, uptime and enterprise strategy. There will also be more pressure to grow revenue, which could mean more platform features, and more platform competition for startups that build on Claude.
- **Business/project idea:** An "AI-vendor intelligence" dashboard for CTOs and procurement teams. It pulls ANT, NVDA and other filings plus model-pricing changes into one feed, and uses Claude to summarise each 10-Q or 8-K into "what changes for customers": price moves, deprecations, capacity, region launches. Sell it as a subscription to companies with large LLM bills.
- Sources: [NPR](https://www.npr.org/2026/11/19/nx-s1-6042558/anthropic-ipo-breaks-records-100-billion) · [Forbes](https://www.forbes.com/sites/fionariley/2026/11/19/anthropic-ipo-live-nasdaq-futures-jump-2-ahead-of-record-stock-debut/) · [Fast Company](https://www.fastcompany.com/91645598/anthropic-ipo-what-time-trading-start-stock-price-live-update)

## 2. Google ships Gemini 4 Neon: a cheaper workhorse model (Nov 18)

**Gemini 4 Neon** costs **$3 / $15 per million tokens** (thinking tokens included). Cached input is **$0.15** (95% off) and **Batch/Flex** jobs are half price. It has a **1M-token context**, **four thinking levels** and **no free API tier**. It is aimed at **coding, knowledge work and science**, and reportedly is Google's fourth new model in about a month. It is also in the Gemini app for AI Pro and Ultra subscribers. Note the pricing calendar: **Gemini 4 Carbon/Argon** go from their intro **$2/$10** to **$4/$20 on 1 December**. That makes Neon the cheaper per-token option from then on. Google's claimed **32% per-task saving** applies at default thinking and has been disputed in third-party tests at the highest setting.

- **Why this matters for you (developer/entrepreneur):** If you run Gemini Carbon/Argon in production, re-run your own evals on Neon before 1 December, or your bill may double. Batch/Flex at half price suits offline jobs.
- **Business/project idea:** A "1M-context codebase auditor". Customers point it at a repo plus its docs, and Neon reviews everything in one call for security, licensing and architecture drift, run through **Batch** at $1.50/$7.50 and with **context caching** on repeat runs. Charge per audit, with weekly re-scans.
- Sources: [MLQ.ai](https://mlq.ai/news/google-releases-gemini-4-neon-at-3-per-million-input-tokens-its-fourth-new-model-in-a-month/) · [AI Weekly](https://aiweekly.co/alerts/google-launches-gemini-4-neon-at-315-per-million-tokens) · [Data Studios](https://www.datastudios.org/post/google-gemini-4-neon-launch-api-pricing-3-input-15-output) · [BigGo Finance](https://finance.biggo.com/news/7a4c8255-7eec-46a0-91d2-6bd980991a64)

## 3. Nvidia after Huang: record quarter, China shipments stopped, tighter neocloud financing

In its first earnings call **without Jensen Huang**, Nvidia reported **$115.8B revenue** (+103% YoY) and guided to about **$130B** next quarter. Interim CEO **Colette Kress** said Nvidia has **stopped shipping US-licensed Hopper chips (H200) to China** and left them out of guidance. Those chips brought in $2.4B last quarter, and Beijing had already been restricting H200 imports. Nvidia also **cut neocloud commitments to $32B** (from $36B). Its guarantees now apply only once neoclouds have **secured their own equity and debt**. Total guarantees stand at **$118B**. Shares fell ~3% on 18 November and more than 13% over the week. The board says it does **not** intend to reinstate Huang.

- **Why this matters for you (developer/entrepreneur):** Tighter funding for neoclouds (CoreWeave-style GPU clouds) could mean more volatile GPU-rental pricing and capacity. Avoid locking all your inference into a single small provider.
- **Business/project idea:** A GPU-capacity broker and failover layer. One API sits in front of several neoclouds and hyperscalers, tracks spot prices and availability, and moves inference or fine-tuning jobs automatically when one provider gets more expensive or runs out of capacity. Earn a margin on routed compute.
- Sources: [US News/Reuters](https://www.usnews.com/news/top-news/articles/2026-11-18/nvidia-stops-shipping-us-approved-ai-chips-to-china) · [Fox Business](https://www.foxbusiness.com/fox-news-tech/nvidia-halts-china-ai-chip-shipments-despite-us-approval) · [Quartz](https://qz.com/nvidia-stops-china-ai-chip-shipments-huang-exit-111826) · [Yahoo Finance](https://finance.yahoo.com/markets/stocks/articles/nvidia-trims-neocloud-commitments-ups-203454654.html) · [Motley Fool transcript](https://www.fool.com/earnings/call-transcripts/2026/11/18/nvidia-nvda-q3-2027-earnings-call-transcript/)

## 4. Microsoft MAI Code 2 lands in GitHub Copilot (Ignite, Nov 17)

Microsoft launched **MAI Code 2**, for complex engineering, and **MAI Code 2 Flash**, for fast high-volume work, in **GitHub Copilot**. They are available across VS Code, Visual Studio, JetBrains, Xcode, the Copilot CLI and the cloud agent. **Flash is on Copilot Free and Student plans** and is in preview on **Microsoft Foundry**. Microsoft claims **98% of GPT-6.1 Sol's score at 40% of its cost**, and **96% of Claude Opus 5.5 at 5% of the cost**. These claims have not been independently replicated, and per-token pricing reports conflict. Support on **OpenRouter, Vercel, Kilo and Open Code** is "coming soon."

- **Why this matters for you (developer/entrepreneur):** A cheap first-party coding model inside Copilot pushes down the price of AI coding. Third-party coding tools will need to compete on workflow and quality, not only model access.
- **Business/project idea:** Once it is on OpenRouter, build a **tiered coding agent**. **MAI Code 2 Flash** handles cheap work (lint fixes, test scaffolding, docs), and the task is escalated to Opus 5.5 or Sol only when tests fail twice. Sell it to agencies as "AI coding with a cost cap," with a per-repo cost dashboard.
- Sources: [GitHub Changelog](https://github.blog/changelog/2026-11-17-mai-code-2-and-mai-code-2-flash-in-github-copilot) · [The New Stack](https://thenewstack.io/microsoft-mai-code-2/) · [AlphaSignal](https://alphasignal.ai/news/microsoft-brings-mai-code-2-to-github-copilot-at-5-of-claude-s-cost)

## 5. Big US banks make customers liable for third-party AI agents

**Citi** updated its online terms so that customers are **liable for losses caused by third-party AI agents** they connect to their accounts. This includes agents that ignore instructions, exceed their permissions, or are **hacked and leak credentials**. Citi's **own** in-app AI tools are excluded. **PNC** (18 November) and **Citizens** have made similar changes, following **JPMorgan** and **Bank of America** in October. Whether federal **unauthorized-transfer protections** (Reg E) can be signed away like this for agent-initiated transactions is legally unsettled.

- **Why this matters for you (developer/entrepreneur):** If you build personal-finance or "agent that pays bills" products that ask for bank logins, your users now carry the risk. Expect churn and pushback unless you move to scoped, tokenised access.
- **Business/project idea:** An **"agent wallet" permission layer**. Agents never see bank credentials: they get scoped, revocable tokens with spending limits, payee allowlists and human approval above a set amount, all through **MCP** tools. Every action is logged for disputes. Sell it to fintech-agent developers as a compliance and safety layer, and to consumers as insurance-backed protection.
- Sources: [Yahoo Finance (TechCrunch)](https://finance.yahoo.com/technology/ai/articles/more-banks-says-customers-using-173210659.html) · [Startup Fortune](https://startupfortune.com/citi-pnc-and-citizens-tell-customers-they-own-any-loss-an-ai-agent-causes/) · [All About Cookies](https://allaboutcookies.org/citi-ai-agent-banking-liability) · [Digital Today](https://www.digitaltoday.co.kr/en/view/127747/us-major-banks-warn-on-external-ai-agents-customers-liable-if-problems-arise)

## 6. OpenAI says its models improved AMD GPU circuit designs by up to 14%

OpenAI reported that its models rewrote selected circuits in **AMD's flagship GPU IP**, finding up to **14% PPA (power/performance/area) gains** against heavily optimised baselines. It describes this as "roughly a year of progress in under five months." **Synopsys** tools checked that the rewrites still behaved correctly, and AMD reportedly used some changes in a design sent for manufacturing. OpenAI's own **Jalapeño** inference chip reportedly got ~10–13% area savings. A **GPT-Synopsys** model is in development. **Caveat:** these are OpenAI's own figures, with no breakdown and no AMD statement in the post. Treat 14% as a best case on selected circuits, not the whole chip.

- **Why this matters for you (developer/entrepreneur):** This is a credible signal that LLM agents can work on highly constrained engineering problems, not just app code, provided a rigorous verifier (formal equivalence checking) sits in the loop.
- **Business/project idea:** Use the same **"LLM + hard verifier"** pattern in a niche that is easier to enter, such as SQL query or database-index optimisation. An agent proposes rewrites, a verifier checks they return identical results on sample data, and only rewrites that pass and are faster are offered. Charge a share of the measured cloud-cost savings.
- Sources: [The Next Web](https://thenextweb.com/news/openai-models-amd-gpu-chip-design-14-percent) · [ANI](https://aninews.in/news/business/ai-models-deliver-up-to-14-chip-design-gains-in-amd-collaboration-openai-says20261119082527/) · [Analytics India Magazine](https://analyticsindiamag.com/ai-news/openai-and-amd-achieve-a-year-of-chip-design-progress-in-under-five-months) · [AI Weekly](https://aiweekly.co/alerts/openai-says-models-found-14-ppa-gains-in-amd-gpu-designs)

## 7. FBI warns ARTEX AI hacking framework can breach networks in under 3 hours

An FBI **FLASH advisory** (issued 13 November, widely covered this week) warns that the open-source **ARTEX** framework has been used by multiple threat actors since August against **finance, government and healthcare** targets. In the fastest cases it reached privileged access in **under three hours**. ARTEX has no model of its own: it **plugs into outside LLMs**. Researchers count **1,465–1,600+ exposed ARTEX consoles**. The advisory includes IOCs, and a community **detection signature pack** has been released.

- **Why this matters for you (developer/entrepreneur):** AI-driven attacks shrink the time defenders have to respond from days to hours. Leaked credentials and unpatched edge devices are the main way in, so tighten secrets scanning and patch cadence now.
- **Business/project idea:** An "AI red-team-as-a-service" for SMBs. Each week you run a controlled, authorised agentic attack simulation against the customer's external surface and cloud, then deliver a prioritised fix list. Use the FBI IOCs and the open detection pack to check that their monitoring actually fires.
- Sources: [BleepingComputer](https://www.bleepingcomputer.com/news/security/fbi-warns-artex-ai-hacking-tool-is-powering-global-cyberattacks/) · [CPO Magazine](https://www.cpomagazine.com/cyber-security/fbi-warns-cybercriminals-are-weaponizing-artex-ai-hacking-tool-to-accelerate-and-scale-cyber-attacks/) · [GitGuardian](https://blog.gitguardian.com/artex-fbi-alert/)

---

*Left out (could not verify across two sources, or too thin): reports of new US chip export-control tightening, and Satya Nadella's "unpatchable infrastructure" remark (single-source headline only).*
