Create a new memory entry in MEMORY.md.

Review the current conversation and extract the most significant decision, problem solved, or lesson learned. Then write a structured memory entry.

Steps:
1. Read the existing MEMORY.md to get the current entry count and determine the next MEM ID.
2. Analyze the current conversation for:
   - Was a meaningful decision made with real tradeoffs?
   - Was a hard problem solved after significant effort?
   - Did something unexpected happen?
   - Was there a clear lesson learned?
3. If nothing meaningful happened, tell the user honestly — not every conversation needs a memory.
4. If there is something worth remembering, create an entry with this format:

## [MEM-{next number, zero-padded to 3 digits}] {Short descriptive title}

**Date:** {today's date YYYY-MM-DD}
**Context:** {One line summary of what was happening}
**Tags:** #{relevant} #{tags} #{for retrieval}
**Confidence:** {high | medium | low}
**Status:** active

### Situation
{2-4 sentences. What was happening, what problem existed, what constraints were in play.}

### Decision
- **Chosen:** {What was picked}
- **Considered:** {What else was on the table}
- **Ruled out:** {What was rejected and why}

### Reasoning
{2-4 sentences. Why this path was chosen. What factors mattered most.}

### Outcome
_Pending — update when results are known._

### Lesson
_Pending — will be clear after outcome._

5. Prepend the new entry after the header comment in MEMORY.md (most recent first).
6. Update the frontmatter: increment entry_count, update last_updated.
7. Show the entry to the user and ask if anything needs adjusting.

Writing rules:
- Be honest about uncertainty. If it was a guess, say so.
- Capture reasoning, not just the conclusion.
- Include what was ruled out and why.
- Tag generously but accurately.
- Use [[MEM-XXX]] wikilinks to connect to related past memories.
- Never fabricate outcomes. If unknown, mark as pending.
- Keep the human's voice. If they said "this was a disaster" don't soften it.
