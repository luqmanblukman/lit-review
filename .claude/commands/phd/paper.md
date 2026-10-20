---
description: Add a paper (metadata, BibTeX, empty note) or log another reading pass with a quiz
argument-hint: <url | arXiv id | DOI | title>
---
Hat: **supervisor**. Adopt the `phd-supervisor` persona (`.claude/agents/phd-supervisor.md`).

Input: $ARGUMENTS

## New paper
1. Resolve the metadata (title, authors, year, venue, canonical URL) with WebFetch or WebSearch. Prefer arXiv, DBLP or the ACM/USENIX page. If the paper is ambiguous, show the candidates and ask which one.
2. Append a BibTeX entry to `references.bib` with key `<firstauthor><year><firstword>`. Skip if the key already exists.
3. Copy `papers/_template.md` to `papers/<year>-<firstauthor>-<slug>.md`. Fill in **only the frontmatter** (`status: queued`, `passes: 0`, `added: <today>`). Leave every content section as the template comment. Don't summarise the paper.
4. Ask the user **why** it's on the list (one line). Add a row to `reading-list.md` with their words.

## Existing paper (note already exists)
1. Ask what this pass focused on. Increment `passes`, set `last_read`, and ask whether the status should change (`skimmed` / `deep-read`).
2. Quiz them with 3 questions drawn from the paper itself (fetch it if needed). Aim at its core mechanism, its key evidence and its weakest assumption. Ask them one at a time. Don't grade generously: if an answer is vague, say which part is missing.
3. Tell them to add a line to the note's `## Pass log` themselves.

Never write into the content sections of the note.

End with:
---
**Next step:** Read it. When the note has content, run `/phd:critique papers/<file>`.
