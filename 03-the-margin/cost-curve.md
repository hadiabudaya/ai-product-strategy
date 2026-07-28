# Cost Curve & Pricing Strategy

## Packaging Decision

* Leader: Centralized place for all public documents where users can search and chat with documents
* Filler: Recommendation of early signals where the clients get notified if something comes up and is relevant to their business
* Killer: Incumbent Contract Expiration & Renewal Tracking where users can see what contracts are going to be expiring
* Killer usage: 


## Cost Model

| Cost Category | Per-User/Month | Notes |
|--------------|----------------|-------|
| Inference (primary model) | $4.50 | ~200 RAG chats + 20 Strategic Briefs using Claude 3.5 Sonnet ($3.00/1M input tokens, $15.00/1M output tokens) |
| Inference (cascading/triage) | $0.80 | Bulk scanning & daily transcript classification using Claude 3.5 Haiku ($1.00/1M input tokens, $5.00/1M output tokens) |
| Infrastructure | $3.00 | Vector DB hosting (Pinecone/Qdrant), automated scrapers, background job queue workers |
| Data/storage | $1.20 | AWS S3 object storage for raw PDFs/transcripts and persistent embedding indexes |
| Human-in-the-loop | $0.00 | N/A |
| **Total AI COGS** | $9.50 | |

## Cascading Strategy
<!-- Cheap model → frontier model routing logic -->

**Triage model:** Claude 3.5 Haiku
**Frontier model:** Claude 3.5 Sonnet
**Routing rule:** Process 100% of incoming daily ingested documents through Claude 3.5 Haiku for noise removal and signal identification. Route to Claude 3.5 Sonnet only when a user initiates a RAG chat, requests a Strategic Brief (Killer feature), or when Haiku's confidence score falls between 0.40 and 0.75.
**Expected cascade ratio:** 85:15 (85% volume handled by Haiku, 15% escalated to Sonnet)

## Pricing Model

**Current pricing:** 
**Proposed AI pricing:**
**Model:** seat-based / usage-based / outcome-based / hybrid

## Stress Tests

| Scenario | Impact on Margin | Response |
|----------|-----------------|----------|
| Inference costs 3x | | |
| Heaviest segment doubles | | |
| Model provider raises prices 50% | | |

## Board One-Pager
<!-- Before/After: Old SaaS revenue vs. AI usage revenue for your product -->

**Before (traditional SaaS):**
**After (AI-enabled):**
**Net margin shift:**
