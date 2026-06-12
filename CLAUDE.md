# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Stack

Vanilla JS/HTML5/CSS3 — no build tools, no npm, no frameworks, no dependencies. Keep it that way.

## Running

Open `index.html` directly in a browser. No server required.

## Critical gotchas

- **Canvas dimensions must stay in sync with constants.** `COLS`, `ROWS`, and `BLOCK` are defined in `game.js`. If you change them, update the `<canvas width>` and `height` attributes in `index.html` or rendering breaks.
- **Next-piece preview uses hardcoded `NB = 30`** — not derived from `BLOCK`. Update both if changing block size.
- **`COLORS` is 1-indexed.** `COLORS[0] = null`; piece types are 1–7. Don't shift this array.

## No tests or linting

No test framework or linter configured. Verify changes by running the game in a browser.
