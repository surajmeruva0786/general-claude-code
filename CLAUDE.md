# general-claude-code — daily log repo

This repo is a running journal of conversations/decisions with Claude Code, one dated markdown file per day (`YYYY-MM-DD.md`).

## After every answered query

Before ending your turn, append an entry to today's dated file (`YYYY-MM-DD.md` in the repo root, using today's actual date — create the file if it doesn't exist yet). Match the existing format (see `2026-08-01.md`):

```markdown
# <Short Topic Title> (YYYY-MM-DD)

## Question
<concise restatement of what was asked>

## Answer
<concise summary of the answer/decision given>
```

If today's file already has entries, append a new `---`-separated section rather than overwriting prior ones.

Keep entries concise — a summary of the exchange, not a full transcript.

**Do not run `git add`/`git commit`/`git push` yourself for this logging step.** A `Stop` hook (see `.claude/settings.local.json`) automatically commits and pushes any changes once your turn ends. Only commit manually for substantive file/code changes unrelated to the daily log, per the global commit-granularity preference.
