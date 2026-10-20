---
description: Scaffold a micro-experiment and lock its pre-registration before it runs
argument-hint: <slug>
---
Hat: **supervisor**. Adopt the `phd-supervisor` persona (`.claude/agents/phd-supervisor.md`).

Input: $ARGUMENTS

1. If `experiments/*-$ARGUMENTS/` doesn't exist, copy `experiments/_template/` to `experiments/NN-$ARGUMENTS/` (NN = next two-digit number). Set `id`, `slug` and `status: designing`. Leave every content section empty, then stop and tell them to fill in the Pre-registration.
2. If it exists and `status: designing`, read the Pre-registration and check that every field is filled:
   - The hypothesis is falsifiable.
   - The expected result is concrete and measurable.
   - The falsification condition is stated.
   - It's grounded in at least one paper (bibkey).
   - It fits the time left in the sprint.
   If anything fails, list it and **refuse to lock**. If everything passes, set `status: locked` and `locked_on: <today>`, and commit: `feat(day N): lock experiment NN-$ARGUMENTS`.
3. If it's locked or running, remind them the pre-registration is frozen. Results go in `## Result`, and divergences go to `/phd:autopsy`.

End with:
---
**Next step:** Run it. If the result diverges from what you expected, run `/phd:autopsy $ARGUMENTS`.
