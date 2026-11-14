---
type: open-problem
status: draft
updated: 2026-11-14
last_checked: 2026-11-14
aliases: ["Hilbert's sixth problem"]
tags: [pde, mathematical-physics, kinetic-theory]
sources: [arxiv.org/abs/2503.01800, arxiv.org/abs/2408.07818, scientificamerican.com, simonsfoundation.org]
---

# Hilbert's Sixth Problem

**Hook:** Physicists describe air three ways: as colliding particles, as a statistical cloud, and as a smooth fluid. Can a mathematician prove these three pictures are the same story told at different zoom levels?

## The question

In 1900 David Hilbert asked for physics to be put on axiomatic footing. One concrete piece: **derive the equations of fluid motion from Newton's laws for individual particles**, passing through Boltzmann's kinetic theory. Three scales:

1. **Microscopic:** billiard-ball particles obeying Newton's laws
2. **Mesoscopic:** the **Boltzmann equation** (1872), describing a "typical" particle statistically
3. **Macroscopic:** the **Euler** and **Navier-Stokes** equations for a continuous fluid

Each step is a [[Glossary#Limit|limit]]: more particles, smaller particles, longer times.

## Status

- **Step 1 → 2, short times:** Lanford (1975) derived Boltzmann from particles, but only for a short time window.
- **Step 1 → 2, long times:** Yu Deng, Zaher Hani, and Xiao Ma, arXiv 2408.07818 (2024), for as long as the Boltzmann solution exists.
- **All the way to fluids:** the same authors, arXiv 2503.01800 (March 2025), **claim** to derive the compressible Euler and incompressible Navier-Stokes-Fourier equations from hard-sphere dynamics. It is a **preprint** (no journal reference on arXiv as of last check); Scientific American framed the result as holding "assuming the proof is correct." The broader program is cited in [[Yu Deng]]'s 2026 Fields Medal.
- Hilbert's sixth problem as a whole (axiomatizing physics) is broad and not something one paper "solves."

## Why it connects to calculus

It is a question about **when one family of [[Glossary#Differential equation|differential equations]] is the limit of another**. Not to be confused with the [[Navier-Stokes Smoothness Problem]]: that one asks whether the fluid equations' solutions stay smooth, while this one asks where the equations come from.

## Next stop

- [[Yu Deng]]
- [[Navier-Stokes Smoothness Problem]]
- [[Research Watch]]
- [[Open Problems]]
