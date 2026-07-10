# Portfolio — Atif Aninda Rahman

A static, single-page academic portfolio built with plain HTML/CSS/JS (no build step), designed for GitHub Pages.

## Structure
```
index.html        → all page content (edit text directly here)
css/style.css      → all styling / design tokens (colors, type, layout)
js/main.js         → mobile nav + footer year
assets/            → put your CV PDF and project images here
```

## Before you publish — replace these
Search the codebase for square brackets `[ ... ]` and italic placeholder text — these mark
everything that needs your real info:
- Research interests statement (`#research` section)
- Work/education dates in the Experience timeline
- Publications
- Contact email + GitHub username link
- CV file: drop a PDF into `assets/` named `Atif_Aninda_Rahman_CV.pdf`
- Optional: swap the abstract SVG project graphics for real map screenshots

## Run locally
No build tools needed. Either:
- Open `index.html` directly in a browser, or
- From this folder run `python3 -m http.server 8080` and visit `http://localhost:8080`

## Deploy to GitHub Pages (via GitHub Actions)

This repo includes `.github/workflows/deploy.yml`, which auto-deploys to Pages on every push to `main`. No manual "build" step — it just uploads the site as-is on each push and gives you a deployment log in the Actions tab.

1. Create a new GitHub repo (e.g. `portfolio` or `yourusername.github.io`)
2. Push this folder's contents (including the `.github` folder) to the `main` branch
3. Repo Settings → Pages → **Source: GitHub Actions** (not "Deploy from a branch")
4. Push to `main` (or re-run manually from the Actions tab) — watch it deploy under the **Actions** tab
5. Site goes live at `https://yourusername.github.io/portfolio/` (or `https://yourusername.github.io/` if you used the special repo name)
6. Optional: add a custom domain in the same Pages settings screen

Every future push to `main` re-deploys automatically — no extra steps.
