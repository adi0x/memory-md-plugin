Update an existing memory entry with outcome and lesson information.

The user is telling you what happened after a previous decision. Find the relevant memory and update it.

Steps:
1. Read MEMORY.md and list all entries that have "Pending" in their Outcome section.
2. Based on what the user is telling you, identify which memory entry they're referring to. If unclear, show them the pending entries and ask which one.
3. Ask the user (if not already clear from their message):
   - What happened? (the factual outcome)
   - Was it positive, negative, or mixed?
   - How long until the outcome was clear?
4. Update the memory entry:

For the Outcome section:
```markdown
### Outcome
- **Result:** {Positive | Negative | Mixed}
- **What happened:** {Factual description of what occurred}
- **Timeline:** {How long until the outcome was clear}
```

For the Lesson section:
```markdown
### Lesson
- {Key takeaway 1}
- {Key takeaway 2 if applicable}
- {Connect to related memories with [[MEM-XXX]] links if relevant}
```

5. Update the frontmatter last_updated date.
6. If the lesson contradicts a previous memory's lesson, note the conflict using strikethrough in the older memory and link to the new one:
```markdown
- ~~Previous lesson text~~ (superseded by [[MEM-XXX]])
- Updated lesson text
- Updated: {date}
```

7. If the lesson seems broadly applicable beyond this project, suggest promoting it to the user's personal memory.
8. Show the updated entry to the user for confirmation.

Important: Never change the original Situation, Decision, or Reasoning sections. Those capture what was known at the time. Only update Outcome and Lesson.
