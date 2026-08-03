# Ashish Poudel — Portfolio

Personal site for **Ashish Poudel**, development finance professional and policy researcher.
Vanilla HTML and CSS, no build step, deployable on GitHub Pages or any static host.

## Structure

```
index.html   All markup + a small inline script (nav, scrollspy, reveals)
style.css    Full stylesheet, design tokens at the top in :root
assets/      Portrait, signature, CV, PTE score report
```

## Design

| | |
|---|---|
| Palette | Archival paper `#F5F3EE`, ink `#14181A`, ledger green `#1E4D3E`, brass `#9A7B32` |
| Display | Fraunces |
| Body | IBM Plex Sans |
| Data / labels | IBM Plex Mono |

All colours and fonts are declared as CSS custom properties in `:root` — change them
there and the whole site follows.

## Sections

1. Profile
2. Publications & working papers
3. Applied research
4. Professional experience
5. Credentials — education, methods, PTE scorecard
6. Contact

## Links still to be filled in

Anchors marked with `data-slot` currently point at `#`. They render in a muted,
dashed state until a real URL is added, so nothing looks broken in the meantime.

| `data-slot` | Where | Needs |
|---|---|---|
| `ssrn` | Hero + contact | SSRN author page |
| `pub1` | Publications | Climate Action through Financial Inclusion |
| `pub2` | Publications | Macroeconomic Determinants of NEPSE |
| `pub3` | Publications | South Asia Monitor article |
| `pub4` | Publications | Sanjibani / DCGF piece |
| `repo` | Applied research | GitHub repository |
| `dashboard` | Applied research | Interactive dashboard |

Replace the `href="#"` on each with the live URL. No other change is needed.

## Run locally

```bash
git clone https://github.com/Godashish/PortfolioV-1.git
cd PortfolioV-1
python3 -m http.server 8000
```

Then open <http://localhost:8000>.

## Deploy

Push to `main`, then **Settings → Pages → Deploy from a branch → `main` / `root`**.

## Accessibility & performance

- Responsive from 320px up
- Skip link, visible focus rings, labelled landmarks
- `prefers-reduced-motion` respected
- Print stylesheet included
- No frameworks, no JS dependencies
