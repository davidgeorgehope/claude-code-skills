# Battlecard Generator

Generate a structured, sales-ready competitive battlecard for a named competitor. Battlecards are **internal-only** documents designed to arm field teams with positioning, depositioning, trap-setting questions, and objection handling.

## Arguments

$ARGUMENTS should be:
- A competitor company name (e.g., `Datadog`, `Splunk`, `Dynatrace`, `ClickHouse`)
- Optionally, a solution area focus: `observability`, `security`, or `search`
- Optionally, a file path to existing competitive intel to incorporate

## Instructions

### Step 1: Research the Competitor

Before writing anything, gather current intelligence. Run 5-8 web searches covering:

1. **Company fundamentals** — founding year, HQ, funding/public status, ticker, recent revenue
2. **Core technology and architecture** — open source vs proprietary, deployment model, underlying tech
3. **Product portfolio** — which solution areas they cover (observability, security, search)
4. **Recent news** — acquisitions, product launches, pricing changes, leadership changes
5. **GTM motion** — PLG vs enterprise sales vs channel, typical deal size, target persona
6. **Pricing model** — per-host, consumption, per-seat, tiered; look for public pricing pages and customer complaints
7. **Known weaknesses** — G2/Gartner Peer Insights reviews, Reddit threads, community complaints
8. **Head-to-head vs Elastic** — any publicly available win/loss context

If the user provided existing competitive intel (file or pasted content), prioritize that over web research. Use web search to fill gaps and verify freshness.

### Step 2: Generate the Battlecard

Produce output in the following structure. Every section must be present. Write in crisp, direct language — this is for salespeople mid-deal, not blog readers.

---

## Battlecard - [Competitor Name]

**FOR INTERNAL USE ONLY — DO NOT DISTRIBUTE**
Last updated: [current date]

---

### Competitive Solution Areas Covered

[Check which apply: Search ▪ Observability ▪ Security]

---

### Company Overview

[2-3 sentence summary of who they are, what they do, and why they matter competitively]

- **Founded:** [year]
- **HQ:** [location]
- **Funding/Market status:** [Privately held w/ $X in funding OR Publicly traded, TICKER, with $X revenue]
- **Core technologies:** [e.g., columnar storage, eBPF, proprietary agents]
- **Core solutions:** [e.g., APM, Infrastructure Monitoring, Log Management, SIEM]

---

### Competitor GTM Strategy

[1-2 paragraphs on how they go to market — sales motion, typical buyer persona, land-and-expand patterns]

#### Their Messaging and Positioning
[What do they lead with? Headline value prop? How do they frame themselves vs. the market?]

#### Strengths — What Customers Like About Them
[3-5 bullet points. Be honest — reps lose credibility if they dismiss competitors customers already like]

#### Sales Process
[Free tier → POC → enterprise? Top-down to CIO? Bottom-up with developers?]

#### Pricing
[Pricing model, known gotchas, hidden costs, consumption traps]

---

### What to Say — Elastic Positioning

These talking points emphasize Elastic's strengths against [Competitor]. Use them to enhance solution discussions, focusing only on customer needs identified during discovery and/or related to MEDDPICC.

#### Differentiators

1. **[Headline]** — [Complete sentence explaining the differentiator and why it matters to the customer]
2. **[Headline]** — [Complete sentence]
3. **[Headline]** — [Complete sentence]

---

### Depositioning

Expose vulnerabilities in [Competitor]'s offerings compared to Elastic. Use these points to assess relevance and diminish perceived value of their solutions.

1. **[Headline]** — [Complete sentence explaining the weakness and customer impact]
2. **[Headline]** — [Complete sentence]
3. **[Headline]** — [Complete sentence]

---

### Heatmap

High-level comparison based on solution attributes:

| Capability | Elastic | [Competitor] | Notes |
|---|---|---|---|
| [Capability] | ✅ Strong | ⚠️ Partial | [Brief context] |

Use: ✅ Strong, ⚠️ Partial/Limited, ❌ Weak/Missing

Cover capabilities relevant to overlap areas. For observability competitors: Log Management, APM, Infrastructure Monitoring, RUM, Synthetics, Universal Profiling, AIOps, OpenTelemetry support, Custom Dashboards, Alerting, SLOs.

---

### What to Do — Recommended Actions

1. [Concrete action specific to this competitor]
2. [Action]
3. [Action]

---

### Trap-Setting Questions

Questions designed to expose [Competitor]'s weaknesses during discovery or evaluation. Frame as genuine customer-concern questions, not transparent gotchas.

1. "[Question surfacing a known competitor limitation]"
2. "[Question]"
3. "[Question]"
4. "[Question]"
5. "[Question]"

---

### Objection Handling

Common objections specific to [Competitor] comparisons with recommended responses.

**"[Competitor] is cheaper/simpler/faster to deploy."**
[Response — validate the concern first, then pivot]

**"[Competitor] has better [specific capability]."**
[Response]

**"Why wouldn't we just use [Competitor] since we already have it?"**
[Response]

[Add 2-4 more objections relevant to this competitor]

---

### Resources and More Info

[Links to Elastic competitive landing pages, technical comparisons, case studies, analyst reports]

---

### Step 3: Writing Guidelines

Follow these principles throughout:

- **Be honest about competitor strengths.** Reps lose deals when they dismiss competitors customers already like. Acknowledge, then redirect.
- **Differentiators must be defensible.** Don't claim Elastic is better at something it demonstrably isn't.
- **Trap-setting questions should sound natural.** Questions a savvy buyer would genuinely want answered.
- **Objection handling should be empathetic.** Validate the concern, then pivot. Never dismiss.
- **Keep it scannable.** Reps reference this mid-call. Short sentences, bold headers, no walls of text.
- **MEDDPICC alignment.** Tie differentiators and depositioning to Metrics, Economic Buyer concerns, Decision Criteria, and Identified Pain.
