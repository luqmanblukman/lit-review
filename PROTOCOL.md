# Protocol

A 30-day replication of the working conditions of PhD research. The aim isn't to produce a result. It's to find out whether I want to keep doing this kind of work.

## Status

| | |
|---|---|
| Start date (Day 1) | _set by `/phd:start`_ |
| Sprint 1 review (Day 14) | _TBD_ |
| Sprint 2 review (Day 30) | _TBD_ |
| Daily budget | 1.5 h of deep work, no email or social media |

## Rules

1. **Systems, not inspiration.** I work a fixed 1.5 h block every day, whether or not I feel like it.
2. **I set my own direction.** Nobody assigns me tasks. I state each day's plan before I start.
3. **No back-filling.** A missed day is logged as missed. Missed days are data.
4. **The AI is a supervisor, not an author.** Claude may explain a concept when I ask. It never writes notes, synthesis, research questions or decks.
5. **Pre-registration.** On Day 0, before I start, I write down the fit criteria and my predicted verdict (privately). The Day 30 verdict is judged against them.
6. **Failures are kept.** Every failed experiment gets an autopsy and stays in the repo.

## Calendar

| Days | Block | Focus | Output |
|---|---|---|---|
| 1–5 | Scoping | Broad reading in applied AI × distributed systems; narrow to one research question | `synthesis/research-question.md` v1 by Day 5 |
| 6–13 | Literature | 3–5 foundational papers read deeply (multiple passes) | Paper notes, `related-work.md` draft |
| 14 | **Sprint 1 review** | 5–10 slide deck, presented out loud and recorded | `sprints/sprint-1/` |
| 15–28 | Hypothesis | One micro-hypothesis, tested; failures autopsied | `experiments/NN-*/` |
| 29–30 | Synthesis | Visuals first, then a 2–3 page narrative | `synthesis/related-work.md`, `sprints/sprint-2/` |
| 30 | **Sprint 2 review + verdict** | Deck critiqued; private verdict written against Day 0 criteria | |

## Rituals

| When | Command | What happens |
|---|---|---|
| Day 0 | `/phd:start` | Baseline interview, pre-registered criteria, calendar fixed |
| Daily start | `/phd:day open` | I state the plan and the supervisor checks it against the sprint goal |
| Daily end | `/phd:day close` | 1–5 ratings for interest, energy and frustration logged; both repos committed |
| Per paper | `/phd:paper` | Metadata, BibTeX and an empty note; later runs quiz me on it |
| Week 1 | `/phd:rq` | Research question pressure-tested |
| Per experiment | `/phd:experiment`, `/phd:autopsy` | Hypothesis locked before running; failures dissected |
| Any time | `/phd:critique <file>` | Reviewer #2 |
| Days 14, 30 | `/phd:sprint-review` | Deck critiqued, I write a rebuttal |
| Weekly | `/phd:week` | Reflection and rating trend |
| Day 30 | `/phd:verdict` | Evidence vs baseline |

## External critique

Working alone can't reproduce the rejection and scrutiny of a real PhD. Two mitigations:
- The AI reviewer critiques every sprint deck as a hostile reviewer would.
- **At least one human** (ideally someone with a research background) reviews the Day 30 deck. Their feedback is recorded in `sprints/sprint-2/review.md`.

## Known limits of this replication

- 30 days can't reproduce the year-2 slump, funding pressure or a real supervisor relationship.
- I'm doing this alongside a full-time job, so the time budget is lower than a real PhD.
- Self-selection: I chose to run this, so I'm likely biased towards a "yes". Pre-registration is the guard against that.
