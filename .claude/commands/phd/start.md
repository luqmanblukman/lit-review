---
description: Day 0 baseline — pre-register fit criteria and fix the calendar
---
Hat: **experimenter**. Adopt the `phd-supervisor` persona (`.claude/agents/phd-supervisor.md`). Run this in the main conversation, because it's an interview.

Steps:
1. If `~/repos/phd-journal/baseline.md` already has a `locked_on` date, stop. The baseline is locked; show it and suggest `/phd:status`.
2. Interview the user **one question at a time**. Record their answers verbatim; don't paraphrase them into something tidier.
   - Why a PhD, and why now? What would they lose by not doing one?
   - What do they expect the hardest part to be?
   - Why applied AI × distributed systems specifically? Name one problem in it that bugs them.
   - For each fit dimension (uncertainty and ambiguity, handling failure, autonomy vs structure, topic interest): what concrete observation by Day 30 would mean **yes**, and what would mean **no**? Push until each criterion is observable, e.g. "average interest ≥ 3.5 in week 4", "skipped ≤ 3 days", "I voluntarily read beyond the 1.5 h on ≥ 5 days".
   - Their predicted verdict, and their confidence from 0 to 100%.
3. Write `~/repos/phd-journal/baseline.md` from the answers and set `locked_on: <today>` in its frontmatter.
4. Ask for the Day 1 date (default: tomorrow). In `PROTOCOL.md`, fill in the start date, the Day 14 date and the Day 30 date.
5. Commit the journal (`chore: lock baseline`) and lit-review (`docs: set experiment calendar`).

End with:
---
**Next step:** On Day 1, run `/phd:day open`.
