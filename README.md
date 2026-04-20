# aravinthakshan.github.io

Personal site + minor-project research workspace.

Live site: **https://aravinthakshan.github.io**

## Repository layout

```
.
├── README.md                                     this file
├── index.html                                    landing page
├── projects.html                                 projects listing
├── projects/
│   └── minor-project/
│       ├── index.html                            GraphIDS baseline-study deck
│       └── figures/
│           ├── fig1-detection-overview.png         Fig. 1  — anomaly detection via reconstruction
│           ├── fig2-graph-construction.png         Fig. 2  — NetFlow → graph construction
│           ├── fig3-pipeline.png                   Fig. 3  — E-GraphSAGE + Transformer pipeline
│           └── tab3-results.png                    Table 3 — empirical performance
└── papers/
    └── graphids-neurips2025.pdf                  baseline paper (arXiv 2509.16625)
```

## Publishing (GitHub Pages)

This is a **user site** — the repository must be named exactly `aravinthakshan.github.io`. No Jekyll, no build step.

1. Push this repo to `github.com/aravinthakshan/aravinthakshan.github.io`.
2. On GitHub → **Settings → Pages**:
   - Source: **Deploy from a branch**
   - Branch: **main**
   - Folder: **/ (root)**
3. Wait ~1 minute. Site is live at `https://aravinthakshan.github.io`.

## Local preview

```bash
python3 -m http.server 8000
# open http://localhost:8000/
```

Use `←` / `→` arrow keys to navigate the deck.

## Adding a new project

1. Create `projects/<slug>/index.html` (self-contained HTML).
2. Add a new `<a class="project">…</a>` entry inside `projects.html`.

No routing, no config — just add files.

## Citing the baseline

> Guerra, J. L., et al. *GraphIDS: Self-supervised graph representations for network intrusion detection.*
> NeurIPS 2025. arXiv:2509.16625.
