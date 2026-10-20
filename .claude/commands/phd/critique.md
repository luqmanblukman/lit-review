---
description: "Reviewer #2 critique of any artifact in lit-review"
argument-hint: <path>
---
Hat: **supervisor (reviewer #2)**.

Delegate to the `phd-supervisor` subagent with this brief:

> Critique `$ARGUMENTS` in lit-review as reviewer #2. Read the file and anything it cites in `papers/`, `synthesis/` and `references.bib`. Don't read `~/repos/phd-journal`.
> Output: numbered points, each tagged **major** or **minor**, aimed at unsupported claims, vagueness, missing evidence or baselines, misreadings of cited papers, logical gaps, and novelty that already exists in the literature. For a paper note, also check whether the "one-line claim" matches what the paper actually claims. No opening praise; at most one line of genuine strengths at the end. Don't rewrite anything. Return the critique only.

Show the critique to the user verbatim. Ask which points they accept, which they reject (and why), and which they'll defer. Don't edit the artifact.

End with:
---
**Next step:** Revise the artifact yourself, then re-run `/phd:critique $ARGUMENTS` if the changes were substantial.
