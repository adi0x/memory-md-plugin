Search MEMORY.md for relevant past experiences.

The user wants to know what past memories are relevant to their current situation or question.

Steps:
1. Read MEMORY.md completely.
2. Based on the user's current question or context, find memories that are relevant by matching:
   - Tags that relate to the current topic
   - Similar situations or decision types
   - Lessons that might apply to the current context
   - Patterns across multiple memories
3. Present the relevant memories concisely:

For each relevant memory, show:
```
[MEM-XXX] Title
Lesson: {the key takeaway}
Relevance: {one sentence on why this applies now}
```

4. If multiple memories point to the same lesson, call that out as a pattern:
```
Pattern detected across [MEM-XXX], [MEM-YYY], [MEM-ZZZ]:
{The recurring lesson}
```

5. If no relevant memories exist, say so honestly. Don't stretch irrelevant memories to fit.

6. Always end with a reminder: "These are past experiences, not rules. Context changes. Consider whether the current situation is similar enough for these lessons to apply."

This command can also be used without arguments. If the user just says /memory:recall, show a summary of all memories organized by domain/tags with their status (active, pending outcome, superseded).
