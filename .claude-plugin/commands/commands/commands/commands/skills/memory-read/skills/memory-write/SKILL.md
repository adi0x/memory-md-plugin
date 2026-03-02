---
name: memory-write
description: Write structured memory entries to MEMORY.md following the MEMORY.md spec. Use this skill when creating new memory entries, updating outcomes, or managing the memory file. Activates when the user asks to remember something, log a decision, update an outcome, or when you detect a meaningful decision worth capturing.
---

# Memory Write Skill

When creating or updating memory entries in MEMORY.md, follow these rules strictly.

## Entry Format

Every new entry must have:
- Sequential MEM ID (zero-padded to 3 digits)
- Date, Context, Tags, Confidence, Status in the header
- Five sections: Situation, Decision, Reasoning, Outcome, Lesson

## Writing Principles

1. **Situation:** 2-4 sentences max. What was happening, what constraints existed.
2. **Decision:** Always include what was chosen, what was considered, and what was ruled out.
3. **Reasoning:** The WHY matters more than the WHAT. Capture the thinking.
4. **Outcome:** Only fill this in when results are actually known. Mark as _Pending_ otherwise. Never guess or assume outcomes.
5. **Lesson:** Distilled takeaways. Actionable. Connected to related memories via [[MEM-XXX]] links.

## Confidence Levels

- **high:** Clear outcome, strong evidence, lesson is well-supported
- **medium:** Outcome known but lesson might not generalize, or limited evidence
- **low:** Early signal, uncertain if the lesson will hold, needs more data

## Status Values

- **active:** This memory and its lessons are current and applicable
- **superseded:** A newer memory has updated or corrected this lesson. Link to the newer one.
- **archived:** No longer relevant due to major context change (tech stack changed, project ended, etc.)

## Updating Existing Entries

When updating outcomes:
- Never modify Situation, Decision, or Reasoning sections
- Only add to Outcome and Lesson sections
- If a lesson contradicts a previous memory, use strikethrough on the old lesson and link to the new one
- Always update the frontmatter last_updated date and keep entry_count accurate

## Tags

Use lowercase, hyphenated tags. Be specific enough to be useful for retrieval:
- Good: #uniswap-v3, #impermanent-loss, #foundry-testing
- Bad: #crypto, #code, #stuff

## Placement

New entries go after the header comment, before existing entries (most recent first).
