# Guided Mode — Nubra Strategy Builder Case Study Site

Mirrors the ChargeClarity case-study site structure (same `styles.css` design system,
same `script.js` scroll/nav behavior), rebuilt around the Nubra product case study notebook.

## Screens

All 6 screens generated via Stitch, then exported into Figma for the linked frames.

| # | File | What it shows | Figma |
|---|------|----------------|-------|
| 1 | `screens/screen1-current-builder.png` | Today: Advanced Builder, empty/unguided — the pain point | [View](https://www.figma.com/design/M63PY6gp4W72lUhAD3aGKY/Untitled?node-id=1-2&t=C7nLLQO0K4F7uaIn-1) |
| 2 | `screens/screen2-guided-toggle.png` | Strategy Builder landing with Guided Mode toggle, on by default | [View](https://www.figma.com/design/M63PY6gp4W72lUhAD3aGKY/Untitled?node-id=1-304&t=C7nLLQO0K4F7uaIn-1) |
| 3 | `screens/screen3-market-view.png` | Guided wizard step 1 of 3 — market outlook (Bullish/Bearish/Neutral) | [View](https://www.figma.com/design/M63PY6gp4W72lUhAD3aGKY/Untitled?node-id=3-182&t=C7nLLQO0K4F7uaIn-1) |
| 4 | `screens/screen4-risk-appetite.png` | Guided wizard step 2 of 3 — risk tolerance | [View](https://www.figma.com/design/M63PY6gp4W72lUhAD3aGKY/Untitled?node-id=2-3&t=C7nLLQO0K4F7uaIn-1) |
| 5 | `screens/screen5-recommended-strategies.png` | Guided wizard step 3 of 3 — Iron Condor / Iron Butterfly matches (Hero Screen) | [View](https://www.figma.com/design/M63PY6gp4W72lUhAD3aGKY/Untitled?node-id=3-369&t=C7nLLQO0K4F7uaIn-1) |
| 6 | `screens/screen6-prefilled-builder.png` | Advanced Builder, auto-filled via Guided Mode, payoff live (Hero Screen) | [View](https://www.figma.com/design/M63PY6gp4W72lUhAD3aGKY/Untitled?node-id=3-579&t=C7nLLQO0K4F7uaIn-1) |

## Project Structure

```
nubra-case-study/
├── index.html                          # Main case study page (multi-file, for hosting/GitHub Pages)
├── styles.css                          # ChargeClarity's design system + benchmark-table/pill/chart-card additions
├── script.js                           # Scroll progress, nav highlighting, reveal animations (unchanged from ChargeClarity)
├── README.md                           # This file
├── charts/                             # Real matplotlib output, regenerated from nubra_product_case_study.ipynb
│   ├── funnel-by-segment.png
│   ├── ab-completion-comparison.png
│   ├── ab-distribution.png
│   ├── sensitivity-analysis.png
│   └── wireframe-diagram.png
└── screens/                            # Figma screens
    ├── screen1-current-builder.png
    ├── screen2-guided-toggle.png
    ├── screen3-market-view.png
    ├── screen4-risk-appetite.png
    ├── screen5-recommended-strategies.png
    └── screen6-prefilled-builder.png
```

`index.html` references `screens/`, `charts/`, `styles.css`, and `script.js` by relative
path — keep all of them alongside it when hosting (GitHub Pages, Netlify, etc).

## Running Locally
Open `index.html` in any browser 
