# Minor Project — Self-supervised graph representations for network intrusion detection

Reproduction and extension of **GraphIDS** (Guerra et al., NeurIPS 2025), with streaming (Zeek + Kafka),
packet-level feature enrichment, and methodological extensions (feature-channel masking, curriculum
masking, relative-time attention bias).

## Repository layout

```
minor-project/
├── README.md                                     this file
├── papers/
│   └── graphids-neurips2025.pdf                  baseline paper (arXiv 2509.16625)
└── site/                                         GitHub Pages source (aravinthakshan.github.io)
    ├── README.md                                   publishing instructions
    ├── index.html                                  landing page
    ├── projects.html                               projects listing
    └── projects/minor-project/
        ├── index.html                              the slide deck
        └── figures/
            ├── fig1-detection-overview.png           Fig. 1  — anomaly detection via reconstruction
            ├── fig2-graph-construction.png           Fig. 2  — NetFlow → graph construction
            ├── fig3-pipeline.png                     Fig. 3  — E-GraphSAGE + Transformer pipeline
            └── tab3-results.png                      Table 3 — empirical performance
```

## Viewing the deck locally

```bash
open site/projects/minor-project/index.html        # macOS
# or
python3 -m http.server 8000                        # then visit http://localhost:8000/site/
```

Use `←` / `→` arrow keys to navigate slides.

## Citing the baseline

> Guerra, J. L., et al. *GraphIDS: Self-supervised graph representations for network intrusion detection.*
> NeurIPS 2025. arXiv:2509.16625.
