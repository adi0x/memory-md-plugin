Initialize MEMORY.md in the current project.

Create a MEMORY.md file in the project root with the proper frontmatter and structure. Before creating, check if one already exists.

Steps:
1. Check if MEMORY.md already exists in the project root. If it does, tell the user and ask if they want to reset it.
2. Ask the user for:
   - Project domain (defi, engineering, product, general, or custom)
   - Their name or identifier for the owner field
3. Create MEMORY.md with this exact format:

---
type: memory
version: 0.1.0
scope: project
domain: {domain they chose}
owner: {their name}
created: {today's date YYYY-MM-DD}
last_updated: {today's date YYYY-MM-DD}
entry_count: 0
---

# Project Memory

_This file captures decisions, outcomes, and lessons learned.
Agents read this file to learn from past experience._

<!-- New entries are added below. Most recent first. -->

4. Confirm to the user that MEMORY.md has been created and explain:
   - Memories will be written here automatically after meaningful decisions
   - They can update outcomes anytime by telling you what happened
   - The file works with any agent that can read markdown
