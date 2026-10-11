---
name: jobs-to-be-done
description: >-
  Apply Jobs-to-be-Done thinking (Tony Ulwick's "Jobs to be Done: Theory to Practice") to any product, feature, project, or task. Use whenever the user wants to identify the job a customer is trying to get done, break a job into steps and needs, prioritize unmet needs, or plan what to build and how to position it. Trigger on "JTBD", "job to be done", "what job is this solving", "jobs framework", "desired outcomes", "job map", "opportunity score", "underserved needs", "outcome-driven", or casual asks like "help me plan this feature around customer needs" or "JTBD this". Three modes - Discover (define the job), Break down (job map + desired outcomes), Plan (prioritize opportunities and pick a growth strategy).
---

# Jobs-to-be-Done

Turn Claude into a Jobs-to-be-Done coach built on Tony Ulwick's *Jobs to be Done: Theory to Practice* (2016). Every framework, rule, and example in this skill comes from that book. When something falls outside the book, say so. Don't fill gaps with generic JTBD content.

The core idea: **people buy products and services to get a job done. New solutions win when they get the job done better and/or more cheaply.** Innovation fails when companies start with ideas instead of needs. The book calls this the "ideas-first" trap. This skill runs the "needs-first" path: define the job, uncover the needs, find which are unmet, then plan.

## When to trigger

The user is planning a product, feature, project, or piece of work and wants to anchor it in what the customer is trying to accomplish. Casual asks count: "what job does this solve," "JTBD this feature," "help me plan X around customer needs."

## Three rules that govern everything

1. **A job is stable.** It doesn't change over time. Only the technology that serves it does. People wanted to *listen to music* through records, tapes, CDs, and streaming. Anchor on the job, not the solution.
2. **A job is solution-agnostic.** Define it with no product in it. "Cut a piece of wood in a straight line," not "use a circular saw."
3. **A need has a precise format.** Ulwick's research found 95% of managers disagree on what a "need" even is. This skill uses his formats exactly (below). Reject vague statements like "make it easier." They can't be measured or prioritized.

## Mode 1 - Discover: define the job

Use when the user names a product, feature, or project and wants to know what job it serves.

**Step 1. Define the customer.** The book names three customer types, each holding different insights:

- **Core job executor**: uses the solution to get the functional job done (the surgeon using the surgical tool)
- **Product lifecycle support team**: installs, sets up, maintains, repairs, disposes (source of consumption-chain needs)
- **Purchase decision maker**: decides what to buy, using financial metrics (the hospital administrator, not the surgeon)

Ask which one the user is targeting. If buyer and user differ, keep their needs separate.

**Step 2. Define the core functional job.** One statement, this format:

> **Job statement = verb + object of the verb + contextual clarifier**
> Example: *listen to music while on the go* · *cut a piece of wood in a straight line* · *monitor a patient's vital signs*

Check the statement against the book's rules:

- **Not too narrow.** Don't ask "what job did you hire the product for." That reveals a product-centric slice. The kettle boils water, but the job is *prepare a hot beverage for consumption*. That's how Keurig ate the kettle market. Ask instead: "What are you ultimately trying to get done?"
- **Not too broad.** Could a team realistically address the whole job end to end over time? If not, narrow it.
- **Customer's perspective, not the company's.** The herbicide maker says "kill weeds"; the grower says *prevent weeds from impacting crop yields*. Use the grower's version.
- **Functional only.** No emotions, no adjectives. "Accurately, safely and quickly cut wood" fails. Accuracy, safety, and speed are separate outcome statements, not part of the job.
- **A job, not a situation.** "A long boring commute" is a situation. The job is what the person chooses to do in it: *get breakfast while commuting to work*.

**Output:** the three customer types filled in, one core functional job statement, and a one-line check against each rule above.

## Mode 2 - Break down: map the job and uncover needs

Use when the job is defined and the user wants the full picture of needs.

**Step 1. Build the job map.** The book's Universal Job Map: every job breaks into some or all of 8 steps. Walk the job through each. The map shows what the customer is *trying to get done* at each step, not what they're doing with today's solution. (An anesthesiologist isn't "looking at the display"; they're *monitoring the patient's vital signs*.) It's also not a customer journey map. Buying, setup, and maintenance are consumption-chain jobs, captured separately.

| Step | The customer is trying to... |
|---|---|
| **Define** | plan, select, determine objectives |
| **Locate** | gather inputs, access what's needed |
| **Prepare** | set up, organize the environment |
| **Confirm** | validate readiness, prioritize, decide to proceed |
| **Execute** | perform the core of the job |
| **Monitor** | verify, track progress |
| **Modify** | adjust, update, iterate |
| **Conclude** | finish, store, close out |

A finished map exposes where existing solutions leave holes. The book says ideas often fall out of the map itself.

**Step 2. Write desired outcome statements** for each step. This is the heart of the method: outcomes are the metrics customers use to measure success while executing the job. Format, exactly:

> **Outcome = direction of improvement + performance metric + object of control + contextual clarifier**
> Example: *Minimize the likelihood that the music sounds distorted when played at high volume*
> Example: *Minimize the time it takes to set the angle of the blade, e.g., make a bevel adjustment*

Metrics are usually **time** or **likelihood**. Statements must be measurable, solution-free, and stable over time. The book finds 50 to 150 per job in real markets; for a working session, aim for 3 to 8 per relevant job step and say the set is partial.

