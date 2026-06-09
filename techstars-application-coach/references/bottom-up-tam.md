# Bottom-Up TAM — the proper method (+ optional web research)

Founders struggle with this question more than any other. They reach for a top-down number ("the market is $50B, we'll get 1%") because it's easy. Reviewers distrust it instantly. A **bottom-up** TAM, built from real buyers and a real price, is what earns credibility. This file is the method. Read it whenever the founder is on Question 5 (money / market size).

> **The pasted answer is only ~400 characters.** Everything below is the founder's working analysis. Once the math is solid, compress the answer to: revenue model in one line + the bottom-up TAM headline (buyers × price = $X) + the SOM. The full table stays in their deck/data room, not the form.

## The method, done properly

A bottom-up TAM is built from the ground up: count the real buyers, multiply by what each realistically pays per year.

**Step 1 — Define the buyer precisely.** Tie this to the Ideal Customer Profile from Question 6. The buyer is the specific person or organization that actually pays. "Restaurants" is loose; "full-service restaurants in the U.S." is countable. If the ICP isn't nailed yet, fix that first — a fuzzy buyer makes every number downstream fuzzy.

**Step 2 — Count the buyers from real data.** How many of that buyer actually exist? This must come from a credible source (government statistics, industry associations, census of businesses, market reports), not a round guess. This is the number founders most often invent — and the easiest to verify or refute. (This is where web research helps most — see below.)

**Step 3 — Set a realistic annual revenue per buyer (ACV).** Annual Contract Value = what one buyer pays you per year. Base it on actual pricing or a defensible planned price, not a hopeful one. If you bill monthly, annualize it (e.g., $100/mo → $1,200 ACV).

**Step 4 — Segment when buyers differ.** If buyers split into groups that pay very differently (e.g., enterprise vs. SMB, multi-location vs. single), don't blend them into one average. Compute each segment separately: buyers in segment × ACV for that segment. This is more honest and usually more persuasive.

**Step 5 — Multiply and sum.**
- Single segment: `TAM = ACV × number of real buyers`
- Multiple segments: `TAM = Σ (buyers in segment × ACV in segment)`

**Step 6 — Sanity-check.** Cross-check the result against any top-down figure you can find. If your bottom-up number is wildly larger than the known industry size, the buyer count or the price is wrong. Adjust until it's defensible.

### Worked example (from the guide)
Annual subscription = $1,200. U.S.: 749,404 restaurants → ~$749.4M. Europe: 1.5M restaurants → ~$1.8B. The strength here is that both the buyer count and the price are concrete and checkable — not "the food-tech market is huge."

## Common mistakes to flag

- **Top-down hand-waving:** "1% of a $50B market." Reviewers discount it entirely. Force the bottom-up build.
- **Counting everyone:** using the whole population instead of *real, reachable* buyers who have the problem and will pay.
- **Fantasy pricing:** an ACV the buyer would never actually agree to.
- **One blended ACV** when segments clearly pay different amounts.
- **No source** for the buyer count — the single most common fatal flaw.
- **A TAM that's too small.** A small TAM is a venture dealbreaker. If the honest number is small, widen the buyer definition (adjacent segments, geographies) rather than inflating the price.

## Optional: offer web research to ground the numbers

Because the buyer count and ACV are the two inputs founders most often guess, **proactively offer to research them** when you reach Question 5:

> "The two numbers that make or break this answer are *how many buyers actually exist* and *how much each would pay per year.* Want me to dig into both with a web search and build the TAM from cited figures? You can correct anything that looks off."

If the founder says yes, run **several targeted searches** (not one) and assemble the estimate:

1. **Buyer count** — search for the size of the buyer population: number of businesses/establishments in the category and geography, industry-association membership counts, government or census data. Run separate searches per geography or segment if the TAM spans more than one. Prefer original sources (gov, trade associations, reputable market reports) over aggregators.
2. **Revenue per buyer (ACV)** — search for pricing benchmarks of comparable products, typical contract or subscription values in the category, or what incumbents charge — to pressure-test the founder's planned price.
3. **Top-down cross-check** — search for the reported overall market size, to sanity-check the bottom-up total in Step 6.

Then present the bottom-up build with each input **attributed to its source**, show the arithmetic, and ask the founder to confirm or adjust before it goes in the answer. Make clear these are research-based estimates, not guarantees — the founder owns the final numbers. Never invent a figure to fill a gap; if research is thin, say so and use a clearly labeled range.

For a market that genuinely needs deep, multi-source research, the founder can also use Claude's Research feature for a more exhaustive pass — mention it if the question is broad.
