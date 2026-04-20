# aravinthakshan.github.io

Personal site — minimal, static, no build step.

## Structure

```
.
├── index.html                          Landing page
├── projects.html                       Projects index
└── projects/
    └── minor-project/
        ├── index.html                  GraphIDS baseline-study deck
        └── figures/                    Deck figures
```

## Publishing to GitHub Pages

This is a **user site** (repo must be named exactly `aravinthakshan.github.io`). No Jekyll, no workflow — GitHub Pages serves the static HTML from `main` directly.

### First-time setup

```bash
cd site/
git init
git add .
git commit -m "Initial site"
git branch -M main
git remote add origin git@github.com:aravinthakshan/aravinthakshan.github.io.git
git push -u origin main
```

Then on GitHub → `aravinthakshan.github.io` → **Settings → Pages** → set Source to `Deploy from a branch`, Branch `main`, Folder `/ (root)`. Site is live at `https://aravinthakshan.github.io` within ~1 minute.

### Subsequent updates

```bash
cd site/
git add .
git commit -m "Update deck / add project"
git push
```

## Adding a new project

1. Create `projects/<project-slug>/index.html` (self-contained HTML, like the deck)
2. Add a new `<a class="project">…</a>` entry inside `projects.html`

No routing, no config — just add files.

## Local preview

```bash
cd site/
python3 -m http.server 8000
```

Open `http://localhost:8000`.
