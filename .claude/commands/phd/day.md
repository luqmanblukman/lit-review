---
description: Open or close a research day (plan check / ratings log + commit)
argument-hint: open | close
---
Adopt the `phd-supervisor` persona (`.claude/agents/phd-supervisor.md`). Run this in the main conversation.

Work out Day N from the start date in `PROTOCOL.md`. Today's log is `~/repos/phd-journal/daily/<YYYY-MM-DD>.md`.

## `open` (hat: supervisor)
1. Note any missed days since the last log. Create a log stub for each one with `missed: true` and no ratings.
2. State Day N, the current block from the PROTOCOL calendar, and the days left until the next deadline.
3. Ask: **"What's the plan for today's 1.5 h, and what does done look like?"** Don't suggest a plan.
4. If the plan is vague or drifts from the block's goal, ask one sharp question about it. Then accept whatever they decide.
5. Create today's log with frontmatter (`day`, `date`, `missed: false`) and a `## Plan` section holding their words verbatim.

## `close` (hat: experimenter)
1. Ask, in one message:
   - deep work minutes
   - `interest`, `energy` and `frustration` (each 1–5)
   - `progress_felt` (1–5)
   - what actually happened, compared with the plan
   - one line: "Do I want to do this again tomorrow?"
2. Write the ratings into today's frontmatter and add `## What happened` and `## Tomorrow?` sections with their words verbatim.
3. Commit the journal: `log: day N`.
4. If lit-review has changes, show `git status --short`, propose a semantic message (`docs(day N): ...`) that reveals no journal content, and commit.

End with:
---
**Next step:** `/phd:day open` tomorrow. If today is the last day of a week, run `/phd:week`; on Day 14 or 30, run `/phd:sprint-review`.
