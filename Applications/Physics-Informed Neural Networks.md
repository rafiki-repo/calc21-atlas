---
type: application
status: draft
updated: 2026-11-24
last_checked: 2026-11-24
tags: [machine-learning, pde, differential-equations, scientific-computing]
sources: [arxiv.org, neurips.cc]
---

# Physics-Informed Neural Networks

**Hook:** Most neural networks learn from examples. A physics-informed one is also graded on whether it obeys a differential equation, and calculus does the grading.

## The idea

A **physics-informed neural network (PINN)** is a network that tries to *be* the solution u(x, t) of a [[Glossary#Partial differential equation (PDE)|PDE]]. Training penalizes two things:

1. **Missing the data:** wrong values at measured points, or at the boundary and starting conditions.
2. **Breaking the equation:** plug the network into the PDE and see how far the result is from zero (the *residual*).

The derivatives in step 2 come from **automatic differentiation**, the same chain-rule machinery ([[Glossary#Automatic differentiation]]) that trains every network (see [[Backpropagation and the Chain Rule]]). So calculus appears twice: once in the equation, once in the training.

Introduced by Maziar Raissi, Paris Perdikaris, and George Em Karniadakis (preprints 2017; *Journal of Computational Physics*, 2019).

## Why people use them

- **No grid.** The equation is checked at scattered points, so awkward shapes are easier.
- **Inverse problems.** A PINN can estimate an *unknown* coefficient in the equation from sparse, noisy measurements. Classical solvers need extra machinery for that job.
- **Extensions everywhere:** domain decomposition (XPINNs), adaptive loss weights, and even a fractional version for [[Fractional Calculus|fractional derivatives]].

## The fine print

- **Training can fail.** A NeurIPS 2021 paper by Krishnapriyan and colleagues found that standard PINNs can fail even on simple convection and reaction problems with known exact solutions. The authors blame a hard-to-optimize loss, not a too-small network.
- **Usually less accurate and slower than classic solvers** for ordinary "solve this PDE" tasks, according to a 2024 review by the method's own originators. Long runs of chaotic systems are a known weak spot.
- Lots of claimed applications are preprints. Individual success stories are best read as claims.

## Next stop

- [[Backpropagation and the Chain Rule]]: the calculus that trains every network
- [[Weather Forecasting]]: where physics and machine learning already run side by side
- [[Navier-Stokes Smoothness Problem]]: the fluid equation that AI-assisted blow-up hunts target
- [[Applications]]

## Sources (checked 2026-11-24)

- [Physics-Informed Neural Networks and Extensions](https://arxiv.org/abs/2408.16806), Raissi, Perdikaris, Ahmadi, Karniadakis, arXiv review, Aug 2024
- [Characterizing possible failure modes in physics-informed neural networks](https://arxiv.org/abs/2109.01050), Krishnapriyan et al., NeurIPS 2021