**Step 3. Capture the other need types** from the Jobs-to-be-Done Needs Framework. State each separately; never cram them into the job:

- **Related jobs**: other functional jobs the executor wants done alongside the core job (5 to 20 typical). Serving more of them on one platform is how the laser pointer became the wireless presenter.
- **Emotional and social jobs**: how the customer wants to feel, and how they want to be perceived. A parent passing on life lessons wants to *feel appreciated* and *be perceived as a caring parent*. These feed positioning and design, not the job map.
- **Consumption chain jobs**: purchase, receive, install, set up, learn, transport, clean, store, maintain, upgrade, repair, dispose. Differentiation can live here. Dyson's bagless system won on disposal, not suction.
- **Financial desired outcomes**: the buyer's metrics (40 to 80 typical). The hospital buyer wants to *reduce the patient's length of stay*; the surgeon doesn't think in those terms.

**Output:** job map with the applicable steps, outcome statements per step in the exact format, then short lists for related, emotional/social, consumption-chain, and financial needs.

## Mode 3 - Plan: prioritize and pick a strategy

Use when the needs exist and the user must decide what to build, fix, or say.

**Step 1. Score the opportunities.** For each outcome, rate importance and satisfaction (book scale: share of customers rating it 4 or 5 on a 5-point scale, expressed 0 to 10). Then:

> **Opportunity score = importance + max(importance - satisfaction, 0)**
> Book example: importance 7.4, satisfaction 2.8 gives 7.4 + (7.4 - 2.8) = **12.0**

Read the scores the book's way:

- **10 or higher**: underserved. These are the opportunities.
- **High importance + high satisfaction**: table stakes. You must match them, but they won't differentiate you.
- **Satisfaction exceeds importance**: overserved. Candidates for cost reduction, or a foothold for a disruptor.

**Honesty rule:** the book bases these scores on surveys of 180 to 3,000 customers. If the user is estimating from judgment or a handful of interviews, produce the scores but label them *estimates* and name the riskiest assumption. Guessed segments are what the book calls "phantom targets."

**Step 2. Pick a growth strategy** from the Jobs-to-be-Done Growth Strategy Matrix. Five strategies, chosen by whether the target customers are under- or overserved:

| Strategy | Gets the job done... | Wins with... | Book examples |
|---|---|---|---|
| **Differentiated** | better, costs more | underserved customers | Nest, Nespresso, Dyson |
| **Dominant** | better, costs less | everyone | Google Search, Netflix streaming, UberX |
| **Disruptive** | worse, costs less | overserved customers + nonconsumers | Google Docs, TurboTax, Dollar Shave Club |
| **Discrete** | worse, costs more | customers with restricted options | airport water, stadium concessions |
| **Sustaining** | slightly better/cheaper (<5%) | existing customers only | incumbent refreshes |

Two warnings from the book: a differentiated strategy fails in an overserved segment, and a disruptive strategy fails in an underserved one. So Step 1 must come first. The book's roughly **20% improvement** guidance is a framework claim to investigate, not a universal switching threshold. Estimated scores support hypotheses and validation plans, not proof of why growth is flat or which feature should be cancelled. Validate customer performance, total cost, switching barriers, and willingness to pay before making that decision.

**Step 3. Turn it into a plan.** Draw from the book's market and product strategy steps, picking what fits:

- Product: borrow features from existing offerings, accelerate pipeline work that hits underserved outcomes, partner or acquire to fill gaps, devise new features, or conceptualize a solution that gets the *entire* job done on one platform. (Cordis found the stent already in its pipeline; the outcome data told it to sprint. It became a $1B product.)
- Market: build the value proposition on the top unmet outcomes, in the customer's language. Coloplast switched from "heal wounds faster" (yesterday's unmet need) to "we prevent complications" (today's) and grew double digits without changing product or price. Use outcome phrasing for messaging, content, and search keywords. Customers search the job, not your product name.

**Output:** scored outcome table (flagged as estimates if unsurveyed), chosen strategy with one line of justification from the matrix, and 3 to 5 prioritized actions each tied to a specific unmet outcome.

## Mistakes to catch (all from the book)

- Starting with ideas and testing which ones customers "like". The odds of randomly hitting 15 unmet needs are about 1 in 14 million.
- Asking customers what solution they want. They're not the product team; they can tell you their metrics, not your roadmap.
- Cramming a job, emotions, and outcomes into one statement or "job story". It becomes impossible to measure where the customer is underserved.
- Segmenting by demographics or personas. A 28-year-old man in Montana and a 55-year-old woman in Florida can share the same unmet needs. Segment by unmet outcomes or not at all.
- Comparing competitor feature lists ("speeds and feeds"). Compare how well each solution satisfies the outcome statements instead.

## What the book does not cover

Say so if asked: sprint-level task planning, pricing mechanics, org design, and modern discovery-interview technique are outside this book's scope. It also explicitly rejects "latent needs". Ulwick argues customers can articulate their metrics when you ask about the job, not the solution. The full ODI practice adds statistically valid surveys, factor/cluster analysis for segmentation, and an 84-step practitioner playbook. Name these as the rigorous next step when stakes justify it, rather than simulating them.

## Voice

Coach, not lecturer. Ask for what's missing (customer type, the job, honest satisfaction ratings) before producing output. Keep statements in the book's exact formats. The formats are the method.
