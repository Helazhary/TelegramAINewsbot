# Tech & AI Daily Briefing — 12 November 2026

**Biggest story:** **Nvidia's board is reportedly weighing whether to remove CEO Jensen Huang**, with shares down about 8% after hours on Wednesday. No decision had been confirmed at the time of writing.

_Note: Only items confirmed by 2+ independent sources are included. Outlet pages could not be fetched directly in this run (network restrictions), so details come from search-result summaries of the linked articles. Yesterday's stories (Anthropic IPO range, Claude Sheets/Meetings, Businesses in ChatGPT, Gemini 4 Carbon, TPU 8tx) are not repeated._

---

## 1. Nvidia board reportedly weighing Jensen Huang's removal as CEO (no outcome confirmed)

The **Wall Street Journal**, as relayed by CBS, ABC and CNN, reports that **Nvidia's board met Wednesday to decide whether to remove co-founder and CEO Jensen Huang**. This follows the board's **independent investigation** into reports that Huang was the target of a foreign intelligence effort, and reported personal-conduct allegations. **Bloomberg** reports the board has engaged an outside firm to look for successors and may name an **interim chief**. Nvidia shares fell **about 8% after hours**. Separately, three House Republican committee chairs have asked Huang for a closed-door briefing and **threatened a subpoena**, and a securities lawsuit has been filed. **These are reports from unnamed sources. No board decision has been announced**, and sources differ on whether the board would act immediately. Nvidia reports Q3 earnings on **17 Nov**.

