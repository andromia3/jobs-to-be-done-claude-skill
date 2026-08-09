# Worked example: B2B API product

**Prompt:** *"JTBD this: we're launching a web scraping API for AI teams. Help me plan the launch around customer needs."*

## Mode 1 - Discover

**Customers (three types, kept separate):**

- Core job executor: the ML/data engineer who pulls web data into pipelines
- Product lifecycle support: the platform engineer who manages keys, quotas, monitoring
- Purchase decision maker: the engineering manager, deciding on cost per successful record, not requests

**Core functional job** (verb + object + contextual clarifier):

> *Acquire structured web data for model training and agent workflows, on a recurring schedule*

Rule check: solution-free (no "API" in the job; Keurig test passed: the job isn't "call a scraping endpoint," it's acquiring usable data); functional only; customer's perspective; a job, not the situation "sites keep blocking us."

## Mode 2 - Break down

**Job map** (steps that apply) with sample desired outcomes. This is a partial set; real markets carry 50 to 150:

| Step | Desired outcomes (Ulwick syntax) |
|---|---|
| Define | Minimize the time it takes to determine which sources contain the needed data fields |
| Locate | Minimize the likelihood that a target source blocks access during collection |
| Prepare | Minimize the time it takes to define the output schema before the first run |
| Confirm | Minimize the likelihood that a sample extract fails validation, e.g., missing fields, wrong types |
| Execute | Minimize the likelihood that records arrive malformed when source page layouts change |
| Monitor | Minimize the time it takes to detect that a recurring collection has silently degraded |
| Modify | Minimize the time it takes to adapt the extraction when a source redesigns its pages |
| Conclude | Minimize the time it takes to confirm a delivered dataset is complete against the request |

**Other need types:** related jobs: clean the collected data, monitor competitor changes. Emotional job: *feel confident the pipeline won't break overnight*. Social job: *be seen as the engineer whose data can be trusted*. Consumption-chain: learn the API from docs in one sitting, rotate credentials without downtime. Buyer's financial outcomes: *reduce the cost per successful record*, *reduce spend on failed requests*.

## Mode 3 - Plan

**Scores (estimates, from 6 customer interviews, not a survey; riskiest assumption: satisfaction ratings for "silent degradation" came from only 2 people):**

| Outcome | Imp | Sat | Opp |
|---|---|---|---|
| Records survive page-layout changes | 9.0 | 3.5 | **14.5** |
| Detect silent degradation fast | 8.4 | 3.8 | **13.0** |
| Adapt to redesigns fast | 8.0 | 4.2 | **11.8** |
| Fast schema definition | 6.5 | 7.0 | 6.5 |
| Raw request speed | 5.8 | 8.5 | 5.8 |

**Reading:** resilience and observability are underserved; speed is overserved. Competitors race on latency that nobody is starving for.

**Strategy: Differentiated.** Target underserved AI teams with self-healing extraction and degradation alerts at premium price. Dominant is the long-term play if unit costs allow about 20% cheaper too.

**Actions (each tied to an unmet outcome):**

1. Ship change-resilient extraction (outcome #1) before adding endpoints
2. Build degradation alerting into the default plan (outcome #2)
3. Value proposition in outcome language: "Data that survives site changes", not "fast scraping API"
4. SEO/content around the job phrases customers actually search: *detect scraper breakage*, *schema drift in web data*
5. Sales tool for the buyer: cost-per-successful-record calculator (financial outcome)
