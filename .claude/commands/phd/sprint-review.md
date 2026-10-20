---
description: "Day 14 / Day 30 sprint review — deck check, reviewer #2 critique, rebuttal"
argument-hint: 1 | 2
---
Hat: **supervisor (reviewer #2)**.

Sprint: $ARGUMENTS. The deck is `sprints/sprint-$ARGUMENTS/deck.md`.

1. If the deck doesn't exist, scaffold an empty Marp file (frontmatter `marp: true`, `theme: default`, `paginate: true`, plus one empty slide per section: Goal, What I tried, What failed, What I now believe, Next). Don't fill in any content. Stop and tell them to write it.
2. Check completeness: 5–10 slides, at least 2 visuals (figure, table or Mermaid), a failures slide, and no slide that's only bullet text. Report any gaps. Ask whether they presented it out loud and recorded it. If not, tell them to do that before the critique.
3. Delegate to the `phd-supervisor` subagent:
   > Critique `sprints/sprint-$ARGUMENTS/deck.md` as reviewer #2 at a sprint review. Read the cited papers, notes, `synthesis/` and any experiments it references. Don't read the journal. Judge: is there a coherent story? Do the visuals support the claims? Are the failures analysed or just listed? Is the research question sharper than two weeks ago? Numbered points, each tagged major or minor. Return the critique only.
4. Write `sprints/sprint-$ARGUMENTS/review.md` with `## Reviewer #2 (AI)` holding the critique verbatim, plus empty `## My rebuttal` and `## Human reviewer` sections.
5. For sprint 2: remind them to get at least one human to review the deck and record that feedback.
6. Commit: `docs(day N): sprint $ARGUMENTS review`.

End with:
---
**Next step:** Write your rebuttal in `review.md`. Sprint 1: then start the hypothesis block with `/phd:experiment <slug>`. Sprint 2: run `/phd:verdict`.
