# AGENTS.md

Shared context for AI collaborators working in this repository.

## Project Summary

- This repo contains a static GitHub Pages presentation for `TSG Services Academy`.
- The presentation promotes and explains a Spanish-language, in-person immigration course in Houston, Texas.
- Instructor shown in the current content: `Tatiana Serrate`.
- This is a slide deck, not a traditional multi-page app.
- The current presentation has `17` slides total, including the promotional flyer gallery slide `#spromo`.

## Repo Identity

- Local folder name: `curso_migraciones`
- GitHub remote repo: `https://github.com/Rabelo83/tsg_services.git`
- GitHub account / repo owner: `Rabelo83`
- Local git identity configured in this repo: `Rabelo83 <Rabelo83@users.noreply.github.com>`

## Stack And Structure

- No framework and no build step.
- Main file: `index.html`
  - Contains the markup, styles, and JavaScript for the full presentation.
- `presentacion_completa.html`
  - Legacy entry point that redirects to `index.html`.
- `404.html`
  - Redirects visitors back to the presentation.
- `*.jpeg`
  - Promotional flyer assets used in the deck.
- `*.pdf`
  - Supporting course materials and project deliverables.

## Deployment

- Intended for GitHub Pages.
- `README.md` says deployment should use branch `main` and folder `/ (root)`.
- Because there is no build step, publishing is just serving the files in this folder.

## Important Content Details

- Brand name: `TSG Services Academy`
- Course title: `Curso de Inmigracion`
- Language of the site content: Spanish
- Current location shown in the deck: `5870 Highway 6 N, Houston, TX 77084 Suite 314`
- Current schedule shown in the deck: `Julio 4 y 5`, `8:30 AM - 3:30 PM`
- Current price shown in the deck: `$799.00`
- Current availability shown in the deck: `11 cupos`

## Editing Notes

- Preserve the current black / gold / beige visual language unless the user asks for a redesign.
- Keep the Spanish marketing copy unless the user explicitly asks for copy changes or translation.
- If you update logistics like date, time, price, location, or seat count, check repeated values in:
  - top metadata in `index.html`
  - slide `#s1`
  - closing slide `#s16`
- Slide navigation depends on hash IDs like `#s1`, `#spromo`, and `#s16`.
- Do not rename slide IDs unless you also update the JavaScript navigation logic.
- `index.html` includes keyboard navigation, swipe navigation, fullscreen mode, hash-based deep links, and a lightbox for flyer previews.
- Do not delete flyer images or PDF files unless the user explicitly asks for it.

## Suggested First Files To Read

- `README.md`
- `index.html`

## Notes For Future AI Sessions

- Prefer direct edits to the existing static files instead of adding tooling.
- If facts like dates, pricing, address, or availability look stale, ask for confirmation before changing them.
- When making social/share updates, also review the `meta` and Open Graph tags near the top of `index.html`.
