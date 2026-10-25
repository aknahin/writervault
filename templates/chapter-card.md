# Chapter card — the canonical chapter contract

Every chapter in the manuscript pipeline is one row in your chapter log, kept to the column spec below. This file is the canonical contract: the columns, their meanings, the word-count rollups and the front-matter keys. Copy it into your vault next to your project card and keep it at hand while the log grows — when in doubt, this file wins.

## Column spec

| Ch | Title | POV | Status | Words | Last edited |
|---|---|---|---|---|---|

Glossary:

- `Ch` — an integer, unique, 1..N. Plain integers in the table, no prefixes of any kind.
- `Title` — free text. Working titles are fine; they get renamed in revision like everything else.
- `POV` — a character from your bible (`templates/character-dossier.md`) or a name of your own. Spell it identically everywhere so counts stay honest.
- `Status` — one of the five ladder words: idea, draft, revise, polished, submitted.
- `Words` — a non-negative integer. Markdown tables may show thousands separators (`3,180`); front-matter and note bodies carry the plain integer (`3180`). Both forms describe the same number; only one of them survives a machine read.
- `Last edited` — a date, `YYYY-MM-DD`. Empty only when `Status` is `idea`.

Example row:

> Example: | 12 | Smuggler's Arithmetic | Orrin Tal | revise | 3,180 | 2026-09-14 |

## Word-count rollups

The same four formulas live here as on the project card, because the log is where the numbers come from:

- Project words = the sum of every chapter's `Words`.
- Progress % = project words ÷ target × 100 (1 decimal).
- Remaining = target − project words.
- Average chapter target = target ÷ chapter count.

Scene rows break a chapter down via `templates/scene-card.md`; the chapter's `Words` equals the sum of its scene `Words`.

## Front-matter contract

If you keep one note per chapter (recommended — it is what makes the export recipe in `reference/manuscript-export.md` work), start each note with these keys, in this order, one key per line, values with no quotes:

```yaml
---
ch: 12
title: Smuggler's Arithmetic
pov: Orrin Tal
status: revise
words: 3180
last_edited: 2026-09-14
---
```

Two details that break things when wrong: `words:` is the plain integer (`3180`), never `3,180` — separators break any tool that reads the number; and `last_edited:` stays off the note entirely (or empty) while the chapter is still `idea`.

## Note-file naming

Name chapter notes `chapter-NN.md` with a zero-padded 2-digit number: `chapter-01.md` … `chapter-24.md`. Two digits sort correctly past nine, which keeps the shell glob in `reference/manuscript-export.md` producing chapters in chapter order. Past 99 chapters the two-digit sort breaks; almost no manuscript meets that problem, and if yours does, keep the padding and compile by hand.
