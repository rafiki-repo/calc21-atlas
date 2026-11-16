---
type: concept
status: solid
updated: 2026-11-16
last_checked: 2026-11-16
tags: [core, integrals, derivatives]
sources: [openstax.org, mathshistory.st-andrews.ac.uk, 3blue1brown.com]
---

# Fundamental Theorem of Calculus

**Hook:** Slope and area sound like unrelated ideas. This theorem says they are two sides of one coin.

## The idea

Take a function *f* that is **continuous on [a, b]**.

- **Part 1:** Build a new function by accumulating area, *F*(*x*) = ∫ₐˣ *f*(*t*) d*t*. Then *F*′(*x*) = *f*(*x*). The rate at which the area grows is the curve's own height. Differentiating undoes accumulating.
- **Part 2:** If *F* is **any** antiderivative of *f*, then ∫ₐᵇ *f*(*x*) d*x* = *F*(*b*) − *F*(*a*). To find an area, you can skip the "infinitely many slices" and just subtract two values.

**Everyday picture:** If you know a car's speed at every moment, the distance traveled is the accumulated speed. If you know the distance traveled, the speed is its rate of change. Same facts, either direction.

## Why it matters

It turns hard summing problems into "find the antiderivative" problems, which is why integration is practical at all.

## Common trip-ups

- **The conditions matter.** The standard statement assumes continuity on the interval. Plugging into *F*(*b*) − *F*(*a*) across a point where the function blows up (such as 1/*x*² across 0) gives nonsense.
- **Antiderivatives are not unique.** Add any constant and it still works. The constant cancels in Part 2.

## Who found it

Isaac Barrow came close with his "differential triangle" but never stated the theorem explicitly. Newton and Leibniz each stated and used it in the late 1600s. See [[Newton vs Leibniz]].

## Go deeper

- [OpenStax Calculus Vol. 1, §5.3](https://openstax.org/books/calculus-volume-1/pages/5-3-the-fundamental-theorem-of-calculus): both parts, with proofs and worked examples (free)
- [The Essence of Calculus, Ch. 1](https://www.3blue1brown.com/lessons/essence-of-calculus), 3Blue1Brown: reaches the theorem visually, starting from the area of a circle (free)

## Next stop

- [[Newton vs Leibniz]]: the two people who each saw this connection
- [[Lean Companion to Analysis I]]: see this theorem proved so a computer can check every step
- [[Feynman Integration Trick]]: another way to play derivatives against integrals
- [[Glossary#Antiderivative]]
