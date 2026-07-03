# 🌽 Cornhole Bracket

A lightweight, mobile-first single-page tournament bracket for cornhole (or any
head-to-head game). No backend, no build step — one self-contained `index.html`
you can open locally or host free on GitHub Pages.

## Features

- **Any team count 2–32** — not just powers of two. Top seeds get first-round byes.
- **Standard seeding** (1 vs last, 2 vs second-last, …) kept consistent through the bracket.
- **Single elimination** with auto-advancing winners.
- **Big tap targets** — designed to be used one-handed on a phone at an outdoor tournament.
- **Multi-level undo** — revert results one at a time all the way back to the start.
- **Auto-save** — progress is stored in `localStorage`, so a refresh never loses the bracket.
- **Champion banner** when the final resolves.
- **New Tournament** reset (with confirm).

Players per team (1–4) and player names are optional and shown under each team.

> Double elimination (losers bracket, grand final, optional bracket-reset toggle)
> is planned as the next milestone.

## Use it

Open `index.html` in any modern browser — that's it. Nothing to install.

## Deploy to GitHub Pages

Serve from the root of the `main` branch (Settings → Pages → Source: `main` / `/root`).
The live site is just the static `index.html`.
