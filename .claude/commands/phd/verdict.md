---
description: Day 30 verdict judged against the pre-registered baseline
---
Hat: **experimenter**. Adopt the `phd-supervisor` persona (`.claude/agents/phd-supervisor.md`). Run this in the main conversation.

1. If it's before Day 30 or the sprint 2 review doesn't exist, warn them and ask whether to proceed anyway.
2. Read `~/repos/phd-journal/baseline.md`, every daily and weekly log, and lit-review's `git log`, papers, experiments and sprint reviews (including the human reviewer's feedback).
3. Present the evidence first, without interpretation:
   - 30-day trends for each rating (week-by-week means), deep-work total and missed days
   - output counts
   - the "again tomorrow?" tally
   - for each pre-registered criterion: the observed value against the threshold, marked **met**, **not met** or **inconclusive**
4. Only then ask them, one at a time:
   - Your Day 0 prediction was X at Y% confidence. What surprised you?
   - Which criteria would you now want to reinterpret, and is that insight or rationalisation?
   - Nature of the work: fit or no fit?
   - The topic: fit or no fit? Or a different topic?
   - What would you need to see in a further 30 days to be sure?
5. Give your own reading as the experimenter in 3–5 sentences, grounded in the numbers. Say plainly if it disagrees with theirs.
6. Write `~/repos/phd-journal/verdict.md`: evidence table, criteria table, their answers verbatim, your reading, final verdict in their words. Commit the journal: `log: verdict`.
7. Ask whether they want a short, public-safe retrospective added to lit-review's README. If so, they write it.

End with:
---
**Next step:** Decide. If it's a yes, the lit-review repo is your portfolio, so keep reading.
