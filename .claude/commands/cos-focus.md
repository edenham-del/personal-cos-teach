---
description: "Find and book focus time blocks on your calendar"
---

Read config.yaml from the project root.

Steps:
1. Find free time for this week (or timeframe from $ARGUMENTS):
   - calendars: config.yaml calendars
   - minDuration: config.yaml focus_time.min_block_hours * 60
2. Filter to preferred times and days from config.
3. Present top options.
4. If the user picks one, create a calendar event titled "Focus Time" with
   no attendees.

$ARGUMENTS
