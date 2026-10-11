# Worked example: consumer app

**Prompt:** *"What job is a meal-planning app actually solving? We keep adding recipe features and growth is flat."*

## Mode 1 - Discover

**Customers:** core job executor: the household cook planning the week. Purchase decision maker: usually the same person. Their needs stay separate anyway: as executor they measure time and stress, as buyer they measure subscription cost against takeout spend.

**Core functional job:**

> *Feed the household satisfying meals across the week, within a budget*

Rule check: "browse recipes" may define too narrow a job if customers are trying to plan, shop, cook, and use leftovers. That is a hypothesis about the scope of their needs, not an explanation of flat growth. Check alternatives such as acquisition, pricing, onboarding, and retention before diagnosing the business. Also: "weeknight chaos" is a situation, not a job. The job is what the cook decides to do in it.

## Mode 2 - Break down

**Job map with sample outcomes** (partial set):

| Step | Desired outcome |
|---|---|
| Define | Minimize the time it takes to decide what to cook for the week, e.g., Sunday planning |
| Locate | Minimize the likelihood of missing an ingredient mid-recipe on a weeknight |
| Prepare | Minimize the time it takes to turn the week's plan into one shopping list |
| Confirm | Minimize the likelihood that a planned meal conflicts with a household member's restriction |
| Execute | Minimize the time it takes to get a weeknight dinner on the table |
| Monitor | Minimize the likelihood that bought ingredients expire unused |
| Modify | Minimize the time it takes to replace a planned meal when the evening changes |
| Conclude | Minimize the likelihood that leftovers go to waste |

**Other need types:** related jobs: manage the grocery budget, accommodate diets. Emotional: *feel like a good parent/partner*, *avoid the nightly "what's for dinner" dread*. Social: *be seen as someone who has it together*. Consumption-chain: set up household preferences in under 10 minutes. Financial (buyer hat): *reduce weekly spend on unplanned takeout*.

## Mode 3 - Plan

**Scores (estimates: founder judgment plus app-store review mining; riskiest assumption: importance of "recipe variety" may be inflated by vocal reviewers):**

| Outcome | Imp | Sat | Opp |
|---|---|---|---|
| Replace a meal when the evening changes | 8.6 | 2.9 | **14.3** |
| Ingredients don't expire unused | 8.2 | 3.4 | **13.0** |
| One shopping list from the plan | 7.9 | 4.5 | **11.3** |
| Find new recipes | 6.0 | 8.8 | 6.0 |

**Reading:** these estimates suggest recipe discovery may be overserved and unmet outcomes may cluster around mid-week adaptation and waste. They do not establish market prevalence or show why growth is flat. Validate both the outcome ratings and the competing explanations before committing the roadmap.

**Strategy candidate:** test adaptive replanning and waste tracking at the current subscription price. A dominant strategy requires evidence of both better job performance and lower cost; the same subscription price alone does not establish lower customer cost. Treat the book's switching-improvement guidance as a framework claim, not a universal customer threshold.

**Actions:**

1. Prototype "swap tonight's meal" one-tap replanning (outcome #1); compare its value with the planned recipe release before reprioritizing either
2. Test expiry-aware planning from existing fridge ingredients (outcome #2); measure actual use and waste before claiming an improvement
3. Test outcome-led positioning against the current recipe-led message; avoid "never" promises until the product can support them
4. Observe household-preference setup and test a shorter flow; treat under 10 minutes as a proposed target, not a measured customer requirement
