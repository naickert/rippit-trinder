# Trinder

A Tinder-style swipe prototype for **[Rippit](https://staging.rippit.games/)** — a provably-fair "rip packs, collect the set, win the jackpot" platform. Browse premium foil packs, set your price, and rip them open for a card reveal with real cash sell-back value.

Single-file, self-contained HTML (no build step, no dependencies beyond a webfont). Open it on a phone for the intended mobile experience.

## Live demo

▶ **https://naickert.github.io/rippit-trinder/**

## Files

| File | What it is |
|------|------------|
| `index.html` | The current prototype (v2) — the main experience |
| `trinder.html` | v1 — the original Tinder-style swipe deck |
| `rippit-prototype.html` | An earlier prototype |

## How to use (`index.html`)

- **Swipe ← / →** (or the `‹ ›` chevrons) — change the pack **theme** (collection) at the same price.
- **− / +** stepper — change the **price**; tier, "up to" ceiling, and card values all scale with it.
- **OPEN** — rip one pack. **BUY 5** — rip five at once (cost = 5 × price).
- **⚡ Fast toggle** (left of Buy 5):
  - **Off** (default) — review each card one at a time: **swipe ← to sell**, **swipe → to collect**.
  - **On** — instant bulk reveal; one Keep / Cash-out decision for the whole batch.
- **Wallet / Sold / Collection** stay visible and update live while you resolve a pack.

### Keyboard
`← →` theme · `O` open · `B` buy 5 · `M` more · in review: `←`/`S` sell, `→`/`C` collect.

## Design

Built to Rippit's brand: deep navy / quilted backdrop, metallic foil packs (gold, platinum, crimson, emerald, violet, sapphire), electric-teal and gold accents, Space Grotesk. Card art uses emoji placeholders — swap in real artwork by editing the `COLLECTIONS` data in `index.html`.

> Prototype only. Pulls are simulated client-side using Rippit's published rarity odds (Common 53% · Uncommon 34.5% · Rare 10% · Epic 2% · Legendary 0.5%); no real money or backend.
