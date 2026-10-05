# Compress to Predict

Website of the research-track project (parcours recherche, CentraleSupélec, L2S).
Static site: no build step, no dependencies to install.

## Files

- `index.html`: the whole page (text, styles, interactive figures).
- `notebook.js`: announcements and weekly sessions. The only file to edit during the year.

## Preview locally

Open `index.html` in a browser. Formulas need an internet connection (MathJax is loaded from a CDN).

## Publish on GitHub Pages (once)

    git init
    git add .
    git commit -m "First version of the project site"
    git branch -M main
    git remote add origin git@github.com:<user>/<repo>.git
    git push -u origin main

Then on GitHub: Settings > Pages > Source "Deploy from a branch", branch `main`, folder `/ (root)`.
The site appears at `https://<user>.github.io/<repo>/` after about a minute.

## Update

Edit `notebook.js` (or `index.html`), then:

    git commit -am "Session 3"
    git push
