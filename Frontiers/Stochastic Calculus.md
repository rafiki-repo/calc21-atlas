---
type: concept
status: draft
updated: 2026-11-17
last_checked: 2026-11-17
tags: [strange-calculi, stochastic-calculus, probability, finance]
sources: [mathunion.org, ocw.mit.edu]
---

# Stochastic Calculus

**Hook:** Ordinary calculus needs curves smooth enough to have a slope. A pollen grain jostled by water molecules traces a path with no slope anywhere. Kiyosi Itô built a calculus for it anyway.

## The problem

**[[Glossary#Brownian motion|Brownian motion]]** is the jittery random path of a small particle being hit by invisible molecules. As a mathematical object it is strange:

- It is **nowhere differentiable**, so there is no slope at any point.
- Over any stretch of time its path has **infinite length**.
- Its typical distance from the start grows like the **square root of time**, not like time itself.

So if a quantity is pushed by both ordinary forces and random kicks, the usual derivative breaks down.

## Itô's fix

Starting in the 1940s, **Kiyosi Itô** (1915–2008) developed **stochastic analysis**: a way to define integrals against random paths and to write **stochastic differential equations** (SDEs). An SDE is a differential equation that includes a noise term.

The key change is to the chain rule. Over a short time *dt*, a random kick is about the size of √*dt*. Its square is about *dt*, which is too big to throw away. **Itô's formula** is the chain rule with an extra second-derivative term that captures this. Shorthand: (*dB*)² = *dt*.

## Why it matters

- **Finance:** option pricing grew out of Itô's ideas. See [[Black-Scholes Equation]].
- **Biology:** random changes in population size and gene frequencies, for example the chance that a gene takes over a population.
- **Physics and engineering:** noisy signals, and controlling systems that are pushed around at random.

In 2006 Itô became the first winner of the **Gauss Prize** for applications of mathematics, "for laying the foundations of the theory of Stochastic Differential Equations and Stochastic Analysis." In his thank-you remarks he said that, since he worked in pure mathematics, the award was unexpected.

## Go deeper

- [MIT 18.642, Week 14: Stochastic calculus](https://ocw.mit.edu/courses/18-642-topics-in-mathematics-with-applications-in-finance-fall-2024/pages/week-14/), MIT OpenCourseWare (Fall 2024). Two lectures on Itô integrals, Itô's formula, and SDEs, ending with the Black-Scholes equation. Video and slides. Free (CC BY-NC-SA). Assumes probability and multivariable calculus.
- [Gauss Prize 2006](https://www.mathunion.org/imu-awards/carl-friedrich-gauss-prize/carl-friedrich-gauss-prize-applications-mathematics-2006), International Mathematical Union. Citation and press releases. The [popular press release](https://www.maths.tcd.ie/EMIS/mirror/IMU/medals/2006/gauss_popular_eng.pdf) (mirror) explains Itô's work with no equations.

## Next stop

- [[Black-Scholes Equation]]: the most famous application
- [[Fractional Calculus]]: a different way of stretching the derivative
- [[SIR Epidemic Model]]: a deterministic model that stochastic versions add noise to
- [[Frontiers]]
