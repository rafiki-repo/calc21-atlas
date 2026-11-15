---
type: puzzle
status: draft
updated: 2026-11-15
last_checked: 2026-11-15
tags: [integration, techniques, feynman, leibniz]
sources: [kconrad.math.uconn.edu]
---

# Feynman Integration Trick

**Hook:** Stuck on an integral? Add a new variable to it, differentiate with respect to that variable, and sometimes the problem gets easier. Richard Feynman built his reputation on this, though Leibniz knew it in 1697.

## The idea

Formally, it is **differentiation under the integral sign** (the Leibniz integral rule). If an integral depends on a parameter *t*, then under mild conditions:

$$\frac{d}{dt}\int_a^b f(x,t)\,dx = \int_a^b \frac{\partial f}{\partial t}(x,t)\,dx$$

The recipe:
1. Insert a parameter into a hard integral, so that it becomes a function I(t).
2. Differentiate under the integral sign. The new integral is often easy.
3. Integrate back in *t*, and fix the constant using a value of *t* where I(t) is obvious.

Classic targets: the Gaussian integral, and ∫₀^∞ (sin x)/x dx = π/2 (via a damped version with e^(−tx) inserted).

## The story

In *Surely You're Joking, Mr. Feynman!*, Feynman says he learned the method from Woods' *Advanced Calculus*, a book his high-school physics teacher gave him. He wrote that it was rarely emphasized at universities. When colleagues at MIT or Princeton got stuck on an integral, he would "come along and try differentiating under the integral sign, and often it worked." His "box of tools," he said, was simply different from everyone else's.

## The fine print

Swapping a derivative and an integral is not always allowed. The rule needs the integrand and its partial derivative to behave well (continuity, or domination for improper integrals). When those conditions fail, the method can give wrong answers. Keith Conrad's notes have a section of counterexamples.

## Go deeper

- [Differentiating Under the Integral Sign](https://kconrad.math.uconn.edu/blurbs/analysis/diffunderint.pdf), Keith Conrad (UConn), free PDF with many worked examples and the Feynman quote

## Next stop

- [[MIT Integration Bee]]: where tricks like this win trophies
- [[Fundamental Theorem of Calculus]]: the derivative-integral relationship this trick exploits
- [[Glossary#Partial derivative]]
- [[Puzzles]]
