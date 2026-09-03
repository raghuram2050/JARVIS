# Personal Workspace — Daily Activity, Brainstorming & Design Notes

This is Gunvi's personal space for day-to-day to-dos, brainstorming, and design notes — separate from client/work repos. It's distinct in purpose from the global Staples Jira/Confluence conventions in `~/.claude/CLAUDE.md`, though work-related thinking can live here too.

## How this space is organized

- `daily/` — one file per day (`YYYY-MM-DD.md`) for whatever's on my mind: to-dos, quick notes, things to follow up on. This is the starting point — jot things down here as they come up, no need to categorize first.
- Other topic folders (e.g. `brainstorm/`, `designs/`) get created on demand — one file per topic, the first time a topic actually needs its own space, not pre-scaffolded in advance. When a new one is created, add a line to the index below.
- `Personal/` — a leftover sample folder, not currently used by this structure.
- `.claude/skills/today/` — the `/today` skill: reads today's daily file (creating it if missing) and reports open to-dos, carrying forward anything unfinished from the most recent prior day.
- This folder is a git repo backed by a **private personal GitHub repo** (not a Staples repo). Three scheduled cloud routines (9:30am/2:30pm/5:00pm ET, named "JARVIS ... Check-in") read from that remote to power alerts, so content needs to actually be pushed to be visible to them. They always run on the lowest-tier model (currently `claude-haiku-4-5-20251001`) — when creating or updating a scheduled routine for this workspace, keep it on the lowest available model unless told otherwise.

## Index of topic folders

(update this list whenever a new topic folder is created)

- `daily/` — day-to-day to-dos and notes

## Working agreement — keeping context light

- Keep this file itself short and stable — an index and pointers, not a content dump. Actual content lives in `daily/` and topic folders; read those on demand rather than restating them here, so this file doesn't grow and doesn't cost context on every turn.
- Durable facts about me (preferences, how I like to work, ongoing goals/projects) belong in your memory system, not here — save them there as they come up and use them automatically across sessions. This file describes the *shape of the workspace*; memory is about *me*.
- When a brainstorm or design conversation produces something worth keeping, write it to the relevant topic file before the session ends, rather than relying on it surviving conversation compaction.
- Prefer many small dated/topic files over one large growing log — it keeps each read cheap and lets you pull in only what's relevant to the current question.

## GitHub backup — push policy

- This folder is a local git repo backed by a private personal GitHub remote (not a Staples repo).
- `daily/`, `Personal/`, and this `CLAUDE.md` file itself: commit and push automatically as soon as they're updated — pre-approved, no need to ask each time.
- Any other folder (e.g. `brainstorm/`, `designs/` — anything not in the pre-approved list above): once a task/edit there is done, ask me whether to push it before doing so. Don't assume. If I say yes regularly for a given folder, ask whether to add it to the pre-approved list.
- Never point this repo at a work/Staples remote.
