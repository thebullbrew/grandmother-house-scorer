# The Grandmother House Scorer

![banner](assets/banner.jpg)

**Live app:** https://thebullbrew.github.io/grandmother-house-scorer/

The holy-grail deal filter, as an app. Score any listing against the grandmother-house method:

- **Good bones** — foundation, layout, structure, lot. What you can't cheaply change.
- **Systems — the risk** — roof, HVAC, plumbing, electrical, water heater. Where deals die.
- **Cosmetics — the discount** — kitchen, baths, flooring, walls, windows. Ugly is the opportunity.
- **The money** — rehab estimate ranges, max allowable offer (70% rule), asking-vs-offer gap, gross rent yield vs the 1% rule.

Verdicts run from **"Holy grail"** down to **"Pass."** Save deals to a local pipeline, rank them, buy the best one.

## The method

> Long-tenure owner. Maintained systems. Dated cosmetics. Good bones.
> Cosmetics are the discount — systems are the risk.

A grandmother house is the ideal buy-renovate-rent deal: an owner who took pride in the home and kept the big-ticket systems maintained, but whose taste froze sometime in the 70s. You buy the discount the wallpaper creates and avoid the risk a dead furnace creates. This scorer turns that judgment into a repeatable 0–100 filter.

## Run it

No build step. Open `docs/index.html` in a browser, or visit the live link above. It's a PWA — Add to Home Screen on iPhone for the full app feel. Works offline after first load; saved deals stay in the browser via localStorage.

## Scoring

| Component | Weight | What it measures |
|---|---|---|
| Good bones | 30% | Structural/layout checks passed |
| Systems | 30% | 100 minus weighted age-risk of roof, HVAC, plumbing, electrical, water heater |
| Cosmetic discount | 25% | How dated the finishes are — worse looking, bigger opportunity |
| Margin | 15% | Spread between asking + rehab and ARV (skipped if ARV unknown) |

Rehab ranges are planning estimates per finish level, not contractor quotes. Always verify with your own eyes.

## Deploy your own

Static files under `docs/` — publish with any static host (this repo uses GitHub Pages).

---

*Part of the daily finance & real-estate tool series. One useful tool, every day.*
