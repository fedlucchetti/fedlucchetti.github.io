# Federico Lucchetti — personal site

Static academic profile page for GitHub Pages, served at
`https://fedlucchetti.github.io/` once published.

Single-file site (`index.html`): markup, CSS and a small script for the
Expertise pop-ups, with no build step. It follows the system light/dark setting.

## Structure

- `index.html` — the whole site: sidebar profile with links, then About,
  Expertise, Experience & education, Publications and Software.
- `images/profile.jpg` — profile photo (500 × 600, cropped from the lab-site
  headshot).
- `images/expertise/` — the four Expertise thumbnails, also shown at the top of
  each pop-up.

## Updating

- **Publications**: each entry is an `<li>` in `#publications`, under either
  "Journal articles" or "Preprints", newest first. Your name is wrapped in `<b>`.
  When a preprint is published, move it to "Journal articles" and swap in the
  journal DOI. The list was assembled from ORCID, Crossref and arXiv in
  November 2026.
- **Expertise**: each card is a `<button class="topic" data-topic="…">`. Its
  pop-up text lives in the matching `<template id="topic-…">`, and the
  template's `data-pubs` lists the ids of the `<li>` entries from
  `#publications` to feature. Every publication `<li>` has an id for this. Each
  pop-up has its own address, e.g. `#expertise/metabolic-connectomics`.
- **Footer**: update "Last updated" when you change the content.

## Publishing to GitHub Pages

1. Create a public repository named exactly `fedlucchetti.github.io` under the
   `fedlucchetti` account.
2. Push this folder's contents to its `main` branch.
3. In the repository's Settings → Pages, set the source to the `main` branch root.
4. The site goes live at `https://fedlucchetti.github.io/`.
