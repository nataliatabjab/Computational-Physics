
# PHY407 — Computational Physics

This repository contains my assignments and formal lab work for **PHY407 (Computational Physics)**. It focuses on
practical numerical methods used across physics: iterative solvers for linear systems, Monte‑Carlo integration,
finite‑difference schemes for ODEs/PDEs, spectral analysis, and data fitting.

## Contents

```
A1/   # Iterative methods, model fitting, convergence analysis
A2/   # Harmonic oscillator discretisation, Monte-Carlo integration
A3/   # Fourier analysis, filtering, signal reconstruction
A4/   # PDE solvers: heat, shallow-water, Burgers' equations
A5/   # Capstone: Laplace's equation, streamlines, shallow-water, Burgers'
Labs/ # Formal lab reports (PDFs) and figures
```

> Tip: keep large data/figures in a `data/` or `figures/` folder with a short README explaining provenance.

## How to run

1. Create a fresh environment (conda or venv) and install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
   If there is no `requirements.txt`, the usual baseline is:
   ```bash
   pip install numpy scipy matplotlib jupyter
   ```

2. Open notebooks or run scripts inside each assignment folder, e.g.:
   ```bash
   python A4/heat_equation.py
   jupyter lab
   ```

## Highlights

- **Laplace’s equation (Gauss–Seidel + over‑relaxation)**: solved on a square grid; compared convergence with and
  without over‑relaxation; computed **electric‑field streamlines** from the potential.
- **Shallow‑water equations (FTCS)**: implemented a finite‑difference scheme, explored stability vs. grid/time step,
  and visualised wave propagation.
- **Burgers’ equation (leapfrog)**: simulated nonlinear steepening and observed numerical oscillations/dispersion.
- Earlier work: **harmonic oscillator eigenmodes**, **Monte‑Carlo integration**, and **DFT‑based signal processing**.

## Reproducibility

- Set random seeds where applicable.
- Save figures into `figures/` with informative filenames.
- Include a small `Makefile` or `run.sh` for common experiment workflows (optional).

## License

Educational use only unless otherwise stated.
