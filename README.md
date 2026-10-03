# multilingual

English learning notebooks, published with GitHub Pages from the `gh-pages` branch.

Live site: https://r0963033043.github.io/multilingual/

## Pages

| Page | File | Description |
| --- | --- | --- |
| Home | `projects.html` | Landing page with a card for each notebook |
| Vocabulary | `Voc.html` | IELTS word list with meanings, example sentences, and quizzes |
| Writing Notes | `Writing Notes.html` | IELTS writing notes and patterns, with a table of contents |
| Phrasing Notes | `Phrasing notes/Phrasing Notes.dc.html` | Natural phrasing and expressions, EN / 中文 |

`index.html` redirects to `projects.html`. Every notebook has a `←` button in its header that returns to the home page.

## Structure

- `index.html` — redirects to the home page
- `projects.html` — home page; cards are generated from the `projects` array in its script
- `styles.css` / `theme.js` — shared dark theme and theme toggle for the home page
- `Voc.html`, `Writing Notes.html` — self-contained single-file notebooks
- `Phrasing notes/` — Phrasing Notes page plus its data
  - `phrasing-data.json`, `phrasing-en.json` — phrasing entries (the only source of truth)
  - `support.js` — runtime for the page

All links are relative, so the site works both on GitHub Pages and when the files are opened locally.

## Adding a notebook

1. Add the HTML file (and any assets) to the repo.
2. Add an entry to the `projects` array in `projects.html` with `href`, `icon`, `title`, and `desc`.
3. Add a back link to the new page's header pointing to `projects.html`.

## Conventions

- Interactive pages use a dark background.
- Files use CRLF line endings.
