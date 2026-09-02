---
name: today
description: >
  Daily to-do lookup for this personal workspace (daily/ notes folder).
  Reads today's dated file, creating it from the previous day's unfinished
  items if it doesn't exist yet, and reports open to-dos and notes. Invoke
  with /today at the start of a session, or anytime, to see what's
  outstanding for today.
---

Follow the detailed instructions in `prompt.md` in this skill's directory.

The `prompt.md` file defines the full today framework including:
- How to locate today's file and the most recent prior file in `daily/`
- The carry-forward rule for unfinished to-dos
- The template used when creating a new daily file
- How to summarize the file for the user instead of dumping it raw
- How to write updates back to the file during the conversation

## When to invoke

- "what are my to-dos for today?"
- "/today"
- Start of a work session, to see what's outstanding
- Anytime something gets added or checked off and should be saved
