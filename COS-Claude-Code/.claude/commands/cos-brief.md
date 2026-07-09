---
description: "Decision brief: gather all context on a topic from email, Slack, and calendar"
---

Read config.yaml from the project root.

The user needs a decision brief on a topic. $ARGUMENTS describes the topic.

Steps:
1. Search Gmail for relevant threads: search by topic keywords, last 30 days.
2. Read the top 3-5 most relevant threads in full.
3. Search Slack for the topic keywords in priority channels.
4. Check calendar for related meetings.
5. Compile a brief:

```
**Decision Brief: [topic]**

**Background:** [2-3 lines of context from email/Slack]

**Key stakeholders:** [who's involved and their positions]

**Current state:** [what's been decided, what's open]

**Options:**
1. [Option with pros/cons]
2. [Option with pros/cons]

**Recommendation:** [based on the evidence gathered]

**Sources:** [list of email threads and Slack threads referenced]
```

Keep it to one screen. Bold the recommendation.

$ARGUMENTS
