# Worked example: consumer app

**Prompt:** *"What job is a meal-planning app actually solving? We keep adding recipe features and growth is flat."*

## Mode 1 - Discover

**Customers:** core job executor: the household cook planning the week. Purchase decision maker: usually the same person. Their needs stay separate anyway: as executor they measure time and stress, as buyer they measure subscription cost against takeout spend.

**Core functional job:**

> *Feed the household satisfying meals across the week, within a budget*

Rule check, and this is where the flat growth gets explained: "browse recipes" fails the narrowness test the way "boil water" did for the kettle. Recipes are one step of the job, and a competitor who serves the *whole* job (plan, shop, cook, use leftovers) takes the market. Also: "weeknight chaos" is a situation, not a job. The job is what the cook decides to do in it.

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

**Reading:** recipe discovery is heavily overserved, which is why shipping more recipe features moved nothing. The unmet outcomes cluster around mid-week adaptation and waste.

**Strategy: Dominant candidate.** Get the job done better (adaptive replanning, waste tracking) at the same subscription price and you undercut recipe-first incumbents on the outcomes that matter. Remember the switching bar: about 20% better on unmet outcomes, or nobody moves.

**Actions:**

1. Build "swap tonight's meal" one-tap replanning (outcome #1); kill the next recipe-pack release
2. Expiry-aware planning: suggest meals from what's already in the fridge (outcome #2)
3. Reposition from "10,000 recipes" to outcome language: "Never wonder what's for dinner, even when plans change"
4. Onboarding rebuilt around the consumption-chain outcome: preferences set in under 10 minutes
