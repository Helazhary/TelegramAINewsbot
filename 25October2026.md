# Tech & AI Briefing — 25 October 2026

**Biggest story:** Anthropic launched **Claude Duet**, a proactive, always-on personal agent (research preview) — the "chief of staff" category is now a three-way race with Meta's Muse and OpenAI's Dots.

> Note: web coverage was mostly aggregators with some date inconsistencies; items below were each confirmed by 2+ sources. Unconfirmed items (e.g. a reported Meta–Sundial acquisition, an Agent Skills foundation donation) were dropped.

---

## 1. Anthropic launches Claude Duet, a proactive agent for Pro and Max users

Anthropic announced **Claude Duet** on 21 October as a **research preview** of a **proactive personal agent**. It sends a **morning brief** from connected apps, **checks apps every few hours** and alerts you when something needs attention, and works on assigned tasks while you're away. It runs on **Opus 5.5**, reuses your Claude **memory, skills and connected apps**, and **asks approval** before sending messages, paying, signing or deleting. Access is **US Pro/Max only** (web and iOS app; some outlets say Android too), and background checks count against plan limits. Anthropic admits it can misjudge urgency or miss mail that arrives between checks.

- **Why this matters for you (developer/entrepreneur):** Proactive "poll, triage, ask approval" is becoming the default agent UX, and the approval-gate pattern is now a reference design for safe autonomy. It also signals that horizontal personal-assistant products will be commoditised by the labs, so vertical niches matter more.
- **Business/project idea:** Build a **vertical "chief of staff" for a niche** (e.g. freelance agencies or solo e-commerce operators) using the Claude API with tool use/MCP connectors: a scheduled job polls Gmail, Stripe and the helpdesk every few hours, an Opus-class model ranks items by urgency, and drafts actions go into an approval queue (Telegram/Slack buttons) before anything is sent or paid. Differentiate with domain rules Duet won't have (invoice chasing, refund policies).

