---
name: plan-my-week
description: Plan and write next week's social media posts for a brand in Cadenzova, check them, and leave them for the owner's approval. Use when the user asks to plan their week, fill their calendar, or "do my social media".
---

# Plan my week with Cadenzova

Use the `cadenzova` MCP tools. The owner approves every post unless their connection is on Autopilot.

1. `get_started`. If a brand has no channels or products, tell the user what to fix and stop.
   If several brands exist, ask which one.
2. Read before deciding, in one pass:
   - `get_brand_brief`, `list_products`, `list_channels` (which platforms are connected, their limits)
   - `get_notes` (decisions from earlier sessions; follow them unless results say otherwise)
   - `get_performance` (30 days) and `get_playbook` for each connected platform
   - `get_calendar` (do not double up on days already planned)
3. Decide and say so briefly: which platforms, how many posts each, which products, which days and
   times (`get_best_times`), and why, citing the numbers you read. If there is little history, say so.
4. Write each post in the brand's voice. Use the brand's own photos first (`search_media`); otherwise
   `render_pin_template` for Pinterest, or `generate_image` (costs credits; say so before using it).
5. `validate_post` every post. Fix every error and every "reads as AI-written" or "close to a recent
   post" warning, then validate again.
6. `create_posts` once with the whole week (each post has its `scheduled_at`). Never create the same
   week twice; never retry a held post as `now`.
7. Tell the user what is waiting for approval and where (`approve_url`), then `save_note` with key
   `weekly-plan` summarising what you chose and why, so next week starts from it.
