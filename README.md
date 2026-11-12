# Federico Lucchetti — personal site

Static academic profile page for GitHub Pages, served at
`https://fedlucchetti.github.io/` once published.

Single-file site (`index.html`): markup and CSS, no JavaScript and no build
step. It follows the system light/dark setting.

## Structure

- `index.html` — the whole site: sidebar profile with links, then About,
  Experience & education, Publications and Software.
- `images/profile.jpg` — profile photo (500 × 600, cropped from the lab-site
  headshot).

## Updating

- **Publications**: each entry is an `<li>` in `#publications`, under either
  "Journal articles" or "Preprints", newest first. Your name is wrapped in `<b>`.
  When a preprint is published, move it to "Journal articles" and swap in the
  journal DOI. The list was assembled from ORCID, Crossref and arXiv in
  November 2026.
- **Footer**: update "Last updated" when you change the content.

## Publishing to GitHub Pages

1. Create a public repository named exactly `fedlucchetti.github.io` under the
   `fedlucchetti` account.
2. Push this folder's contents to its `main` branch.
3. In the repository's Settings → Pages, set the source to the `main` branch root.
4. The site goes live at `https://fedlucchetti.github.io/`.
