# ANCHOR project page

Project website for **ANCHOR: Safe Diffusion Planning via Analytic Approximation of Doob’s h-function**.

**Website:** https://doobdiffusion.github.io/ANCHOR/

A responsive, dependency-free static research page, with a Nerfies-inspired layout, original manuscript figures, accessible experiment tabs, and benchmark tables.

## Local preview

```bash
python -m http.server 8000
```

Open http://localhost:8000. No build step or JavaScript package install is required.

## Hosting

GitHub Pages publishes the root of the `main` branch. `.nojekyll` keeps the site static. Push changes to `main` to update the page.

## Editing

- `index.html`: paper summary, resource links, experiment descriptions, and result tables.
- `assets/css/style.css`: layout, typography, and responsive styles.
- `assets/js/main.js`: mouse and keyboard controls for experiment tabs.
- `assets/figures/`: optimized WebP exports of manuscript figures.

The page is intentionally anonymous. Do not add author names, affiliations, or links to the GitHub repository. Code, Paper, and Dataset are displayed in separate icon boxes, each marked “Coming soon”.

## Content provenance

Source: `new_paper/ICLR/` from the ANCHOR research workspace.

- Title and overview: `iclr_main.tex`, `sections/01_introduction.tex`, `sections/03_method.tex`.
- Main Maze results: `sections/tables/maze2d_medium.tex` (combined Medium/Hard table). The Hard row uses the constant-weight variant reported in the main comparison, not the inverse-std variant in the separate Hard table.
- Robotics results: `sections/tables/robotics_main.tex`.
- Figure exports: `figures/anchor_conference_figure.pdf`, `2dgaussian_comparison_2x2_fullHessian.pdf`, `sequential_comparison_2x2_inverse_std.pdf`, `maze_datasets_styled.pdf`, and the method-comparison / robotics PNGs.

The overview is a manuscript-based summary, not a verbatim abstract: the draft abstract’s original Maze2D claims differ from the newer multimodal Maze benchmarks. The page uses the detailed experimental tables and distinguishes theoretical continuous-time safety, measured planned safety, and measured execution safety. No venue or acceptance status is claimed.

Design inspiration: [Nerfies](https://nerfies.github.io/). Site implementation is original; no Nerfies source code or analytics are bundled. Research figures belong to their respective authors.
