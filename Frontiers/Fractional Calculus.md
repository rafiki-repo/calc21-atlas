---
type: concept
status: draft
updated: 2026-11-17
last_checked: 2026-11-17
tags: [strange-calculi, fractional-calculus, derivatives]
sources: [mathpages.com, chalkdustmagazine.com, blog.wolfram.com]
---

# Fractional Calculus

**Hook:** You can take a first derivative and a second derivative. In 1695 L'Hôpital asked Leibniz about a *half* derivative. The answer turned out to be yes, with some fine print.

## The idea

A **half derivative** is an operation that, done twice, gives the ordinary derivative. Fractional calculus extends derivatives and integrals to orders like ½, 9¾, or even negative numbers.

The usual route goes through integrals first:

1. **Cauchy's formula** writes "integrate *n* times" as a single integral with (*n* − 1)! in it.
2. Replace the factorial with the **Gamma function** Γ, which is defined for non-whole numbers too. That gives a fractional integral of any order.
3. A **fractional derivative** is then a fractional integral combined with an ordinary derivative.

Do step 3 in one order and you get the **Riemann–Liouville** derivative. Do it in the other order and you get the **Caputo** derivative.

## A taste

With lower limit 0, the Riemann–Liouville half derivative of *x* is **2√(*x*/π)**. Take the half derivative again and you get 1, the ordinary derivative of *x*. Odd as it looks, π appears.

## The fine print (the "paradox")

Leibniz's reply to L'Hôpital, as Mathpages quotes it: it "leads to a paradox, from which one day useful consequences will be drawn." Two features cause that:

- **No single answer.** Riemann–Liouville and Caputo can disagree. For example, Caputo gives 0 for the derivative of a constant and Riemann–Liouville does not.
- **Memory.** A fractional derivative depends on the function's values all the way back to a chosen starting point, not just near one point. Change the starting point and the answer changes.

That memory is the useful consequence. It is why fractional derivatives are used to model materials and systems whose past shapes their present.

## Where it shows up

- **Damping in viscoelastic materials** (things that behave partly like a solid and partly like a liquid)
- **Sound travelling through biological tissue**
- **Control theory and signal processing**

Sources: Chalkdust and the Wolfram blog (below).

## Go deeper

- [Fractional calculus: the calculus of witchcraft and wizardry](https://chalkdustmagazine.com/features/fractional-calculus/), Rafael Prieto Curiel, *Chalkdust* (2016). Readable walk from Cauchy's formula to Caputo vs Riemann–Liouville. Free.
- [Fractional Calculus](https://www.mathpages.com/home/kmath616/kmath616.htm), Mathpages. Sets out the 1695 question and several ways to answer it. Free.
- [Fractional Calculus in Wolfram Language 13.1](https://blog.wolfram.com/2022/08/12/fractional-calculus-in-wolfram-language-13-1/), Wolfram blog (2022). Worked examples with plots, from a commercial software vendor. Free to read.

## Next stop

- [[Stochastic Calculus]]: another calculus built for something ordinary derivatives can't handle
- [[Newton vs Leibniz]]: Leibniz again, the man who couldn't leave a notation alone
- [[Glossary#Derivative]]
- [[Frontiers]]
