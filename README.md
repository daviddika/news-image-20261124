# The World in One Image — 24 November 2026

[![make.fun · news-image-20261124](https://make.fun/badge/news-image-20261124.svg)](https://make.fun/bounty/news-image-20261124?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261124)
[![rank](https://make.fun/badge/news-image-20261124/daviddika/news-image-20261124/rank.svg)](https://make.fun/bounty/news-image-20261124/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261124)
[![reward](https://make.fun/badge/news-image-20261124/daviddika/news-image-20261124/reward.svg)](https://make.fun/bounty/news-image-20261124?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261124)

Entry for the make.fun bounty **news-image-20261124** — "Sum up 24 November's
world news in one image" ($100).

**Entrant:** Mahardika (@dika-david)

## Design

A newspaper-front-page editorial infographic, 1024×1024, in a newsprint
palette (cream paper, black ink, one red accent). The masthead names the date
**24 NOVEMBER 2026**; the lead hero covers the Russian drone entering Polish
airspace overnight, with four medium stories below it (Gaza strike, Trump's
hush-money appeal, Iran's tankers passing the US blockade, China's
Shenzhou-24 crew). A three-column "World in Brief" grid carries the other 43
stories — 48 verified stories in total across 7 regions (North America,
Latin America, Europe, Middle East, Africa, Asia-Pacific, South Asia), each
with a region tag, a one-line summary, its source, and a confidence marker
(● HIGH / ◐ MEDIUM). Claims are worded as claims. All graphics are drawn in
code (inline SVG/CSS) — no photographs or copied artwork.

## Files

- `entry.png` — the rendered entry image (1024×1024, ≤1 MiB)
- `src/frontpage.html` — the front-page source (single self-contained HTML file)
- `main.ts` — validates `entry.png` (PNG magic, ≤1 MiB, ≤1024×1024, IEND
  trailer) and copies it to `$MAKEFUN_OUTPUT_DIR/entry.png` (default
  `/output/entry.png`). Node 22, standard library only, no network.
- `NOTES.md` — evidence trail: all 48 stories with region, field, source and
  confidence, plus the date-verification note
- `LICENSE` — MIT
- `.makefun/owner.json` — entrant wallet

## Run

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out node main.ts
```
