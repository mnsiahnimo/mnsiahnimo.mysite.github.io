# MyGitRSIte

Personal website for Michael Nsiah-Nimo, built with [Quarto](https://quarto.org/).

## Files

| File | What it is |
|---|---|
| `_quarto.yml` | Site settings: title, navbar, theme, footer |
| `index.qmd` | About / home page |
| `research.qmd` | Publications and projects |
| `uses.qmd` | "What I use" page |
| `styles.css` | Custom styling |

Search every `.qmd` and `_quarto.yml` for `[TO BE SUPPLIED` and fill those in.

## Preview locally

```bash
quarto preview
```

## Publish to GitHub Pages (first time)

1. On GitHub, create an **empty** public repo named exactly `mnsiahnimo.github.io`
   (no README, no .gitignore). That name gives you the URL https://mnsiahnimo.github.io
2. In this folder:

```bash
git init
git add .
git commit -m "First version of site"
git branch -M main
git remote add origin https://github.com/mnsiahnimo/mnsiahnimo.github.io.git
git push -u origin main
quarto publish gh-pages
```

3. On GitHub: **Settings → Pages → Source: Deploy from a branch → `gh-pages` / root**.

## Updating later

```bash
git add . && git commit -m "Update site" && git push
quarto publish gh-pages
```
