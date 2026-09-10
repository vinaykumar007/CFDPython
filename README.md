# CFD Python — Numerical Simulation Portfolio

> **A computational fluid dynamics learning portfolio built around the 12 steps to Navier–Stokes.**
>
> This repository contains Python/Jupyter implementations of progressively richer PDE models, from 1D transport equations to 2D Navier–Stokes cavity and channel flow.

[![DOI](https://jose.theoj.org/papers/10.21105/jose.00021/status.svg)](https://doi.org/10.21105/jose.00021)
[![Python](https://img.shields.io/badge/Python-3.x-blue)](https://www.python.org/)
[![NumPy](https://img.shields.io/badge/NumPy-scientific%20computing-orange)](https://numpy.org/)
[![SciPy](https://img.shields.io/badge/SciPy-numerical%20tools-blue)](https://scipy.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-notebooks-orange)](https://jupyter.org/)

## Portfolio Snapshot

| Dimension | What this repository demonstrates |
|---|---|
| **Physics** | Convection, diffusion, Burgers' equation, Laplace, Poisson, incompressible flow |
| **Mathematics** | Partial differential equations, finite differences, boundary/initial conditions |
| **Numerics** | Explicit time marching, iterative solvers, stability, numerical diffusion, convergence |
| **Scientific Python** | NumPy array operations, Matplotlib visualization, SciPy/SymPy tooling, Jupyter |
| **Simulation thinking** | Start from a governing equation → discretize → implement → visualize → inspect numerical behavior |

## Why This Repository Matters

The strongest value of this repository is not a single fluid-flow result; it is the **numerical modelling workflow**.

Each step turns a mathematical statement of physics into executable code and makes the effect of numerical choices visible. The progression provides a practical foundation for computational engineering work where model formulation, discretization, stability, accuracy, convergence, and interpretation matter as much as programming syntax.

## Governing-Equation Progression

```text
Linear / Nonlinear Convection
            ↓
          Diffusion
            ↓
      Burgers' Equation
            ↓
      2D Transport Models
            ↓
        Laplace / Poisson
            ↓
    2D Navier–Stokes Flow
       ↙              ↘
   Cavity Flow      Channel Flow
```

## Numerical Concepts Explored

### Stability

The repository explicitly explores the CFL condition and the relationship between spatial resolution, time step, and stable explicit integration.

### Numerical Diffusion

The exercises make it possible to see how discretization can alter a transported field and why numerical diffusion matters when interpreting simulated results.

### Accuracy and Convergence

Resolution and parameter changes are used to build intuition for how numerical solutions approach a more resolved representation of the underlying PDE.

### Boundary and Initial Conditions

The lessons repeatedly connect the governing equation to physically meaningful initial and boundary conditions, including Dirichlet and Neumann cases.

## Simulation Portfolio

| Step | Model | Computational focus |
|---|---|---|
| 1 | 1D linear convection | Upwind-style transport implementation and visualization |
| 2 | 1D nonlinear convection | Nonlinear transport behaviour |
| 3 | 1D diffusion | Diffusive smoothing and explicit time stepping |
| 4 | 1D Burgers' equation | Coupled nonlinear convection–diffusion |
| 5 | 2D linear convection | Extension from scalar 1D to 2D fields |
| 6 | 2D nonlinear convection | Nonlinear 2D transport |
| 7 | 2D diffusion | Two-dimensional diffusion behaviour |
| 8 | 2D Burgers' equation | Nonlinear coupled transport |
| 9 | Laplace equation | Elliptic PDE with Neumann/Dirichlet BCs |
| 10 | Poisson equation | Source-driven elliptic problem |
| 11 | 2D cavity flow | Navier–Stokes / pressure–velocity coupling workflow |
| 12 | 2D channel flow | Steady channel-flow simulation |

## Reproducing the Work

The original course is notebook-based and designed for interactive exploration.

### Environment

```bash
pip install jupyter numpy scipy sympy matplotlib
```

Launch Jupyter from the repository root:

```bash
jupyter notebook
```

Then work through the lessons in order. Change grid size, time step, physical parameters, and boundary conditions to investigate numerical behaviour rather than only reproducing the default examples.

## Portfolio Mindset

A useful way to read these notebooks is as a repeatable scientific-computing loop:

```text
Physical model
      ↓
Governing PDE
      ↓
Discretization
      ↓
Boundary / initial conditions
      ↓
Numerical implementation
      ↓
Stability / convergence checks
      ↓
Visualization
      ↓
Physical interpretation
```

This is the workflow I use as a foundation for broader computational modelling across fluid flow, subsurface engineering, geomechanics, and materials-related simulation.

## Repository Context

**CFD Python**, also known as **the 12 steps to Navier–Stokes**, is an educational module created by **Lorena A. Barba and Gilbert F. Forsyth**. The material was developed as a practical introduction to CFD through coding basic PDEs governing fluid flow. The module is presented here as part of my computational modelling portfolio and learning practice.

### Original source / citation

Barba, Lorena A., and Forsyth, Gilbert F. (2018). *CFD Python: the 12 steps to Navier-Stokes equations*. Journal of Open Source Education, 1(9), 21. https://doi.org/10.21105/jose.00021

Please cite the original work when reusing the educational material.

## Related Work

This repository fits into a broader scientific-computing portfolio:

- [Computational Geophysics](https://github.com/vinaykumar007/computational-geophysics) — geophysical processing, inversion, geomodelling, and ML workflows.
- [PyReservoir](https://github.com/vinaykumar007/pyreservoir) — Python utilities for reservoir-engineering calculations and analysis.
- [GeostatsPy Intro Course](https://github.com/vinaykumar007/GeostatsPy_Intro_Course) — spatial statistics, variograms, and kriging.
- [Computational Materials Simulation](https://github.com/vinaykumar007/vinaykumar007/tree/main/computational-materials-simulation) — an application-focused continuum thermal-diffusion case study.

## License and Attribution

The original educational content states that course content is available under **CC BY 4.0** and the code under **BSD-3-Clause**. See the upstream project and its license files for the applicable terms.

---

<p align="center"><i>From governing equations to executable simulations — one numerical step at a time.</i></p>
