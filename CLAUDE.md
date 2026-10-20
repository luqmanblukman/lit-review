# lit-review: instructions for Claude

This repo is a 30-day PhD-fit experiment and a public literature-review portfolio. Read [PROTOCOL.md](PROTOCOL.md) first.

## Two repos

| Repo | Path | Visibility | Contents |
|---|---|---|---|
| lit-review | this repo | public | papers, synthesis, experiments, sprint decks and critiques |
| phd-journal | `~/repos/phd-journal` | **private** | baseline, daily logs, weekly reflections, verdict |

Never copy journal content (ratings, self-doubt, criteria, verdict) into this repo. Never create journal files here.

## The AI boundary (hard rule)

The point of this experiment is to test whether *I* like this work, and the portfolio has to be my own. So Claude:
- **may** scaffold files with empty content sections, fetch paper metadata and BibTeX, explain a concept when asked, quiz me, critique harshly, and run git;
- **must not** write or rewrite paper notes, summaries, synthesis, research questions, experiment hypotheses, autopsy answers or deck content, even if asked casually. If I ask, remind me of this rule. I can override it explicitly, and the override gets noted in the day's journal log.

## Guide

Use the `phd-supervisor` persona defined in `.claude/agents/phd-supervisor.md`. All rituals go through `/phd:*` commands in `.claude/commands/phd/`.

## Conventions

- Paper notes: `papers/<year>-<firstauthor-lowercase>-<short-slug>.md`, copied from `papers/_template.md`.
- BibTeX keys: `<firstauthor><year><firstword>`, e.g. `moritz2018ray`.
- Experiments: `experiments/NN-<slug>/`, copied from `experiments/_template/`.
- Decks: Marp markdown at `sprints/sprint-N/deck.md`.
- Diagrams: Mermaid.
- Commits: semantic prefixes (`docs:`, `feat:`, `chore:`) with a `day N:` scope where relevant, e.g. `docs(day 7): deep-read ray`.
