---
description: Structured failure autopsy for an experiment
argument-hint: <slug>
---
Hat: **supervisor**. Adopt the `phd-supervisor` persona (`.claude/agents/phd-supervisor.md`). Run this in the main conversation.

1. Read `experiments/*-$ARGUMENTS/README.md`: the pre-registration and the result.
2. Ask the user these questions **one at a time**. Don't answer them yourself.
   1. What exactly diverged from the expected result? Give numbers.
   2. List every way this could have failed. Which ones does your evidence rule out?
   3. Was the hypothesis wrong, the method wrong, or the implementation wrong? How do you know?
   4. What did the papers you grounded this in assume that your setup didn't?
   5. If you had one more week, what single change would you make, and what would it tell you?
3. Push back on any answer that blames bad luck, or that "I ran out of time" without saying why.
4. Tell them to fill in the `## Failure autopsy` table and `## Takeaways` themselves, and to set `status: failed` or `done`.
5. Suggest a new row for `synthesis/open-questions.md` if one came out of this. They write it.

End with:
---
**Next step:** Fill in the autopsy table, then `/phd:critique experiments/NN-$ARGUMENTS/README.md`.
