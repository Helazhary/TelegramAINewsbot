# Tech & AI Briefing — September 22, 2026

**Today's biggest story:** **xAI shipped Grok 4.7**, a 2.1-trillion-parameter model built for coding and agentic work, landing the same day **Amazon blocked Meta's "Muse" AI shopping agent** from Amazon.com — escalating the platform-level battle over who controls agentic commerce — while **StepFun released a 600B-parameter open-weight Chinese model** and **OpenAI stood up an independent math advisory group** amid ongoing controversy over its Navier-Stokes claim.

---

## 1. xAI releases Grok 4.7, but benchmarks show it trailing Claude and GPT-6

**xAI** shipped **Grok 4.7**, its most capable model yet for coding and knowledge work, built on a new **2.1-trillion-parameter** base (up ~40% from Grok 4.6's 1.5T) with longer reinforcement-learning training and self-verification, plus supplemental training data from internal **SpaceX** engineering records. Pricing stayed flat at **$2/M input, $6/M output tokens** (a faster "Grok 4.7 Fast" variant is available via Cursor and Grok Build at 2x rates). On the independent Artificial Analysis Intelligence Index, Grok 4.7 scored **46**, landing mid-pack behind Claude Fable 5.1 and GPT-6 (53 each); on Terminal-Bench 4.0 it hit **26%** versus GPT-6 Astra's 60% and Claude Fable 5.1's 55%. It topped Hacker News with nearly 500 points.

- **Why this matters for you (developer/entrepreneur):** Grok 4.7 is meaningfully cheaper than frontier leaders but clearly behind on real coding/agentic benchmarks — useful as a cost-optimized tier, not a drop-in replacement for your primary coding agent.
- **Business/project idea:** Build a **model-routing layer** for AI coding tools that defaults to Grok 4.7 for simple/high-volume tasks (autocomplete, boilerplate, low-stakes agent loops) and escalates to Claude/GPT-6 only for complex multi-step work — capturing the cost savings without sacrificing quality on hard tasks.

Sources: [the-decoder](https://the-decoder.com/xai-launches-grok-4-7-at-bargain-prices-but-benchmarks-reveal-a-wide-gap-to-claude-and-gpt-6/), [kingy.ai](https://kingy.ai/blog/grok-4-7-release-features-pricing-access/), [Android Headlines](https://www.androidheadlines.com/2026/09/grok-4-7-ai-launch-coding-upgrades-pricing.html), [BenchLM.ai](https://benchlm.ai/models/grok-4-7)

---

## 2. Amazon blocks Meta's Muse AI agent from shopping on Amazon.com

**Amazon** began blocking **Meta's Muse** AI assistant from accessing Amazon.com on Sunday night after Meta declined a request to remove it, serving users an error citing violation of Amazon's Conditions of Use. Amazon alleges Meta never disclosed the access, that the agent doesn't identify itself, and that it appears to store customer login credentials; Meta counters that Muse has no visibility into passwords or payment details and keeps shared credentials in secure storage. This follows Amazon's earlier blocks of agentic-shopping tools from **OpenAI**, **Google**, and **Perplexity** — making it a pattern rather than an isolated dispute.

- **Why this matters for you (developer/entrepreneur):** Agentic commerce is hitting a hard platform wall — major retailers are treating third-party AI shopping agents as unauthorized bots regardless of the AI lab's size, so any product betting on "AI agent buys things on X's site" needs a fallback plan.
- **Business/project idea:** Build **official retailer-partnered shopping-agent APIs/plugins** (working with merchants directly rather than scraping/automating their checkout) — the access model retailers are actively blocking is exactly the gap a sanctioned integration layer could fill for both sides.

Sources: [TechCrunch](https://techcrunch.com/2026/09/21/metas-ai-agent-has-been-blocked-from-using-amazon-com/), [Bloomberg](https://www.bloomberg.com/news/articles/2026-09-21/amazon-blocks-meta-s-muse-ai-agent-from-its-retail-site), [GeekWire](https://www.geekwire.com/2026/amazon-blocks-metas-muse-ai-assistant-in-new-standoff-over-agentic-shopping/), [Forbes](https://www.forbes.com/sites/jonmarkman/2026/09/21/amazon-blocks-metas-new-muse-ai-agent-from-shopping-on-amazoncom/)

---

## 3. StepFun launches Step 5 Preview, a 600B open-weight agentic model

Chinese lab **StepFun** launched **Step 5 Preview**, a sparse Mixture-of-Experts model with **~600B total parameters** (~27B activated per token, 4.5% sparsity) on a 92-layer narrow-deep architecture, featuring a **1M-token context window** and native image input. It targets long-horizon agent workloads — coding, financial analysis, professional knowledge work — and scored **44** on the Artificial Analysis Intelligence Index. API access opened September 20 at **$1 per million input tokens**, with **model weights opening October 15**.

- **Why this matters for you (developer/entrepreneur):** Another credible, low-cost, soon-to-be-open-weight frontier-class model narrows the gap between US frontier labs and freely-deployable alternatives — relevant if you need to self-host or avoid per-token API lock-in for long-context agentic work.
- **Business/project idea:** Once weights land October 15, consider **fine-tuning or distilling Step 5** for a narrow, high-context vertical use case (e.g., legal document review, financial report analysis) where the 1M-token window and low base cost make self-hosted long-context inference economically viable in a way closed frontier APIs aren't.

Sources: [Pandaily](https://pandaily.com/stepfun-step-5-preview-600b-moe-1m-context), [runtimewire](https://runtimewire.com/article/stepfun-step-5-preview-600b-agent-model-pricing), [Eastern Herald](https://easternherald.com/2026/09/20/stepfun-step-5-preview-china-ai-model-open-weights/), [explainx.ai](https://www.explainx.ai/blog/stepfun-step-5-preview-pareto-frontier-launch-2026)

---

## 4. OpenAI forms independent math advisory group amid Navier-Stokes controversy

**OpenAI** announced an independent **Advisory Group on Mathematics and Artificial Intelligence**, hosted at Princeton's Institute for Advanced Study with nine initial mathematician members, to advise on reviewing and communicating OpenAI's math-related AI results and on academic/professional research standards — though the group has no authority to slow or redirect OpenAI's internal research pace. The move follows OpenAI's disputed early-September claim that an internal model resolved the **Navier-Stokes** Millennium Prize problem: mathematician **Tristan Buckmaster** alleged OpenAI's model may have absorbed his and a colleague's unpublished proof approach via chatbot interactions (which OpenAI denies), and multiple outlets (Nature, Scientific American, MIT Technology Review) report the underlying proof remains undisclosed and disputed by fluid dynamicists. **UNVERIFIED/DISPUTED:** OpenAI's claim of having "resolved" Navier-Stokes and 100+ other open problems is contested by the mathematics community and should not be treated as an independently confirmed result.

- **Why this matters for you (developer/entrepreneur):** This is a live case study in AI-generated research credit, provenance, and verification disputes — a preview of governance problems that will hit any domain where AI models train on or interact with unpublished human work product.
- **Business/project idea:** Build **provenance/verification tooling for AI-assisted research** (chat-log audit trails, idea-attribution tracking, independent proof-checking pipelines) — labs and academic institutions will need this exact tooling as more high-stakes "AI solved X" claims arrive without disclosed methodology.

Sources: [TechCrunch](https://techcrunch.com/2026/09/21/openai-forms-math-advisory-group-as-its-ai-resolves-more-than-100-open-problems/), [OpenAI](https://openai.com/index/advisory-group-on-mathematics-and-ai/), [Nature](https://www.nature.com/articles/d41586-026-02910-w), [Scientific American](https://www.scientificamerican.com/article/openai-claims-blockbuster-math-breakthrough-amid-swirl-of-controversy/)

---

*All items above were cross-checked across at least two independent sources. Stories already covered in prior briefings (Trump's "AI Force" announcement, CXMT's EUV-free DRAM milestone, clinician pushback on medical AI, Microsoft/HUMAIN's AI PC, Qwen3.8-Omni-Flash, Nvidia's chip-sales doubling guidance, Anthropic's Life Sciences Verification Program, the Plugin4Shell vulnerability, and Dario Amodei's "pace the frontier" essay) were intentionally omitted. Several searched items — Gemini 3.8 Flash/Live, Google's Finland data-center investment, and the Nvidia–Hugging Face acquisition — were excluded for being more than 48 hours old rather than fresh developments.*
