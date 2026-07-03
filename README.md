# 🌽 Cornhole Bracket

A lightweight, mobile-first single-page tournament bracket for cornhole (or any
head-to-head game). No backend, no build step — one self-contained `index.html`
you can open locally or host free on GitHub Pages.

## Features

- **Single & double elimination.**
- **Real bracket flow** — left-to-right columns with connector lines, rendered as three
  color-coded sections (winners = green, losers = amber, grand final = purple).
- **Any team count 2–32** — not just powers of two. Top seeds get first-round byes,
  which auto-advance and cascade correctly into the losers bracket.
- **Standard seeding** (1 vs last, 2 vs second-last, …) kept consistent through the bracket.
- **Auto-advancing winners** — tapping "Win" records the result and moves the team on.
- **Big tap targets** — designed to be used one-handed on a phone at an outdoor tournament.
- **Multi-level undo** — revert results one at a time all the way back to the start.
- **Auto-save** — progress is stored in `localStorage`, so a refresh never loses the bracket.
- **Champion banner** when the tournament resolves.
- **New Tournament** reset (with confirm).

Players per team (1–4) and player names are optional and shown under each team.

### Double elimination

- Winners-bracket losers drop into the losers bracket; the winners-final loser enters
  the losers final.
- Grand final: winners-bracket champion vs losers-bracket champion.
- **Bracket reset** (setup toggle, default **off**): if the losers-bracket team wins the
  grand final, a single deciding game is played. With it off (casual rule), the losers
  team winning the grand final ends the tournament immediately.

## Use it
[JoyCollect live site](https://brettcookie40.github.io/Cornhole-Bracket/)

In test:
Open `index.html` in any modern browser — that's it. Nothing to install.

## Deploy to GitHub Pages

Serve from the root of the `main` branch (Settings → Pages → Source: `main` / `/root`).
The live site is just the static `index.html`.
