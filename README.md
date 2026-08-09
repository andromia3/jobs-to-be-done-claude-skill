# Jobs-to-be-Done skill for Claude

**Plan any product around the customer's job, not your roadmap.** A Claude skill built strictly on Tony Ulwick's *Jobs to be Done: Theory to Practice*: job maps, desired outcome statements, opportunity scoring, and growth strategy, in the book's exact formats.

![License: MIT](https://img.shields.io/badge/license-MIT-green) ![Works with: Claude Code](https://img.shields.io/badge/works%20with-Claude%20Code-blue) ![Works with: Cowork / claude.ai](https://img.shields.io/badge/works%20with-Cowork%20%2F%20claude.ai-blue) ![Source: Ulwick 2016](https://img.shields.io/badge/source-Ulwick%2C%20JTBD%3A%20Theory%20to%20Practice-orange)

## 10-second demo

**You type:**

> JTBD this: we're adding AI-powered dashboards to our analytics product

**You get back** (truncated):

> The job isn't "view dashboards". That's your product talking. The core functional job: ***monitor business performance against targets, daily***. Job executor: the ops lead, not the analyst who buys it.
>
> | Desired outcome (Ulwick syntax) | Imp | Sat | Opp |
> |---|---|---|---|
> | Minimize the time it takes to determine *why* a metric moved | 8.8 | 3.1 | **14.5** |
> | Minimize the likelihood that an anomaly goes unnoticed overnight | 8.5 | 4.0 | **13.0** |
> | Minimize the time it takes to build a new dashboard | 6.2 | 7.8 | 6.2 |
>
> *(Scores are estimates. Survey before betting the roadmap.)*
>
> Verdict: dashboard-building is **overserved** (sat > imp). The underserved outcomes are diagnosis and alerting. Strategy: **Differentiated**. Target underserved ops leads with root-cause explanation, priced premium. Building more dashboard features targets an outcome nobody is starving for.

That's the skill catching an ideas-first bet before it ships.

## Install

**Claude Code** (personal, all projects):

```bash
git clone https://github.com/anilkk/jobs-to-be-done-claude-skill.git
cp -r jobs-to-be-done-claude-skill/jobs-to-be-done ~/.claude/skills/
```

For one project only: copy the folder to `<repo>/.claude/skills/` instead.

**Cowork / claude.ai:** open [`jobs-to-be-done/SKILL.md`](jobs-to-be-done/SKILL.md), copy the content (below the frontmatter), and ask Claude: *"Save this as a skill named jobs-to-be-done."*

## Usage

```
JTBD this feature: [your feature idea]        → Discover mode
Build a job map for [job/product]             → Break down mode
Score these outcomes and pick a strategy      → Plan mode
```

Casual asks trigger it too: *"what job is this actually solving?"*, *"help me plan this around customer needs."*

## What's inside

| Mode | What it does |
|---|---|
| **Discover** | Defines the job executor (3 customer types) and the core functional job in `verb + object + contextual clarifier` format, checked against Ulwick's 5 definition rules |
| **Break down** | Walks the 8-step Universal Job Map, writes desired outcome statements in exact syntax, captures related / emotional / consumption-chain / financial needs |
| **Plan** | Scores outcomes with the Opportunity Algorithm (`importance + max(importance - satisfaction, 0)`), picks from the 5-strategy Growth Strategy Matrix, outputs prioritized actions |

Cheat sheet of every format: [REFERENCE.md](REFERENCE.md). Full worked examples: [examples/](examples/).

## Grounding, and what this skill refuses to do

Everything comes from Ulwick's *Jobs to be Done: Theory to Practice* (2016): the Jobs-to-be-Done Needs Framework, the Universal Job Map, desired outcome syntax, the Opportunity Algorithm, Outcome-Based Segmentation, and the Growth Strategy Matrix. Nothing is generic-blog JTBD.

Deliberate limits: it labels unsurveyed opportunity scores as **estimates** (the book demands surveys of 180 to 3,000 customers), it says so when a topic is outside the book, and it rejects malformed inputs: job statements with adjectives, "job stories" that cram emotion and outcomes into one line, persona-based segments.

## Credits and license

This skill is based on the book [*Jobs to be Done: Theory to Practice*](https://jobs-to-be-done-book.com/) by Tony Ulwick. The frameworks (Universal Job Map, desired outcome syntax, Opportunity Algorithm, Growth Strategy Matrix, Outcome-Driven Innovation) belong to Tony Ulwick and [Strategyn](https://strategyn.com). This repo references them with attribution and reproduces no book text. If this skill is useful, [buy the book](https://jobs-to-be-done-book.com/); it's short and the source of everything here.

Skill and repo text: [MIT License](LICENSE).

Contributions welcome: better worked examples and install-path fixes especially. Open a PR.
