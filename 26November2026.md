# Daily Tech & AI Briefing — 26 November 2026

**Biggest story:** Within hours of each other, the US Treasury's **FinCEN** took systems offline after **unauthorized access**, and reports surfaced of an intrusion at the **CIA, NGA and ODNI**. Investigators reportedly suspect a **repurposed AI security tool** was used in the intelligence breach. That attribution is **UNVERIFIED**.

> Note: I could not open several digest sites from this environment (The Neuron, DEV Community), so cross-checks rely on search coverage from several outlets. Benchmarks are vendor-reported unless stated. Items that were in the 24–25 Nov briefings (Huang reinstated, CrowdStrike–Zscaler, Claude Ship, Muse shopping, OpenAI protein design) are not repeated here.

---

## 1. FinCEN breach follows a reported intrusion at the CIA, NGA and ODNI (Nov 24–25)

The Treasury's financial-crimes bureau, **FinCEN**, confirmed a **cybersecurity incident** in which an intruder gained **unauthorized access** to a limited subset of its systems. It took some systems offline as a precaution. The **BSA E-Filing** site stayed up, and a FinCEN official told Reuters there was no evidence that the **Bank Secrecy Act** or **beneficial-ownership databases** were breached. Hours earlier, reports said attackers had reached an **open-source intelligence analysis system** shared by the **CIA, NGA and ODNI**; officials say no classified data was taken. According to the New York Times, sources say investigators suspect **Artex**, an open-source **AI defensive tool** that was **repurposed for offense**. That claim is **UNVERIFIED**, and nobody has established that the two incidents are linked.

