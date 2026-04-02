---
name: prompt-review
description: Analyze the user's most recent prompt for clarity, ambiguity, and effectiveness, then provide a rewrite
user_invocable: true
---

Look at the user's most recent prompt before this skill was invoked (not the skill invocation itself). Analyze it and respond with exactly this structure:

## Score: X/10

Rate the prompt's overall quality.

## Verdict

One sentence: was this prompt clear enough to get what the user actually wanted?

## Problems found

Bullet list. For each issue, name the problem and quote the specific words that caused it. Check for:

- Ambiguity — Could this be interpreted multiple ways? Which words are doing the damage?
- Missing context — What did the user assume Claude already knows but didn't state?
- Buried intent — Is the real ask hidden behind filler? Where does the actual request start?
- No success criteria — How would Claude know if it got the right answer?
- Scope creep — Is this secretly 2+ requests in one? Should it be split?
- Vague references — "this", "that", "it" — what do they actually point to?

If the prompt was actually good, say so and explain what made it work.

## Rewrite

Provide a rewritten version that:
1. Leads with the action (what Claude should do)
2. States the goal (why)
3. Defines the output format (what success looks like)
4. Removes filler words and redundancy
5. Is at least 30% shorter OR more precise (or both)

## Pattern to remember

One transferable lesson for future prompts. Frame it as: "When you want X, start with Y."
