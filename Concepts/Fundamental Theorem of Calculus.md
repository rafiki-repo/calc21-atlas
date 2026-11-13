---
type: concept
status: draft
updated: 2026-11-13
tags: [core, integrals, derivatives]
sources: unverified-seed
---

# Fundamental Theorem of Calculus

**Hook:** Slope and area sound like unrelated ideas. This theorem says they are two sides of one coin.

## The idea

- **Part 1:** If you build a function by accumulating the area under a curve, then the *rate* at which that area grows is the curve's own height. Differentiating undoes accumulating.
- **Part 2:** To find the area under a curve between two points, find any function whose derivative is the curve, then subtract its values at the endpoints. You skip the "infinitely many slices" step.

**Everyday picture:** If you know a car's speed at every moment, the distance traveled is the accumulated speed. If you know the distance traveled, the speed is its rate of change. Same facts, either direction.

## Why it matters

It turns hard summing problems into "find the antiderivative" problems, which is why integration is practical at all.

## Common trip-ups

- The theorem needs conditions (such as continuity on the interval); it is not a license to ignore them.
- "Antiderivative" is not unique: add any constant and it still works. The constant cancels in Part 2.

## Next stop

- [[Newton vs Leibniz]] — the two people who each saw this connection
- [[Basel Problem]] — a different kind of "adding up" puzzle
- [[Glossary]] — derivative, integral, antiderivative
