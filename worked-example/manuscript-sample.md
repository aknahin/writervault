# Worked example — manuscript sample

This file shows a fictional writer, **Wren Calloway**, and her fictional novel **The Salt Cartographer** (adult fantasy, 90,000-word target) across July–October 2026: the project card as filled, a 24-row chapter log, a scene breakdown of chapter 12, and a four-week sprint log. All names of people, agencies, venues, titles and figures in this worked example are fictional, and every figure is sample data for demonstration only.

> **Sample note:** this repository is a free sample — it includes only this file from `worked-example/`, so the dashboards referenced below ship with the full kit rather than here. All figures below are fictional sample data.

Every number here is internally reconciled: the rollups in `dashboards/pipeline-dashboard.md` recompute from these tables exactly — status word sums add to 69,080 against a 90,000 target, the five chapter-12 scenes sum to that chapter's 3,180 words, and the sprint log totals 18,600 words over 20 sessions. Copy the shapes, replace the content, keep the columns.

## Project card (filled)

| Field | Value |
|---|---|
| Title | The Salt Cartographer |
| Genre | adult fantasy |
| Target words | 90,000 |
| Status | revising |
| Draft started | 2026-06-01 |
| Query started | 2026-07-06 |

## Chapter log

| Ch | Title | POV | Status | Words | Last edited |
|---|---|---|---|---|---|
| 1 | The Chart at Low Tide | Mira Venn | submitted | 3,150 | 2026-08-02 |
| 2 | Harbor of Borrowed Names | Mira Venn | submitted | 3,420 | 2026-08-05 |
| 3 | Orrin's Knot | Orrin Tal | submitted | 2,980 | 2026-08-09 |
| 4 | The Lantern Grid | Mira Venn | submitted | 3,610 | 2026-08-14 |
| 5 | Salt Debt | Mira Venn | polished | 3,240 | 2026-08-18 |
| 6 | Maps That Lie | Mira Venn | polished | 3,050 | 2026-08-21 |
| 7 | The Undertow Market | Orrin Tal | polished | 3,480 | 2026-08-26 |
| 8 | Grandmother Halcyon | Mira Venn | polished | 3,120 | 2026-08-30 |
| 9 | Bellweather | Isolde Bray | polished | 3,760 | 2026-09-03 |
| 10 | The Eighth Lens | Mira Venn | polished | 3,330 | 2026-09-07 |
| 11 | What the Tide Remembers | Mira Venn | revise | 2,940 | 2026-09-11 |
| 12 | Smuggler's Arithmetic | Orrin Tal | revise | 3,180 | 2026-09-14 |
| 13 | The Auditor's Ledger | Isolde Bray | revise | 3,410 | 2026-09-18 |
| 14 | Paper Saints | Mira Venn | revise | 3,070 | 2026-09-22 |
| 15 | A Map of the Missing | Mira Venn | revise | 3,520 | 2026-09-26 |
| 16 | Saltmere Burning | Mira Venn | draft | 3,290 | 2026-10-01 |
| 17 | The Covenant Breaks | Orrin Tal | draft | 3,640 | 2026-10-05 |
| 18 | Drowned Ground | Mira Venn | draft | 2,870 | 2026-10-09 |
| 19 | The Cartographer's Choice | Mira Venn | draft | 3,350 | 2026-10-14 |
| 20 | High Water | Isolde Bray | draft | 3,910 | 2026-10-18 |
| 21 | All the Living Charts | Mira Venn | draft | 2,760 | 2026-10-22 |
| 22 | The Last Tide | Mira Venn | idea | 0 |  |
| 23 | Home is a Harbor | Mira Venn | idea | 0 |  |
| 24 | Epilogue: The New Chart | Mira Venn | idea | 0 |  |

## Scene breakdown — Chapter 12

| Scene | Ch | POV | Location | Status | Words |
|---|---|---|---|---|---|
| SC-056 | 12 | Orrin Tal | Undertow Market - stall row | polished | 610 |
| SC-057 | 12 | Orrin Tal | Undertow Market - back room | revise | 720 |
| SC-058 | 12 | Mira Venn | Harbor office | revise | 545 |
| SC-059 | 12 | Orrin Tal | Smuggler's skiff | draft | 690 |
| SC-060 | 12 | Mira Venn | Lantern stair | polished | 615 |

Rule: the scene words sum to 3,180 = chapter 12 `Words`. The chapter's `revise` status is the writer's editorial call, not a function of the mixed scene statuses above it.

## Sprint log (last 4 weeks)

| Week starting | Sessions | Words drafted | Cumulative |
|---|---|---|---|
| 2026-09-28 | 5 | 4,150 | 4,150 |
| 2026-10-05 | 6 | 5,480 | 9,630 |
| 2026-10-12 | 4 | 3,220 | 12,850 |
| 2026-10-19 | 5 | 5,750 | 18,600 |
| **Total** | **20** | **18,600** | — |

The rollups derived from these logs — status shares, progress, sprint pace, POV split — live in `dashboards/pipeline-dashboard.md`, worked out from exactly these rows.