- **Why this matters for you (developer/entrepreneur):** Nvidia sets GPU supply, pricing and roadmap for almost every AI product. A leadership change will not alter CUDA or shipping hardware in the short term, but it adds uncertainty to allocation deals, export policy and AI-equity sentiment, a week before Anthropic's IPO.
- **Business/project idea:** A **GPU-portability audit tool**. It scans a codebase and infra config for Nvidia-only dependencies (CUDA kernels, TensorRT, NIM endpoints) and produces a costed migration plan to TPU, AMD or inference-API alternatives. Use a coding model to rewrite the easy paths automatically and sell it to startups whose investors now ask about single-vendor risk.
- **Sources:** [CBS News](https://www.cbsnews.com/news/nvidia-board-ceo-jensen-huang-china/) · [CNN live updates](https://www.cnn.com/2026/11/11/business/live-news/nvidia-jensen-huang-investigation-fallout) · [ABC News](https://abcnews.com/US/nvidia-board-reportedly-preparing-oust-ceo-jensen-huang/story?id=138062059) · [ABC News (subpoena)](https://abcnews.com/amp/Politics/house-republicans-issuing-subpoena-nvidia-ceo-jensen-huang/story?id=138022782)

## 2. OpenAI's Q3: ~$10B revenue, ~$10.9B adjusted operating loss (reported)

Investor documents seen by the **Wall Street Journal**, and reported by Reuters and Forbes, show **OpenAI's Q3 2026 revenue at about $10B**, up roughly **50%** from about $6.7B in Q2. The **adjusted operating loss widened to about $10.9B** from $10.1B. The figure reportedly excludes about $2.6B of stock-based compensation. Adjusted operating margin improved to **-109% from -150%**, and **enterprise revenue reportedly doubled** quarter over quarter. OpenAI has not published these numbers itself.

- **Why this matters for you (developer/entrepreneur):** OpenAI is still losing more than a dollar for each dollar of revenue. That makes current API prices and generous consumer tiers a subsidy that can change. The enterprise doubling shows where the paying demand is.
- **Business/project idea:** A **price-shock simulator for AI products**. Connect it to a company's LLM usage logs, model 2x–5x price increases or rate-limit cuts per provider, and show which features go margin-negative. Then recommend caching, smaller models or routing per feature. Sell to seed and Series A founders preparing board decks.
- **Sources:** [Forbes](https://www.forbes.com/sites/gabrielalinzainescu/2026/11/11/openai-revenue-hits-10-billion-as-losses-reach-109-billion/) · [Dataconomy](https://dataconomy.com/2026/11/11/openai-revenue-hits-10-billion-as-operating-losses-widen/) · [TipRanks](https://www.tipranks.com/news/openai-posts-steep-losses-even-as-quarterly-revenue-rises-to-10-billion) · [Exchange4media](https://www.exchange4media.com/digital-news/openai-q3-revenue-jumps-50-to-10-billion-but-operating-loss-widens-to-109-billion-160109.html)

## 3. Meta's Muse models arrive on Google Cloud

Three Meta models are now offered on **Google Cloud**: **Muse Wonder** (Meta's most capable model, aimed at complex software engineering), **Muse Spark 1.3** (a workhorse agentic model) and **Muse Ember** (an efficient multimodal model). Mark Zuckerberg announced it and Sundar Pichai publicly welcomed it. Sources differ on the access route: most say **Model Garden**, and others say **public preview via Vertex AI / Gemini Enterprise Agent Platform**. **Google Cloud pricing was not confirmed.**

- **Why this matters for you (developer/entrepreneur):** If you are on GCP you can now test Meta's frontier models under your existing billing, IAM and data-residency setup, next to Gemini and Claude. More models on one cloud makes multi-model routing easier.
- **Business/project idea:** A **coding-agent bake-off service** on GCP. Run a customer's real repo tasks (bug fixes, migrations, test writing) through Muse Wonder, Gemini 4 Carbon and Claude in identical sandboxes, score results against their CI, and deliver a per-task-type recommendation. Gemini's intro pricing ends 30 Nov, so the comparison is timely.
- **Sources:** [BusinessToday](https://www.businesstoday.in/technology/news/story/sundar-pichai-welcomes-mark-zuckerbergs-meta-ai-models-to-google-cloud-with-a-special-message-566892-2026-11-12) · [Dataconomy](https://dataconomy.com/2026/11/11/metas-ai-models-now-available-on-google-cloud/) · [NewsBytes](https://www.newsbytesapp.com/news/science/meta-s-muse-ai-models-now-available-on-google-cloud/story)

## 4. Databricks launches a new "always-on" Genie agent

Databricks announced a rebuilt **Genie** on 11 Nov. The agent can **run in the background on dedicated compute**, take **scheduled or event-triggered jobs**, follow up on missing information and handle several assignments at once, with users choosing which actions need approval. Admins can **restrict MCP tools, require approvals and set budgets and spending caps** through Unity governance. The press release says Genie is generally available, while **Genie Search, Ontology Manager and the always-on mode are in preview/beta**. Databricks' docs say Genie One and Genie Agents usage is **free for users until 31 Jan 2027**. Databricks claims **91% task accuracy** in one test and itself cautions that this came from an established deployment.

- **Why this matters for you (developer/entrepreneur):** Data platforms are becoming agent runtimes with built-in governance. If your customers are on Databricks, an agent that lives next to their governed data will be the default. Third-party tools need to plug in through MCP instead of asking for data exports.
- **Business/project idea:** Build **vertical MCP tool packs for Genie**, for example a "revenue ops" pack exposing CRM write-backs, dunning emails and quote generation. Genie handles the analysis on lakehouse data and your tools take the action, with approval gates mapped to Databricks' controls. Price per connected system.
- **Sources:** [Databricks press release](https://www.databricks.com/company/newsroom/press-releases/databricks-launches-new-always-genie-autonomous-ai-complex) · [IT Brief](https://itbrief.com.au/story/databricks-launches-always-on-genie-ai-agent-for-firms) · [Unite.AI](https://www.unite.ai/databricks-turns-genie-into-an-autonomous-enterprise-ai-coworker/) · [Databricks docs (pricing)](https://docs.databricks.com/aws/en/genie/monitor-cost)

## 5. United Airlines bans unauthorized AI agents from booking flights

United said on 11 Nov it is tightening booking and distribution rules to **block unauthorized personal AI assistants** from booking on its platforms, including **indirectly through travel agencies and aggregators**. Its **contract of carriage (Rule 5.H)** now lists AI agents under prohibited ticketing practices and lets United **cancel reservations** made or modified by them. AI tools may still **search and display** fares. United cites security, privacy and unintended purchases, and says it has not yet authorized any third-party agent. Bookings made by agents before 11 Nov will be honored. **Delta**, by contrast, permits authenticated AI assistants under safeguards.

- **Why this matters for you (developer/entrepreneur):** This is a clear precedent of a large consumer brand contractually blocking agentic checkout. Agents that act on websites without a partnership carry real risk for your users (cancelled tickets). Expect "authorized agent" programs to become the gate.
- **Business/project idea:** An **agent-permissions registry and compliance layer**. Maintain a machine-readable database of which merchants allow, restrict or ban AI-agent transactions (terms of service, contracts of carriage, robots-style policies), and expose an API that agent builders call before checkout to decide between "book", "hand off to user" or "deep-link". Use an LLM pipeline to monitor terms changes daily.
- **Sources:** [Bloomberg](https://www.bloomberg.com/news/articles/2026-11-11/united-blocks-ai-agents-from-booking-flights-ahead-of-holidays) · [PYMNTS](https://www.pymnts.com/news/artificial-intelligence/2026/united-airlines-blocks-ai-bots-from-booking-flights/) · [One Mile at a Time](https://onemileatatime.com/news/united-airlines-bans-ai-agents-protect-customers/) · [WTKR](https://www.wtkr.com/us-news/united-airlines-blocks-ai-assistants-from-booking-flights)

## 6. UK chip startup Fractile raises ~$720M at ~$7B valuation

London-based **Fractile**, which designs **AI inference chips** aimed at the memory bottleneck, raised a **Series C of about $720M at about $7B post-money**, up from about $1.1B in May. **Thrive Capital** co-led, with Founders Fund, Conviction, CapitalG, Lightspeed and the **UK government's sovereign AI fund** participating. The exact figures come from people familiar with the deal. The UK government says only "over £500M" at "over £5B". Fractile has **no production chip yet** and says it will ship first chips and systems **next year**. The FT reports **Anthropic** has shown interest as an early customer, which neither company has confirmed.

- **Why this matters for you (developer/entrepreneur):** Investors are paying heavily for alternatives to Nvidia in inference. If these chips deliver, expect cheaper and faster inference from 2027, which changes what is affordable (long-running agents, real-time voice and video).
- **Business/project idea:** An **inference benchmarking service for new silicon**. Publish independent tokens-per-second, latency and cost-per-token results for popular open models across Nvidia, TPU, Cerebras/Groq-class and upcoming chips such as Fractile's, and sell private benchmark runs on customers' own workloads to infra buyers.
- **Sources:** [TechCrunch](https://techcrunch.com/2026/11/11/with-720m-round-britains-fractile-gets-a-leg-up-in-the-race-for-ai-chips/) · [EU-Startups](https://www.eu-startups.com/2026/11/londons-fractile-secures-massive-e649-million-series-c-to-challenge-nvidia/) · [Yahoo Finance](https://finance.yahoo.com/technology/ai/articles/720m-round-britain-fractile-gets-193455349.html)

## 7. Google DeepMind releases AlphaGenome 2

DeepMind announced **AlphaGenome 2** on 11 Nov. It predicts how **DNA variants affect gene regulation in specific cell types and cell states**, instead of tissue averages, and can condition on a researcher's own **single-cell data**. It was trained on **100M+ single-cell profiles across 68 tissues**. On one immune dataset DeepMind reports recovering **30% of likely causal expression variants at 90% precision, versus 16%** for the fine-tuned original. It adds **DNA methylation** to existing readouts. It is **free for non-commercial research via the AlphaGenome API**, and companies can apply for a **private preview**.

- **Why this matters for you (developer/entrepreneur):** A free research API for cell-type-specific variant effects lowers the cost of building genomics tools. Commercial use needs the private preview, so apply early if you are in biotech.
- **Business/project idea:** A **variant-interpretation workbench for academic labs**. Users upload GWAS hits or patient variants, the tool calls the AlphaGenome API across relevant cell types, and an LLM writes a ranked, cited report of likely causal variants and suggested validation experiments. Start free for academia under the non-commercial terms and apply for the commercial preview to serve biotech.
- **Sources:** [Unite.AI](https://www.unite.ai/google-deepminds-alphagenome-2-predicts-cell-state-variant-effects/) · [OODAloop](https://oodaloop.com/briefs/technology/google-deepmind-unveils-alphagenome-2-to-bridge-single-cell-biology-and-human-genetics/) · [Digital Today](https://www.digitaltoday.co.kr/en/view/124629/google-deepmind-unveils-alphagenome-2-ai-to-pinpoint-causes-of-disease)

## 8. New York launches the first state-run program to independently test AI models

Governor **Kathy Hochul** announced on 10 Nov that the **New York Center for AI Responsibility and Research (NYCAIRR)** at **Binghamton University**, with 80+ scientists and Empire AI compute, will **independently evaluate the safety and security of advanced AI models**. Politico reports funding of a **$30M gift from Tom Secunda** plus **$25M from SUNY and the state**. It arrives before the **RAISE Act**, which requires large AI developers to **register with the state by 1 Jan 2027**. A key limit: researchers can test only **publicly released** models.

- **Why this matters for you (developer/entrepreneur):** State-level AI oversight is becoming operational, not just legislative. If you sell AI into New York, expect buyers to ask for evaluation evidence, and expect public third-party test results on the models you build on.
- **Business/project idea:** A **RAISE Act readiness kit** for AI companies. It provides a checklist, document templates and an automated eval harness that produces the safety documentation enterprise and public-sector buyers in New York will request. Offer it as a low-cost SaaS with a paid audit-prep tier.
- **Sources:** [Yahoo News / Politico](https://www.yahoo.com/news/politics/articles/york-hochul-launches-nation-first-130000835.html) · [Slashdot](https://yro.slashdot.org/story/26/11/10/2058226/new-york-launches-nations-first-state-ai-testing-program) · [FingerLakes1](https://www.fingerlakes1.com/2026/11/11/new-york-ai-safety-research-center-binghamton/)

---

## Also verified, in brief

- **CoreWeave Q3 2026:** revenue **$3.661B (+168% YoY)**, backlog **$132.5B**, full-year guidance raised to **$13.0–13.3B**, adjusted net loss $529M. Demand for AI compute is still outrunning supply. [CoreWeave IR](https://investors.coreweave.com/news/news-details/2026/CoreWeave-Reports-Strong-Third-Quarter-2026-Results/default.aspx) · [Motley Fool transcript](https://www.fool.com/earnings/call-transcripts/2026/11/10/coreweave-crwv-q3-2026-earnings-call-transcript/)

## Dropped / UNVERIFIED (not included as fact)

- **OpenAI retiring Advanced and Standard Voice on 11 Dec 2026:** seen in one newsletter and one search summary of an OpenAI post. No independent confirmation found. **UNVERIFIED.**
- **DeepMind agents formally verifying the Signal protocol:** one newsletter only. Searches found only the unrelated "Signal Shot" project. **Dropped.**
- **"New bill requires federal permission to train AI":** this is coverage of the Sanders–Casar bill (S.5493) introduced in **September**, not a new development.
- **Amazon Alexa agent by text message, Ring indoor drone, Apple background-assistant plans:** single-source or rumor-level in this run.
