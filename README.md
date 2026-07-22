# Vinova Energy — Static Website

Single-page static site for **Vinova Energy Systems Pvt Ltd** (Solar PV module manufacturer & solar power integrators, Hosur, Tamil Nadu). Built as plain HTML/CSS/JS with **zero external dependencies** — ready for GitHub Pages.

## Files
- `index.html` — the entire site (inline CSS + inline SVG graphics).
- `assets/logo.png` — company logo.
- `assets/favicon.svg` — site icon.
- `.nojekyll` — tells GitHub Pages to serve files as-is.

All paths are **relative**, so the site works whether it's served from a user page
(`username.github.io`), a project page (`username.github.io/vinova.in/`), or a custom domain.

## Deploy to GitHub Pages
1. Push these files to your repository (root of the branch you publish).
2. In the repo: **Settings → Pages → Build and deployment → Source: Deploy from a branch**.
3. Choose your branch (e.g. `main`) and folder `/ (root)`, then **Save**.
4. Your site goes live at the URL shown on that page.

### Custom domain (optional)
If you point `vinova.in` at GitHub Pages, add a file named `CNAME` (no extension)
in the root containing just:
```
vinova.in
```

## Adding real photos later
The original photos couldn't be recovered, so project/hero imagery is drawn with SVG.
To use real photos:
- Drop images into an `assets/projects/` folder.
- In `index.html`, the `projects` array (in the `<script>` block) drives the gallery —
  add an `img` field per project and swap the generated `thumb()` SVG for an `<img>` tag.
