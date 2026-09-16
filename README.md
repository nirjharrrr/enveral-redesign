# Enveral — Redesign Concept

A UI/UX-only redesign concept for [Enveral](https://enveral.com), an AI video-clipping
product. This is a static mockup — no backend, no real AI processing, no auth. It exists
to explore a consistent design system across the site and a new "call screens" feature
(live-call recording that feeds the same clip-detection pipeline as uploads).

## Why this exists

The live site currently mixes three different visual systems: a dark violet/magenta
marketing homepage, a separate creation-studio page, and a completely different light
dashboard for the account area — plus a stock-photo-style logo. This concept proposes one
consistent system across all of it, and extends the product with a new capability: turning
a live call into clips the same way an uploaded file works today.

## Design system

- **Palette** — near-black graphite base (`#0a0a0c`) with a single electric-lime accent
  (`#d7ff3f`). Red is reserved for live/recording states only.
- **Type** — Inter throughout, tight tracking on headlines.
- **Logo** — a simple waveform-into-mark glyph, replacing the old photographic circular badge.
- **Components** — pill buttons, rounded cards, an icon-rail app shell, and a vertical
  clip-card grid shared by the studio, dashboard, and call-summary screens.

## Pages

| Page | Purpose |
|---|---|
| [`index.html`](index.html) | Marketing homepage |
| [`studio.html`](studio.html) | Upload / paste-link / generate-clips flow |
| [`dashboard.html`](dashboard.html) | Account home — stats, recent clips, call history |
| [`call-lobby.html`](call-lobby.html) | **New** — pre-call device check & join screen |
| [`call-live.html`](call-live.html) | **New** — in-call view with live AI highlight detection |
| [`call-summary.html`](call-summary.html) | **New** — post-call clip review & export |

## Running locally

No build step — it's plain HTML/CSS.

```bash
python3 -m http.server 4173
```

Then open `http://localhost:4173`.

---

UI/UX concept only — not affiliated with or deployed to the production Enveral product.
