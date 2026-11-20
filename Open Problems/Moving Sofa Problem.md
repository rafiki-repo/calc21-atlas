---
type: open-problem
status: draft
updated: 2026-11-20
last_checked: 2026-11-20
tags: [geometry, optimization, area, greens-theorem]
sources: [arxiv.org, quantamagazine.org, horizon.kias.re.kr, thestar.com.my]
---

# Moving Sofa Problem

**Hook:** What is the biggest sofa you can carry around a corner? Mathematicians chipped away at it for almost 60 years. A 119-page proof posted in 2024 says the answer is a strange 18-piece shape from 1992. It is **still in peer review**.

## The question

A hallway is 1 unit wide and turns a right angle. What is the **largest area** of a flat, rigid shape that can be slid and rotated around the corner? Leo Moser posed it in **1966**.

## The race (lower and upper bounds)

| Year | Who | What |
|---|---|---|
| 1968 | John Hammersley | A "telephone" shape of area **π/2 + 2/π ≈ 2.2074**, and proof that no sofa can beat **2√2 ≈ 2.83** |
| 1992 | Joseph Gerver | A shape built from **18 curve sections**, area **≈ 2.2195**. Widely suspected to be the best, with no proof |
| 2017 | Yoav Kallus and Dan Romik | A computer-assisted upper bound that narrowed the gap but did not close it |
| 2024 | **Jineon Baek** | Claims a proof that Gerver's sofa **is** optimal |

## Status (checked 2026-11-20)

- **Proof claimed, not yet refereed.** Baek posted *Optimality of Gerver's Sofa* to arXiv on Nov 29, 2024 (119 pages). *Quanta* (Feb 2025) reported it was being peer reviewed. *The Korea Herald* reported in Jan 2026 that it was under review at the *Annals of Mathematics*. A KIAS interview (Jun 2026) still describes it as not yet peer reviewed, with "a broad consensus that his argument is correct."
- **No computers.** Baek first tried a computer-assisted proof, then found an argument that did not need one. That surprised people who expected the final step to be computational.
- *Scientific American* named it one of its top 10 math breakthroughs of 2025, according to the same report.

## Why it connects to calculus

This is an **optimization problem**, but the thing being optimized is a whole shape rather than a number.

- Baek narrows the candidates to sofas with a few natural properties (they rotate a full 90°, they are "balanced," and so on).
- He then builds a stand-in function **Q** that is always at least the true area and equals it exactly for Gerver's sofa. Q is **concave and quadratic**, so a local maximum is a global one. Showing Gerver's sofa is a local maximum of Q finishes the proof.
- The area carved out by the hallway's inner corner is written as a **line integral using Green's theorem**, the multivariable cousin of the [[Fundamental Theorem of Calculus]].

## Sources

- [Optimality of Gerver's Sofa](https://arxiv.org/abs/2411.19826), J. Baek, arXiv preprint, Nov 2024
- [The Largest Sofa You Can Move Around a Corner](https://www.quantamagazine.org/the-largest-sofa-you-can-move-around-a-corner-20250214/), *Quanta Magazine*, Feb 14, 2025 (history, quotes from Gerver and from Baek's adviser Michael Zieve)
- [South Korean mathematician solves 60-year-old maths puzzle](https://www.thestar.com.my/aseanplus/aseanplus-news/2026/01/05/south-korean-mathematician-solves-60-year-old-maths-puzzle), *The Korea Herald*/ANN via *The Star*, Jan 5, 2026 (review status)
- [An Interview with Jineon Baek](https://horizon.kias.re.kr/33559/), KIAS *Horizon*, Jun 30, 2026 (how the proof works)

## Next stop

- [[Kakeya Conjecture]]: another "how much room do you need to turn?" problem
- [[Fundamental Theorem of Calculus]]: the one-dimensional version of the Green's theorem trick
- [[Irrationality of Zeta Values]]: another 2020s result still waiting on referees
- [[Open Problems]]
