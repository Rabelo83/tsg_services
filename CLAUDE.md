# CLAUDE.md — Project Context for AI Assistants

This file gives any AI assistant (Claude, Copilot, Cursor, etc.) the context needed to contribute effectively to this project.

---

## What this project is

**TSG Services Academy — Curso de Inmigración**

A self-contained, static interactive presentation for a Spanish-language in-person immigration course taught by **Tatiana Serrate** in **Houston, Texas**. The presentation runs entirely in the browser with no build step — just open `index.html`.

The course covers U.S. immigration topics (visas, green cards, asylum, etc.) and is designed to be projected in a classroom setting as well as shared digitally via a public link.

---

## Repository & hosting

| Item | Value |
|------|-------|
| GitHub repo | https://github.com/Rabelo83/tsg_services |
| GitHub user | Rabelo83 |
| Owner email | evanrabelo@gmail.com |
| Live site | Published via **GitHub Pages** from the `main` branch, root folder |
| Live URL pattern | `https://rabelo83.github.io/tsg_services/` |

---

## File map

| File | Purpose |
|------|---------|
| `index.html` | Main entry point — the full interactive slide deck |
| `presentacion_completa.html` | Legacy URL; redirects to `index.html` |
| `404.html` | Catches unknown paths and redirects to root |
| `.nojekyll` | Tells GitHub Pages to skip Jekyll processing |
| `*.jpeg` | Flyer images embedded in specific slides |
| `*.pdf` | Supporting materials (class notes, TSG Services brochure) |
| `README.md` | Spanish-language setup guide for GitHub Pages deployment |
| `CLAUDE.md` | This file |

---

## Tech stack

- **Pure HTML + CSS + vanilla JavaScript** — no framework, no bundler, no npm.
- Font: **Montserrat** via Google Fonts.
- Color palette: black `#0D0D0D`, gold `#C9A84C`, beige `#F5EDD6`.
- Everything ships from the root; no build or compile step is needed.

---

## Slide deck features

- 17 slides navigable by keyboard arrows, on-screen buttons, and touch swipe.
- Shareable deep-links per slide via URL hash (e.g. `#s5`).
- Browser history integration (back/forward works).
- Fullscreen toggle in the nav bar.
- Responsive — works on mobile and desktop.
- Social meta tags (Open Graph + Twitter Card) for link previews.

---

## Design conventions

- Slides are `<section class="slide" id="sN">` elements inside `.deck`.
- Active slide gets class `active`; all others are `display:none`.
- CSS variables for colors are defined in `:root` at the top of `index.html`.
- Navigation JS lives at the bottom of `index.html`.
- Keep all slide content inside `index.html` — do not split into separate HTML files.

---

## Deployment

No CI/CD pipeline. To publish:
1. Push to `main` on GitHub.
2. GitHub Pages automatically serves the updated site within ~1 minute.
3. No build command needed.

---

## Language

- **UI and slide content**: Spanish (es-US).
- **Code comments and this file**: English is fine.
- The `lang` attribute on `<html>` is `es`.

---

## Key contacts

| Role | Name |
|------|------|
| Course instructor | Tatiana Serrate |
| Developer / repo owner | Evan Rabelo (Rabelo83) |