- **Why this matters for you (developer/entrepreneur):** If AI-assisted attacks shorten the time from break-in to damage, defenders need faster detection and tighter control over what agents and service accounts can access. Expect government and enterprise buyers to spend more on this.
- **Business/project idea:** Build an "agent-speed" anomaly detector for identity and API logs. It would learn each service account's normal call patterns and flag the bursty, systematic enumeration that automated attackers produce. Run it on your cloud provider's audit-log streams and sell it first to regulated mid-market firms, such as fintechs that file with FinCEN.
- Sources: [ABC News](https://abcnews.com/US/treasurys-fincen-cybersecurity-incident-includes-unauthorized-access-systems/story?id=138432822) · [Newsweek](https://www.newsweek.com/treasury-financial-crime-unit-cyber-incident-fincen-12766120) · [BleepingComputer](https://bleepingcomputer.com/news/security/hackers-reportedly-breached-cia-intelligence-analysis-system) · [Cybernews](https://cybernews.com/security/us-government-cyberattacks-treasury-cia-fbi/) · [The Decoder](https://the-decoder.com/back-to-back-cyber-incidents-at-us-financial-investigators-and-spy-agencies-follow-a-string-of-federal-hacks-and-outages/)

## 2. ChatGPT and Codex will share one usage meter on paid plans (announced Nov 25; starts December)

OpenAI says **Plus, Pro and Business** subscribers will draw on a **single token-based usage pool** for both **ChatGPT and Codex**, as Work's agent features fold into the main ChatGPT experience. Because the pool is **measured in tokens**, advanced models and long agent tasks use it up faster. **Instant chat is exempt.** Combined remaining usage and reset times will appear under **Settings → Usage**. OpenAI hasn't published the size of the pooled allowance. Some outlets say December; Notebookcheck says no exact start date was given.

- **Why this matters for you (developer/entrepreneur):** If you use Codex heavily, a long day of chatting can now eat into your coding budget. Track your token use, and move predictable batch coding jobs to the API, where costs are metered and predictable.
- **Business/project idea:** A "usage budgeter" browser extension or CLI. It would estimate the token cost of each ChatGPT or Codex task before you run it, warn you when you're close to your reset limit, and suggest moving large jobs to a cheaper API model through a simple router. Sell it to solo founders and small dev teams on Plus or Pro.
- Sources: [Android Authority](https://www.androidauthority.com/chatgpt-codex-shared-usage-limits-3739254/) · [Notebookcheck](https://www.notebookcheck.net/ChatGPT-and-Codex-will-share-one-usage-limit-starting-in-December.1440897.0.html) · [MLQ.ai](https://mlq.ai/news/openai-merges-chatgpts-chat-and-work-tabs-heavy-users-may-hit-limits-sooner/)

## 3. Cognition releases SWE-2.1, an RL-trained coding model, free on Devin for a limited time (Nov 24)

**Cognition** released **SWE-2.1**, trained with **pure reinforcement learning on Kimi K3**. Reported scores are **50.0% on Terminal-Bench 4.1** and **41.3% on FrontierCode 2.0**. It is available in **Devin Cloud, Devin Desktop** (formerly Windsurf) and the **Devin CLI**, with **Low–Max reasoning-effort** levels. A **Cerebras-hosted fast variant** runs at about **600 tokens/s**, versus about 60 for the standard model. It's **free on self-serve plans until Dec 8**, after which Devin's docs list **$0.50 / $2.50 per million tokens** (input/output). A separate **SWE-2.1 Cyber** variant has looser safeguards and is meant for security scans.

- **Why this matters for you (developer/entrepreneur):** You get a cheap coding model in a commercial product, built on an open-weight base, plus two free weeks to test it against your current agent on real tickets.
- **Business/project idea:** A "PR triage on rails" service. The fast SWE-2.1 variant would handle the high volume of small fixes, such as lint, type errors and dependency bumps, through the Devin CLI in CI, and only hard tickets would go to a frontier model. Charge per merged PR and keep the margin from the low per-token price.
- Sources: [Cognition on X](https://x.com/cognition/status/2125305349414523061) · [Devin Docs – Models](https://docs.devin.ai/desktop/models) · [Sulat AI & Tech News](https://news.sulat.com/2026/11/25/devin-swe-2-1/) · [Superpower Daily](https://superpowerdaily.com/posts/cognition-releases-swe-2-1-with-a-claimed-10-faster-cerebras-variant)

## 4. EU proposes a €50B Sovereign Tech Equity Fund for AI and quantum (Nov 25)

The **European Commission** proposed a **Sovereign Tech Equity Fund** with a target size of **€50 billion**. It would make **long-term, high-risk equity investments** in European **AI and quantum** companies and aims to bring in up to **€6 of private capital for every public euro**. Tech chief **Henna Virkkunen** presented it alongside a draft **Quantum Act** that includes **procurement preferences** for European technology. The Commission said this is "not a blanket requirement" that every component be made in the EU. It is a **proposal**, and member states and Parliament still have to approve it.

- **Why this matters for you (developer/entrepreneur):** EU-based AI and quantum startups may soon have access to a large new source of equity capital, and "sovereign" procurement preferences could favour European vendors in public tenders.
- **Business/project idea:** A "sovereign stack readiness" tool for EU startups. It would scan a company's infrastructure and AI vendors (models, clouds, chips), map where each one is from and where data goes, and produce the compliance and positioning documents that fund applications and public tenders will likely ask for.
- Sources: [France 24 / AFP](https://www.france24.com/en/live-news/20261125-after-ai-eu-bets-on-quantum-as-next-big-thing) · [TechXplore](https://techxplore.com/news/2026-11-eu-billion-euro-investment-ai.html) · [Archyde](https://www.archyde.com/eu-unveils-e50-billion-sovereign-tech-fund-for-ai-quantum-computing/)

## 5. US jury convicts Huawei of trade-secret conspiracy and bank fraud (Nov 24)

A **Brooklyn federal jury** found **Huawei** and three subsidiaries (**Huawei Device, Futurewei, Huawei Device USA**) guilty of **conspiracy to steal trade secrets**, **bank and wire fraud**, **money-laundering conspiracy** and **IEEPA (Iran sanctions) violations**. It **acquitted** them of the **racketeering (RICO)** charge. Huawei called the verdict without merit and is expected to appeal.

- **Why this matters for you (developer/entrepreneur):** This adds to US–China tech decoupling. If your hardware, telecom or supply chain depends on Huawei-linked parts or partners, expect more vendor-risk questions from US customers and investors.
- **Business/project idea:** A supply-chain screening API. It would check a bill of materials or vendor list against US entity lists, court outcomes and sanctions data, using an LLM to resolve subsidiaries and aliases, and return a risk score that procurement teams can use in their ERP.
- Sources: [PBS NewsHour / AP](https://www.pbs.org/newshour/nation/u-s-jury-finds-chinese-tech-giant-huawei-guilty-of-conspiracy-to-steal-trade-secrets-bank-fraud) · [Al Jazeera](https://www.aljazeera.com/economy/2026/11/24/chinese-tech-giant-huawei-found-guilty-of-conspiracy-to-steal-trade-secrets) · [The Next Web](https://thenextweb.com/news/huawei-convicted-trade-secrets-bank-fraud)

## 6. Sakana AI's Namazu Small: a 30B MoE that beats a 120B model on search tasks (Nov 25)

**Sakana AI** announced **Namazu Small**, a **30B mixture-of-experts** model with about **3B active parameters**, built on **NVIDIA's Nemotron 3 Nano**. Sakana reports a **25-benchmark average of 60.1**, compared with **56.2** for the **120B Nemotron 3 Super**. The gains are mostly in **web research and long-document** tasks: **BrowseComp 73.5 vs 36.1**. It is weak on **built-in factual recall** (SimpleQA Verified 6.8). Sakana promises **on-prem availability in December**; it hasn't announced an API, weights or a license. All scores are vendor-reported.

- **Why this matters for you (developer/entrepreneur):** The results suggest small, cheap models can do agentic search well if you give them retrieval. Don't rely on them for facts they have to remember, so always connect a search or RAG tool.
- **Business/project idea:** An on-prem "research analyst" appliance for Japanese or regulated enterprises. Namazu Small (once it ships) or a similar small MoE would run on one workstation, connected to internal document search and a web-search API, to produce cited due-diligence or compliance briefs without data leaving the building.
- Sources: [AlphaSignal](https://alphasignal.ai/news/sakana-ai-s-30b-namazu-small-beats-nvidia-s-120b-model-on-25-benchmarks) · [Emergent](https://emergent.sh/news/sakana-s-30b-namazu-small-beats-nvidia-s-120b) · [Superpower Daily](https://superpowerdaily.com/posts/sakana-ai-introduces-a-30b-model-it-says-outperforms-nvidia-s-120b-rival)

## 7. DeepMind says AI agents now direct part of the compute for Gemini experiments (podcast, ~Nov 19–25)

DeepMind research VP **Koray Kavukcuoglu** said on **Google DeepMind: The Podcast** that **AI agents control part of the lab's compute** and **run experiments for upcoming Gemini models on their own**. He added that full **recursive self-improvement** is still far off. He also said DeepMind **does not reward chain-of-thought** during training, so agents' reasoning stays readable. No share of compute was given, and the episode date varies between reports.

- **Why this matters for you (developer/entrepreneur):** "Agents running ML experiments" is now happening inside a frontier lab. The same pattern (propose, run, evaluate, iterate under a budget) applies to hyperparameter sweeps, A/B tests and data-pipeline tuning.
- **Business/project idea:** An "autonomous experiment runner" for small ML teams. An agent would read the experiment backlog, launch sweeps on rented GPUs under a hard dollar budget, log results to W&B or MLflow, and write a daily summary of what to try next. Charge a percentage of the compute it manages.
- Sources: [Emergent](https://emergent.sh/news/deepmind-ai-agents-now-control-gemini) · [Oossa](https://oossa.com/en/google-lets-ai-agents-run-gemini-experiments-but-self-improvement-is-distant) · [ExplainX](https://explainx.ai/blog/google-deepmind-gemini-agents-training-compute-koray-kavukcuoglu-november-2026)

## 8. Nvidia RTX Spark mini PCs for local AI go on sale from ASUS, Dell and MSI (this week)

The first **RTX Spark** compact desktops are now **on sale**. They use Nvidia's **Arm-based N1X** chip with up to **128GB of unified memory**, **10GbE** and **PCIe Gen 5 M.2**. Reported prices: **MSI EdgeMesa N AI+ from $4,399** (64GB) or **$7,499** (128GB), and **ASUS ProArt GR1X from $4,499**. A Dell XPS model is also available. **Acer, GIGABYTE, HP** and Microsoft's **Surface RTX Spark Dev Box** are still to come.

- **Why this matters for you (developer/entrepreneur):** 128GB of unified memory on a desk means you can run sizeable open-weight models (including MoEs like item 6) locally for private inference and agent development, with no cloud bill.
- **Business/project idea:** "Private AI in a box" for law firms, clinics or accountancies. You'd preconfigure an RTX Spark mini PC with a local open-weight model, a RAG index over the client's documents and an MCP-based assistant, then sell it as hardware plus a monthly managed-update subscription.
- Sources: [NVIDIA Blog](https://blogs.nvidia.com/blog/rtx-spark-desktop-local-ai-available-now/) · [The Next Web](https://thenextweb.com/news/nvidia-rtx-spark-compact-desktops-asus-dell-msi-local-ai) · [Windows Report](https://windowsreport.com/?p=1516312)

---

**Dropped as unverified or not confirmed:** a reported Axelera AI $400M raise (search only found its $250M round in Feb 2026), a "$25B Dell buyback" (not found), an Anthropic "58 companies / 300 deployments" study (not found), and Meta Muse working inside Instagram DMs (coverage only confirms Muse on Instagram profiles).
