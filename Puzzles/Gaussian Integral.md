---
type: puzzle
status: draft
updated: 2026-11-28
last_checked: 2026-11-28
tags: [integrals, multivariable, probability, history]
sources: [kconrad.math.uconn.edu]
---

# Gaussian Integral

**Hook:** The bell curve *e*^(−*x*²) has no antiderivative you can write down. Yet the total area under it is exactly √π, and the slickest proof works by making the problem *harder*: going to two dimensions.

## The puzzle

$$\int_{-\infty}^{\infty} e^{-x^2}\,dx = \sqrt{\pi}$$

The usual tools fail: no substitution or integration by parts gives an antiderivative of *e*^(−*x*²) in terms of familiar functions. So where does π, a circle number, come from?

## The famous trick (try it first)

1. Call the integral *I*. Write *I*² as the product of two copies, one in *x* and one in *y*.
2. That product is a double integral of *e*^(−(*x*²+*y*²)) over the whole plane.
3. *x*² + *y*² is *r*² in polar coordinates. That's where the circle sneaks in.

<details><summary>Finish the calculation</summary>

In polar coordinates the area element is *r* d*r* dθ, and that extra *r* is exactly what makes the integral doable: ∫₀^∞ *r e*^(−*r*²) d*r* = 1/2. Multiply by the 2π from θ to get *I*² = π, so *I* = √π.
</details>

Keith Conrad's note credits this widely known proof to **Poisson**. It was not the first: **Laplace** found the value in 1774 by a different route.

## Why anyone cares

It is the normalizing constant of the **normal distribution**, the bell curve of statistics. Conrad traces three routes to that curve: De Moivre's 1733 approximation of coin-flip counts, Gauss's 1809 "error curve" from tracking the asteroid Ceres, and Laplace's 1812 first version of the central limit theorem.

## Go deeper

- [The Gaussian Integral](https://kconrad.math.uconn.edu/blurbs/analysis/gaussianintegral.pdf), Keith Conrad (UConn), free PDF: **eleven** different proofs, including polar coordinates, [[Feynman Integration Trick|differentiating under the integral sign]], residues, and Fourier transforms, plus a short history. Mostly calculus-level, with a few advanced proofs.

## Next stop

- [[Feynman Integration Trick]]: Conrad's third and fourth proofs use it
- [[Basel Problem]]: another place π turns up where nobody ordered it
- [[Diffusion Models]]: Gaussian noise, put to work in AI image generators
- [[Puzzles]]
