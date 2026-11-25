---
type: concept
status: draft
updated: 2026-11-25
last_checked: 2026-11-25
tags: [strange-calculi, discrete-calculus, finite-differences, sums]
sources: [parabola.unsw.edu.au, cs.purdue.edu]
---

# Discrete Calculus

**Hook:** What if the smallest step is 1, not "infinitely small"? You get a calculus for whole numbers, and it turns nasty sums like 1² + 2² + ... + *n*² into a one-line calculation.

## The idea

Ordinary calculus lets the step size shrink to zero. **Discrete calculus** (also called *finite calculus* or the *calculus of finite differences*) keeps the step at exactly 1.

- **The difference** replaces the derivative: **Δ*f*(*x*) = *f*(*x* + 1) − *f*(*x*)**.
- **Sums** replace integrals.
- **A discrete Fundamental Theorem:** adding up the differences telescopes, so the sum of Δ*f*(*x*) from *x* = *a* to *b* − 1 is just *f*(*b*) − *f*(*a*). Compare the [[Fundamental Theorem of Calculus]].

## The trick that makes it work

Ordinary powers behave badly: Δ*x*² = 2*x* + 1, not 2*x*. The fix is the **falling power**

> *x*⁽ⁿ⁾ = *x*(*x* − 1)(*x* − 2) ··· (*x* − *n* + 1)

which obeys **Δ*x*⁽ⁿ⁾ = *n* *x*⁽ⁿ⁻¹⁾**, exactly like the power rule. To sum *x*² from 1 to *n*: write *x*² = *x*⁽²⁾ + *x*⁽¹⁾, "integrate" each piece with the reverse power rule, plug in the endpoints, and out comes *n*(*n* + 1)(2*n* + 1)/6. No induction or guessing needed.

## Look-alikes

| Ordinary calculus | Discrete calculus |
|---|---|
| derivative *d/dx* | difference Δ |
| *x*ⁿ | falling power *x*⁽ⁿ⁾ |
| *e*ˣ (its own derivative) | 2ˣ (its own difference) |
| integration by parts | summation by parts |

## Where it shows up

- **Counting the cost of algorithms.** Gleich's tutorial opens with the number of operations in Gaussian elimination, a sum that finite calculus handles cleanly.
- **Numerical methods**, where derivatives are approximated by differences on a grid (see [[Weather Forecasting]]).
- **Competition math**, where closed forms for sums come up often.

## Go deeper (checked 2026-11-25)

- [Mathematics with a Difference](https://parabola.unsw.edu.au/sites/default/files/2024-03/vol33_no1_2.pdf), Peter G. Brown, *Parabola* 33(1), 1997 (UNSW's magazine for school students; free PDF): the gentlest introduction found, with worked sums
- [Finite Calculus: A Tutorial for Solving Nasty Sums](https://www.cs.purdue.edu/homes/dgleich/publications/Gleich%202005%20-%20finite%20calculus.pdf), David Gleich, 2005 (free PDF, 18 pages): adds summation by parts and Stirling numbers
- *Concrete Mathematics* (Graham, Knuth, and Patashnik, 1989), the standard textbook treatment, which Gleich points to for more (commercial)

## Next stop

- [[Fundamental Theorem of Calculus]]: the continuous original
- [[Fractional Calculus]]: another way to bend the rules, with derivatives of order ½
- [[Basel Problem]]: a sum that discrete tricks *can't* close, which needs π
- [[Frontiers]]
