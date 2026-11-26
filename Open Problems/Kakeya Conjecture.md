---
type: open-problem
status: draft
updated: 2026-11-26
last_checked: 2026-11-26
tags: [harmonic-analysis, geometric-measure-theory, fourier-analysis]
sources: [arxiv.org/abs/2502.17655, arxiv.org/abs/2308.08819, plus.maths.org, math.ubc.ca, simonsfoundation.org, claymath.org]
---

# Kakeya Conjecture

**Hook:** How little room do you need to spin a needle so it points in every direction? The answer is "almost none," and that turns out to be a problem.

## The question

- **1917:** Sōichi Kakeya asks for the smallest region in which a needle can be turned all the way around.
- **Besicovitch's surprise:** in the plane, such regions can have **area as small as you like**. Sets containing a unit segment in every direction (*Kakeya sets*) can have zero area.
- **The modern conjecture:** even so, these sets can't be *thin* in the sense of **dimension**. A Kakeya set in n-dimensional space should have full [[Glossary#Hausdorff dimension|Hausdorff dimension]] n. Small volume, yes; lower-dimensional, no.

## Status

| Dimension | Status |
|---|---|
| 2 (the plane) | **Proved** (Davies, 1971) |
| 3 | **Proof posted (preprint).** Hong Wang and Joshua Zahl, arXiv 2502.17655 (February 2025, 127 pages). The result is named in the citation for Wang's 2026 Fields Medal; no journal reference is listed on arXiv as of last check. |
| 4 and up | **Open** |

The 3D proof built on a 2022 Wang–Zahl paper on "sticky" Kakeya sets, which followed a program set out by Katz and [[Terence Tao]], and on earlier work by Łaba, Katz, Tao, Shmerkin, Pramanik, Yang, and Zahl.

**A cousin, settled first.** The **Furstenberg set conjecture** asks a similar question about how thin tubes can overlap in the plane. Kevin Ren and Hong Wang posted a proof in 2023 ([arXiv 2308.08819](https://arxiv.org/abs/2308.08819), no journal reference listed as of 2026-11-26). In April 2026 the Clay Research Award went jointly to Tuomas Orponen, Pablo Shmerkin, Wang, and Zahl for the line of work behind both results; Clay notes that Ren "also made a substantial contribution" ([Clay announcement](https://www.claymath.org/news/2026-clay-research-awards/)).

## Why it connects to calculus

Kakeya sits at the base of a **tower of conjectures in [[Glossary#Fourier analysis|Fourier analysis]]** (restriction, local smoothing for wave equations). Those are questions about how waves add up, which is integration doing the heavy lifting. Wang told *Plus*: "If you disprove the Kakeya conjecture, then you disprove the whole tower of conjectures."

## Go deeper

- [*Plus* explainer with Hong Wang](https://plus.maths.org/icm-2026-fm-2): needles, fractals, and Hausdorff dimension without equations
- [The preprint](https://arxiv.org/abs/2502.17655), for the brave

## Next stop

- [[Hong Wang]]: who proved the 3D case
- [[Jacobian Conjecture]]: another simple-to-state problem, this one disproved in 3D in 2026
- [[Moving Sofa Problem]]: the furniture version of "how much room do you need to turn?"
- [[Research Watch]]
- [[Open Problems]]