Sources: [MacRumors](https://macrumors.com/2026/10/21/anthropic-claude-duet/) · [Thurrott](https://thurrott.com/a-i/anthropic/343121/anthropic-announces-claude-duet-a-personal-ai-agent) · [iPhone in Canada](https://iphoneincanada.ca/2026/10/21/claude-duet-proactive-ai-agent-app) · [iPhoneSoft](https://iphonesoft.fr/2026/10/21/claude-duet-anthropic-agent-ia-toujours-actif)

---

## 2. Salesforce to buy Braze for ~$5.66B to deepen its AI/Agentforce push

On 20 October **Salesforce** agreed to acquire customer-engagement platform **Braze** for about **$5.66B enterprise value**, **$47.50 cash per share** (~58% premium). Braze's **real-time messaging and AI tools** will join Marketing Cloud, CRM, Data 360 and **Agentforce**. Closing is expected in Salesforce's **fiscal 2028**, pending shareholder and regulatory approval; break fees are $300M / ~$191M in specified cases. Braze stock jumped over 50%.

- **Why this matters for you (developer/entrepreneur):** Big platforms are paying real money for engagement data plus agent-ready messaging, validating the "AI-native lifecycle marketing" space. Braze/Salesforce integrators and competitors will see demand shifts during the long close.
- **Business/project idea:** Build an **AI campaign copilot for Braze-style APIs**: an LLM agent reads event/segment data via the Braze REST API, proposes segments and message variants, A/B-tests them, and reports lift. Sell it to mid-market Braze customers wary of Salesforce lock-in, or as a Braze-to-alternative migration tool.

Sources: [The Star (Reuters-sourced)](https://www.thestar.com.my/tech/tech-news/2026/10/20/salesforce-to-acquire-braze-in-a-566-billion-deal) · [The Next Web](https://thenextweb.com/news/salesforce-to-buy-marketing-platform-braze-for-5-7bn) · [BusinessDay](https://www.businessday.co.za/world/international-companies/2026-10-20-salesforce-to-buy-braze-for-566bn-in-ai-push/) · [ITdaily](https://itdaily.com/news/business/salesforce-braze/)

---

## 3. Gemini 4 Argon is generally available, with promo API pricing that doubles Dec 1

Google made **Gemini 4 Argon** (`gemini-4-argon`) generally available on **13 October** via the paid Gemini API and Google AI products. It has a **~1M-token context** and introductory pricing of **$2 / $10 per million input/output tokens through 30 Nov**, rising to **$4 / $20 on 1 Dec** (no free API tier). Benchmarks are vendor-reported; an independent comparison with Claude on developer tests found a split. Reports conflict on which subscriptions unlock AI Studio/Antigravity access.

- **Why this matters for you (developer/entrepreneur):** You have a ~5-week window of half-price frontier inference; benchmark it against your current model now and lock in cost assumptions before the December jump. Don't design unit economics around the promo price.
- **Business/project idea:** Build a **long-context codebase/document analyst** (whole-repo or whole-contract-set in one 1M-token prompt) and run a **model-routing layer** that sends heavy ingestion to Argon while the promo lasts and falls back to a cheaper/other model after Dec 1, with an eval harness proving equal quality.

Sources: [Let's Data Science](https://letsdatascience.com/news/gemini-4-argon-undercuts-claude-on-price-73027210) · [eesel.ai pricing breakdown](https://www.eesel.ai/blog/gemini-4-argon-pricing) · [DEV Community](https://dev.to/hassann/gemini-4-argon-is-out-5cpp) · [shattered.io](https://shattered.io/gemini-4-argon-malaysia-1m-tokens-price-doubles-dec-1-2026)

---

## 4. Tenstorrent raises $1.5B at $6.2B valuation for non-Nvidia AI hardware

On 19 October **Tenstorrent** (Jim Keller's open-RISC-V AI chip company) closed a **$1.5B Series E at a $6.2B post-money valuation**, led by **Trace Capital and Innovation X**, with ARK, Fidelity, Morgan Stanley, T. Rowe Price and Tether participating. Funds go to **volume manufacturing** and next-gen **Galaxy servers**. It reportedly chose funding over takeover talks with Intel and Qualcomm. Analysts note this shows investor appetite, not yet proven commercial scale.

- **Why this matters for you (developer/entrepreneur):** Credible non-Nvidia inference hardware could pressure GPU pricing and supply over time, and open software stacks (Tenstorrent's is open source) make early experimentation cheap.
- **Business/project idea:** Offer a **portability/benchmark service**: take customers' open-weight model deployments (vLLM/PyTorch), port and benchmark them on Tenstorrent and GPU backends, and publish cost-per-token reports to help teams negotiate or diversify compute.

Sources: [DatacenterDynamics](https://datacenterdynamics.com/en/news/ai-chip-startup-tenstorrent-raises-15bn-at-62bn-valuation) · [Dealroom](https://dealroom.co/news/163940-tenstorrent-raises-1-5b-series-e-doubling-valuation-to-6-2b/) · [Kyodo News PR Wire (company release)](https://kyodonewsprwire.jp/release/202610218369) · [AI Weekly](https://aiweekly.co/alerts/tenstorrent-raises-15b-series-e-at-62b-valuation-pulling-in-fidelity-ark-morgan)

---

## 5. DeepSeek's first outside funding round reportedly balloons past $12B (not confirmed closed)

**UNVERIFIED FINAL FIGURES.** DeepSeek's first external round, backed by **Tencent and CATL**, was reported by Reuters in June at ~50B yuan (~$7.4B). Newer Bloomberg-sourced reports say it is nearing **80B+ yuan (~$12B)**, possibly approaching 100B yuan, on strong demand after its latest model launch; one outlet reports $15B as already raised. Reuters could not verify the newer figure, and valuation estimates conflict. A **STAR Market IPO** is being prepared (CITIC Securities hired), but timing is undecided.

- **Why this matters for you (developer/entrepreneur):** A well-funded DeepSeek means continued pressure on API prices and more open-weight releases to build on, but treat geopolitical/compliance risk (data residency, procurement rules) as part of vendor choice.
- **Business/project idea:** Build a **cost-optimised inference gateway**: route bulk/low-risk workloads to DeepSeek-class open-weight models self-hosted in your own region and sensitive tasks to US frontier APIs, with per-request policy rules and logging for compliance.

Sources: [Khaleej Times (Bloomberg)](https://www.khaleejtimes.com/business/deepseek-to-raise-at-least-12-billion-in-tencent-backed-funding) · [SCMP](https://scmp.com/tech/big-tech/article/3355818/deepseek-nears-us7b-haul-first-ever-funding-round-backing-tencent-catl) · [TechNode](https://technode.com/2026/06/04/deepseek-in-talks-to-raise-7-billion-from-tencent-catl-and-other-investors/) · [The Daily Star](https://thedailystar.net/news/technology/news/chinese-ai-startup-deepseek-raises-15-billion-ahead-potential-ipo-4305031)
