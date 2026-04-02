---
name: session-review
description: Review the entire conversation for prompt quality patterns, scoring communication and identifying recurring habits
user_invocable: true
---

Review the entire conversation from start to this invocation. Analyze the user's prompts, questions, decisions, and interactions as a whole. Respond with exactly this structure:

## Score: X/10

Rate the overall quality of the user's communication throughout this session.

## What worked

Bullet list: 2-3 specific things the user did well. Quote the prompt or action that demonstrates each.

## What didn't

Bullet list: 2-3 specific moments where a better prompt, decision, or sequence would have saved time or gotten a better result. Quote the prompt and explain what to do differently.

## Recurring pattern

If you have access to previous session review logs, check if any feedback from this session matches previous reviews. If a pattern repeats, call it out clearly: "This is the Nth time this has come up: [pattern]." If no prior reviews exist, write "No recurring patterns yet."

## Top takeaway

One sentence — the single highest-impact habit to practice in the next session.
