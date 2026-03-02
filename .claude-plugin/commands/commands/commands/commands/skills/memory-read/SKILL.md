---
name: memory-read
description: Automatically check MEMORY.md for relevant past experiences before giving advice or making recommendations. Use this skill whenever the user is asking for help with a decision, debugging a problem, choosing between options, planning a strategy, or any situation where past experience would be valuable. Always check for MEMORY.md in the project root before responding to these types of requests.
---

# Memory Read Skill

Before responding to any request that involves a decision, recommendation, strategy, debugging, or problem-solving:

1. Check if MEMORY.md exists in the project root.
2. If it exists, scan the entries for anything relevant to the current request.
3. Match by tags, similar situations, and applicable lessons.
4. If relevant memories exist, factor them into your response naturally.

## How to reference memories in your response

Do NOT say "According to MEMORY.md" or "Based on your memory file." That sounds robotic.

Instead, weave it in naturally:
- "Last time we tried a narrow range on a volatile pair it didn't go well — we lost about 12% to IL in 48 hours. Might want to consider a wider range this time."
- "We've hit rate limit issues with CoinGecko before during peak hours. Worth setting up a fallback data source from the start."
- "Based on how the GraphQL migration went — it took 3x longer than estimated — I'd pad the timeline on this one."

## When NOT to reference memories

- If no relevant memories exist, don't force it.
- If the current context is clearly different from past situations, acknowledge that.
- Never let past memories override clear current evidence. Memories inform, they don't dictate.

## Suggesting new memories

If during the conversation a meaningful decision is made and MEMORY.md exists, offer to create a new entry:
"This feels like a decision worth remembering. Want me to add it to MEMORY.md?"

Don't create entries without asking. The human owns the memory.
