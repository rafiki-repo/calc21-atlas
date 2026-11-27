---
type: puzzle
status: draft
updated: 2026-11-27
last_checked: 2026-11-27
tags: [integrals, patterns, fourier-analysis]
sources: [en.wikipedia.org, chalkdustmagazine.com, physicstoday.aip.org, 3blue1brown.com]
---

# Borwein Integrals

**Hook:** Seven integrals in a row give exactly π/2. The eighth comes out about 0.00000000002 short. It is not a rounding error.

## The pattern

Write sinc(*x*) = sin(*x*)/*x*. Now integrate products of stretched copies from 0 to ∞:

- ∫ sinc(*x*) d*x* = **π/2**
- ∫ sinc(*x*) · sinc(*x*/3) d*x* = **π/2**
- ∫ sinc(*x*) · sinc(*x*/3) · sinc(*x*/5) d*x* = **π/2**
- ... and so on, adding *x*/7, *x*/9, *x*/11, *x*/13: still **π/2** every time.
- Add sinc(*x*/15) and the answer is **π/2 − about 2.3 × 10⁻¹¹**.

The exact value at that step is a fraction times π whose top and bottom each have dozens of digits (per Wikipedia).

## Who found it

**David and Jonathan Borwein**, a father-and-son pair, published the family in 2001 ("Some remarkable properties of sinc and related integrals," *The Ramanujan Journal*). According to *Physics Today*, when numerical checks first showed the deviation, it was blamed on a **software bug**. It wasn't one.

## Why it breaks

The short answer is **1/3 + 1/5 + ... + 1/13 is less than 1, but adding 1/15 pushes the total past 1.**

The longer answer uses [[Glossary#Fourier analysis|Fourier analysis]]. Each sinc factor turns into a flat "box." Multiplying sincs means blurring the boxes into each other (convolution). Each blur spreads the shape a little wider. The value at the center stays fixed until the spreading, which is the sum of those reciprocals, finally reaches the center from the edge. Then the value dips.

- **Random walkers:** in 2019, physicists Satya Majumdar and Emmanuel Trizac recast the integrals as a random walk. In their version, the break happens when "news" from the edge reaches the origin (reported by *Physics Today*).
- **A longer streak:** if you put a factor of 2cos(*x*) in front, the pattern holds all the way to *x*/111 and fails at *x*/113, by about 10⁻¹³⁸. The reason is the same, except the threshold is 2 instead of 1.

## The lesson

Checking the first few cases is not a proof, and here even the first seven are not enough. Mathematicians often cite this family as a warning about trusting a pattern.

## Go deeper

- [3Blue1Brown: "Researchers thought this was a bug"](https://www.3blue1brown.com/lessons/borwein) (Nov 2022, video, free): an animated explanation by [[Grant Sanderson]], with a follow-up on convolutions
- [Chalkdust: "Borwein integrals"](https://chalkdustmagazine.com/features/borwein-integrals/) (Aimen Khan, Nov 2024, free): a student magazine walkthrough with the Fourier argument
- [Physics Today: "Random walkers illuminate a math problem"](https://physicstoday.aip.org/news/random-walkers-illuminate-a-math-problem) (Heather M. Hill, Sep 2019)
- [Wikipedia: Borwein integral](https://en.wikipedia.org/wiki/Borwein_integral): exact values and the general rule

## Next stop

- [[Sophomores Dream]]: the opposite surprise, a too-good-to-be-true formula that is true
- [[Basel Problem]]: another place where π turns up uninvited
- [[Feynman Integration Trick]]: one of the standard ways to get the first integral, ∫ sin(*x*)/*x* = π/2
- [[Puzzles]]
