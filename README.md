# GiftKit — Never Give a Boring Gift Again

A single-file gift planner that remembers every birthday, every budget and every
gift you've already given — so the next one lands perfectly.

**Live:** https://abhiramunni.github.io/giftkit/

## What it does

- **Occasions on the horizon** — a horizontal countdown rail of birthdays,
  anniversaries and festivals, each with days left, a budget, and whether a
  gift has been picked, bought, or not thought of yet.
- **Gift Finder** — stuck? Pick the person, set a budget, choose a vibe
  (thoughtful / practical / fun / keepsake) and GiftKit ranks the three best
  ideas from your vault, each with a plain-words reason it fits them.
- **People** — every person you buy for, with what they love, their per-person
  budget, their last gift, and a full gift history — so you never repeat a gift.
  GiftKit warns you before you buy the same thing twice.
- **Idea Vault** — 12 seeded ideas across 8 categories, searchable, filterable
  and sortable. Save any idea you spot and attach it to an occasion, or mark it
  given straight from the vault.
- **Budget, honestly** — one yearly budget (default ₹12,000), a progress ring,
  and spent-per-person bars, all counted from your real gift history.
- **Last-minute lifesavers** — four under-₹750 gifts you can buy today, with
  one-tap save to the vault.
- **Guides** — six short, plain rules for generous, appropriate gifting.
- **Settings** — yearly budget, reminder lead time, copy-my-summary, remove
  sample data, two-tap erase-all.

## Details

- Single self-contained `index.html` — no backend, no signup, no tracking.
  All data lives in `localStorage` (`giftkit-v1`).
- Warm editorial design (ivory paper, espresso ink, bronze/amber/terracotta),
  Fraunces + Inter, cinematic intro with tap-to-skip (quick on return visits),
  3-step onboarding coach, Ken Burns photography.
- Seeded with clearly-marked sample people, occasions and ideas — remove them
  with one tap and start from a clean slate.
- Prices are indicative; check the shop before you buy.

## QA

- `node --check` clean.
- 59/59 headless jsdom assertions pass (`qa-test.js`): seed state, date math
  (next occasion: Appa's Birthday, 6 days), money math (₹5,794 spent in 2026
  of a ₹12,000 budget = 48%), no-repeat detection, finder scoring and ranking,
  vault search/filter/sort, finder UI, mark-bought flow, intro skip, and a
  no-pictographic-emoji check.

## How to use

Open the live link, skim the 3-step tour, then add your real people and
occasions. When you're stuck, use the Gift Finder. When you give a gift, log
it — that's what keeps the budget honest and the repeats away.
