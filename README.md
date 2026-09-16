# Enveral — Redesign Concept

A UI/UX-only redesign concept for [Enveral](https://enveral.com). This is a static
mockup — no backend, no real AI processing, no auth. Enveral does one thing: turn a
long-form video into short, shareable clips (upload a file or paste a link, AI finds
the best moments, export captioned/cropped clips) — the same category and workflow as
Opus Clips.

## Why this exists

The live site currently mixes three different visual systems: a dark violet/magenta
marketing homepage, a separate creation-studio page, and a completely different light
dashboard for the account area — plus a stock-photo-style logo. This concept proposes
one consistent system across all of it, matching the visual language of an existing
`enveral-vercel.vercel.app` reference build (light surfaces, Figtree type, a single
indigo accent, near-black pill buttons).

## Design system

- **Palette** — white/soft-gray surfaces, near-black ink for primary actions, a single
  indigo accent (`oklch(0.55 0.19 272)`) reserved for badges, links and active states.
- **Type** — Figtree throughout, matching the reference build.
- **Logo** — a simple waveform glyph, replacing the old photographic circular badge.
- **Components** — pill buttons, rounded cards, an icon-rail app shell, and a vertical
  clip-card grid shared by the studio and dashboard.

## Pages

| Page | Purpose |
|---|---|
| [`index.html`](index.html) | Marketing homepage |
| [`studio.html`](studio.html) | Upload / paste-link / generate-clips flow |
| [`dashboard.html`](dashboard.html) | Account home — stats, recent clips, library |
| [`pricing.html`](pricing.html) | Free / Pro / Team tiers |

## Running locally

No build step — it's plain HTML/CSS.

```bash
python3 -m http.server 4173
```

Then open `http://localhost:4173`.

---

UI/UX concept only — not affiliated with or deployed to the production Enveral product.
