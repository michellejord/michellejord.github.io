# michellejord.github.io

Personal website for Michelle Alicia Jordan. Built with [Quarto](https://quarto.org/), deployed via GitHub Pages from the `docs/` folder.

## Local preview

```bash
quarto preview
```

Opens at <http://localhost:4444> (or similar) with live reload.

## Build

```bash
quarto render
```

Output is written to `docs/` — this is what GitHub Pages serves.

## Deploy

```bash
quarto render
git add -A
git commit -m "update site"
git push
```

GitHub Pages is configured to serve from the `main` branch, `/docs` folder.

## File map

| File | Purpose |
|---|---|
| `_quarto.yml` | Site config (navbar, theme, output dir) |
| `index.qmd` | Home / about page |
| `research.qmd` | Working papers and WIP |
| `cv.qmd` | HTML CV + link to PDF |
| `styles.css` | Custom CSS (muted pink accent) |
| `files/CV_MichelleAliciaJordan.pdf` | Downloadable CV |
| `.nojekyll` | Tells GitHub Pages not to run Jekyll on `docs/` |

## To do before going live

1. Replace the two `href: "#"` placeholders in `research.qmd` with the actual paper links.
2. (Optional) Drop a `profile.jpg` in the project root and uncomment `image:` in `index.qmd`'s YAML.
3. Re-copy the CV into `files/` whenever it's updated.
