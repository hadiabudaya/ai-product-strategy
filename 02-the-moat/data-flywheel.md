# Data Flywheel Map

> Score each loop 1-5. Your weakest loop is where competitors attack first.
> The four loops below are the M2 starting point - adapt if your product has 2 or 6 loops instead of 4.

## Flywheel Loops

| Loop | What It Measures | Score 1 | Score 5 | Score |
|------|------------------|---------|---------|-------|
| **Correction** | Do users fix AI outputs? Is that signal captured and reused? | No capture | Automated retraining | 3/5 |
| **Preference** | Does the product learn individual / team preferences over time? | Stateless | Deep personalization | 4/5 |
| **Domain Context** | Does usage in one area improve quality in adjacent areas? | Siloed | Cross-domain transfer | 2/5 |
| **Network** | Does each new user / team make the product better for everyone? | Isolated | Strong network effects | 2/5 |

### Correction Loop - 3/5
**What you capture today:** Explicit user feedback on flagged signals (e.g., sales reps marking an extracted transcript excerpt as "Not Relevant", correcting a mismatched municipal contact, or flagging a false positive intent score).
**How it compounds:** Direct user corrections continuously re-tune the underlying classification LLMs and named-entity recognition (NER) models. Over time, false positive intent flags drop, dramatically improving signal precision across specific municipal sectors (e.g., water infrastructure vs. IT procurement).

### Preference Loop - 4/5
**What you capture today:** User account configurations, accepted opportunity recommendations, targeted municipal agency choices, ideal deal thresholds, and specific solution keywords saved by sales teams.
**How it compounds:** As users accept or dismiss daily opportunity alerts, the recommendation engine maps subtle supplier preferences to early municipal discussion topics. The platform progressively serves higher-qualified, tailored lead signals that match each supplier's ideal customer profile (ICP) without requiring manual search tweaks.

### Domain Context Loop - 2/5
**What you capture today:** Cross-references between unstructured municipal council jargon (e.g., local agenda codes, line-item budget revisions, strategic plan phrases) and commercial product/service taxonomies.
**How it compounds:** As the model processes hundreds of thousands of municipal meeting transcripts across various regions, it builds an internal dictionary of pre-RFP indicators. Knowing that a specific council discussion topic in one municipality reliably leads to an RFP 6 months later allows the system to recognize that same pattern faster in other jurisdictions.

### Network Loop - 2/5
**What you capture today:** Anonymized, platform-wide interaction aggregate data showing which types of municipal signals lead to active buyer outreach and high proposal success rates.
**How it compounds:** As more suppliers interact with early signals across North America, the platform establishes fleet-level predictive indicators regarding municipal buying cycles. This collective intelligence powers platform-wide benchmark metrics—such as predicting municipal tender timelines—benefiting all users without exposing competitive vendor bidding strategies.

**Total Flywheel Score: 11/20**
**Weakest Loop:** Network Loop
**Fix for weakest loop:** Build an anonymized "Municipal Intent Index" that tracks early spending indicators by region and industry category. Using aggregate activity from across the platform, this index will automatically elevate high-confidence early signals to all users in that vertical.

---

## Encroachment Threat Assessment

### 1. Platform Encroachment
**Attacker:** OpenAI (SearchGPT / Operator) / Perplexity Enterprise
**Vector:** Native integration of deep web scraping, document parsing (council agendas/transcripts), and automated summarization into general workspace search tools at near-zero incremental cost.
**Time-to-threat:** 3–6 Months
**% of value at risk:** 60% (Raw data extraction and intent detection become baseline commodities).

### 2. Vertical Competitor
**Attacker:** StarBridge
**Vector:** Embedding native LLM scrapers across their massive, existing databases of government contracts, leveraging established enterprise sales relationships and CRM integrations.
**Time-to-threat:** 6–12 Months
**% of value at risk:** 80% (Risk of losing enterprise B2B sales teams who prefer an all-in-one incumbent platform).

### 3. Adjacent Expansion
**Attacker:** Salesforce / HubSpot (CRM Platforms)
**Vector:** Launching native "Public Sector Lead Discovery" AI agents inside the CRM that automatically flag municipal opportunities and auto-populate deal pipelines.
**Time-to-threat:** 12+ Months
**% of value at risk:** 40% (Loss of the workflow layer where reps draft outreach and track leads).

---

## 90-Day Encroachment Plan

*Your partner played the Big Tech attacker. What was their plan to kill you?*

**Attacker:** Big Tech AI Platform (e.g., OpenAI / Perplexity)
**Attack vector (target the weakest loop):** Exploiting weak **Network Loop (2/5)** and **Data Advantage (2/5)** by offering free, multi-modal web scraping across municipal video transcripts and PDF council minutes directly inside general chat search interface.
**Weeks 1-4 - what they ship:** A free "Government & Municipal Intelligence" plugin/agent that allows users to prompt, "Alert me whenever [City] council discusses [Cloud Security / Road Construction] in their meetings."
**Weeks 5-8 - how they poach users:** Bundling this capability into existing enterprise seat licenses (e.g., ChatGPT Enterprise / Perplexity Pro for Teams) at $0 extra cost, undercutting your standalone subscription fees.
**Weeks 9-12 - why users don't come back:** Users build custom custom GPTs / AI Agents directly inside their primary AI productivity workspace, centralizing their entire research workflow in one spot and making a single-point discovery tool redundant.
**Your defense:** Shift immediately from **discovery** to **workflow depth and execution**. Integrate directly with B2B CRMs (Salesforce/HubSpot) to automatically draft hyper-personalized outreach emails based on historical municipal buyer preferences, and build a proprietary **Correction Loop** that scores lead likelihood based on past closed-won bids.
