# Echoveil website

A small static site for Echoveil and its Unity Editor tools. Plain HTML and CSS: no build step, no
JavaScript, no dependencies.

| File | Page |
|---|---|
| `index.html` | Home: tools, about, contact |
| `editor-plus.html` | Editor Plus product page |
| `docs/editor-plus.html` | Editor Plus user guide |
| `support.html` | Support and how to report a problem |
| `404.html` | Not-found page |
| `style.css` | Shared styles (light and dark) |
| `.nojekyll` | Tells GitHub Pages to serve the files as they are |

All links between pages are relative, so the site works at the root of a user site
(`https://USER.github.io/`) or in a project site (`https://USER.github.io/REPO/`).
The one exception is `404.html`, which uses absolute paths; see the comment in that file.

## Before publishing: fill in the placeholders

Placeholders are highlighted in yellow in the browser (the `todo` class in `style.css`):

- [ ] **Contact email**: `support@example.com` in `index.html` and `support.html`
      (a `mailto:` link and its visible text, so two places in each file).
- [ ] **Package install URL**: the `https://github.com/your-username/your-repo.git` line in `editor-plus.html`.
- [ ] **About text** in `index.html` (the HTML comment marks the spot).
- [ ] **Screenshots** in `editor-plus.html` (the HTML comment marks the spot).
- [ ] Once the placeholders are filled, remove the `todo` class from those spans.

Search the folder for `example.com`, `your-username` and `TODO` to find anything left.

## Publishing on GitHub Pages

1. Push this folder to a GitHub repository. For a site at `https://USER.github.io/`, name the repository
   `USER.github.io`. Any other name publishes at `https://USER.github.io/REPO/`.
2. In the repository: **Settings > Pages > Build and deployment > Source: Deploy from a branch**, then choose the
   `main` branch and the `/ (root)` folder, and save.
3. After a minute or so the site is live at the address shown on that settings page.

## Keeping it current

When Editor Plus changes, update the version and notes in `editor-plus.html`, and the guide in `docs/editor-plus.html`
(it mirrors the package's `Documentation~/UserGuide.md`).
