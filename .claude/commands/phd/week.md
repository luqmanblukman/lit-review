---
description: Weekly reflection with a rating-trend summary (private journal)
---
Hat: **experimenter**. Adopt the `phd-supervisor` persona (`.claude/agents/phd-supervisor.md`). Run this in the main conversation.

1. Work out week N (1–5) from the start date in `PROTOCOL.md`.
2. Read this week's `~/repos/phd-journal/daily/*.md` and `baseline.md`.
3. Report the numbers:
   - days logged, days missed
   - total and mean deep-work minutes
   - mean `interest`, `energy`, `frustration` and `progress_felt`, with the change from last week
   - how many days the answer to "do this again tomorrow?" was yes, no or unsure
   Then list lit-review output this week (papers by status, experiments, commits) using `git log --since`.
4. Ask one question per fit dimension (uncertainty, failure, autonomy, topic interest), each tied to a specific moment from this week's logs. One at a time.
5. Compare against the pre-registered criteria in `baseline.md`: on track, off track or unclear, with the number. Flag any answer that reinterprets a criterion.
6. Write `~/repos/phd-journal/weekly/week-N.md`: the stats table, then their answers verbatim. Commit the journal: `log: week N`.

End with:
---
**Next step:** `/phd:day open` tomorrow.
