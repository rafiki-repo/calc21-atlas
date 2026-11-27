---
type: puzzle
status: draft
updated: 2026-11-27
last_checked: 2026-11-27
tags: [integrals, series, history]
sources: [mathworld.wolfram.com, en.wikipedia.org]
---

# Sophomore's Dream

**Hook:** An integral that turns into a sum that looks like a typo. It is true, and Johann Bernoulli proved it in 1697.

## The formulas

$$\int_0^1 x^{-x}\,dx = \sum_{n=1}^{\infty} \frac{1}{n^n} = 1 + \frac{1}{2^2} + \frac{1}{3^3} + \frac{1}{4^4} + \cdots \approx 1.29129$$

$$\int_0^1 x^{x}\,dx = \sum_{n=1}^{\infty} \frac{(-1)^{n+1}}{n^n} = 1 - \frac{1}{2^2} + \frac{1}{3^3} - \cdots \approx 0.78343$$

## Why the name

It is a joke. The "**freshman's dream**" is the classic mistake (*a* + *b*)ⁿ = *a*ⁿ + *b*ⁿ, which is false. The "sophomore's dream" looks just as naive, since "x to the x" seems to turn into "n to the n", but this one is true. The name appears in Borwein, Bailey, and Girgensohn's *Experimentation in Mathematics* (2004), per Wikipedia and MathWorld.

## How it works (no spoilers beyond the first step)

1. Rewrite *x*ˣ as *e*^(*x* ln *x*).
2. Expand that as a [[Glossary#Power series|power series]] and integrate it term by term.
3. Each term is an integral of the form *x*ⁿ(ln *x*)ⁿ, which integration by parts handles.

<details><summary>What each term gives</summary>

Each term contributes ±1/(*n*+1)^(*n*+1), and adding them up gives the series. Bernoulli did this with repeated integration by parts, since the gamma function, today's shortcut, did not exist yet (Wikipedia, citing William Dunham's *The Calculus Gallery*, ch. 3).
</details>

## Go deeper

- [MathWorld: Sophomore's Dream](https://mathworld.wolfram.com/SophomoresDream.html): both identities and the term-by-term proof
- [Wikipedia: Sophomore's dream](https://en.wikipedia.org/wiki/Sophomore%27s_dream): history and the full calculation

## Next stop

- [[Borwein Integrals]]: the reverse surprise, a pattern that looks true and is false
- [[Basel Problem]]: another sum with a surprising closed form
- [[MIT Integration Bee]]: where tricks like step 1 are worth seconds
- [[Puzzles]]
