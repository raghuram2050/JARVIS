# /today — Daily To-Do Lookup

> Scope: the `daily/` folder in this workspace (Base).

Report on today's activities using the `daily/` folder in this project.

## Steps

1. Determine today's date and look for `daily/<YYYY-MM-DD>.md`.
2. If it doesn't exist yet:
   - Find the most recent existing file in `daily/` before today (filenames sort chronologically, so this is a plain filename sort — no date parsing needed).
   - Create today's file using the template below.
   - Carry forward any unfinished items from that prior file's `## To do` section into today's `## To do` section. Skip anything already checked off or moved to `## Done`. Don't duplicate an item that's already present in today's file.
3. Read today's file and give the user a concise summary:
   - Open to-dos first
   - Then any notes worth surfacing
   - Summarize — don't dump the raw file contents
4. If the user adds, removes, or checks off items during the conversation, write those changes back to today's file so it stays current.

## Daily file template

```
# YYYY-MM-DD

## To do
-

## Notes
-

## Done
-
```

## Notes

- Never invent to-dos — only report what's actually written in the files.
- If `daily/` has no prior files at all (first-ever run), just create today's file empty from the template and say so — there's nothing to carry forward.
