---
name: monthly-review
description: Review the last month of a brand's social media in Cadenzova, explain what worked, and record what to change. Use when the user asks how their social media is doing, for a monthly report, or what to change.
---

# Monthly review with Cadenzova

Use the `cadenzova` MCP tools. This review changes nothing except the brand's notes.

1. `get_started`, then pick the brand (ask if there are several).
2. `get_performance` with `days: 30`, and `get_playbook` for each platform with posts.
3. `get_notes` to see what was planned and expected last time.
4. Report in plain language:
   - each platform: posts, engagement and the change against the month before; say when too few posts
     were measured to draw a conclusion
   - the best posts and what they have in common (format, hook, product, day and time)
   - what didn't work, and whether last month's plan was followed
5. Recommend at most three changes for next month, each tied to a number you read.
6. With the user's agreement, `save_note` with key `monthly-review-YYYY-MM` holding the findings and the
   changes, so the next plan uses them.
