# Felipe Almeida

Personal academic website, built with [Quarto](https://quarto.org/) and published with GitHub Pages.

**Website:** https://felipeeconomist.github.io/
**Contact:** falmeida2\@huskers.unl.edu

## How the site is organized

| File or folder | What it holds |
|---|---|
| `index.qmd` | Home page: profile, research interests, recent events, featured projects |
| `education.qmd` | Degrees, advisors, scholarships and awards |
| `research.qmd` | Research page. Its entries come from `publications.yml` |
| `publications.yml` | All papers, reports, op-eds, presentations and talks |
| `projects.qmd` | Projects page. Its cards come from the files in `projects/` |
| `projects/` | One `.qmd` file per project |
| `experience.qmd` | Teaching and professional experience, skills |
| `_templates/` | Templates that turn `publications.yml` and `projects/` into cards |
| `styles.css` | Site styles |
| `_quarto.yml` | Site settings: menu, footer, theme, metadata |
| `FelipeAlmeida-CV.pdf` | CV offered for download |
| `docs/` | Generated site that GitHub Pages serves. Do not edit by hand |

## How to update the site

1. Edit the source files (`.qmd`, `publications.yml`, `projects/`, or replace `FelipeAlmeida-CV.pdf`).
2. Run `quarto render` in this folder. It rebuilds everything in `docs/`.
3. Commit the source files **and** `docs/`, then push to `main`.

### Add a publication

Add an entry to `publications.yml` under the right `section`. Entries appear in the order they are written in the file.

### Add a project

Copy `projects/_template.qmd` to a new file in `projects/`, fill it in, and remove the `draft: true` line when it is ready.
Set `home: true` to also show it on the home page.
