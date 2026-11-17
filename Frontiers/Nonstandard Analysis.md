---
type: concept
status: draft
updated: 2026-11-17
last_checked: 2026-11-17
tags: [strange-calculi, infinitesimals, logic, history]
sources: [plato.stanford.edu, people.math.wisc.edu]
---

# Nonstandard Analysis

**Hook:** Newton and Leibniz calculated with infinitely small numbers. A bishop mocked these as "ghosts of departed quantities," and they were dropped for two centuries. In the 1960s a logician made them rigorous.

## The story in three steps

1. **The founders' shortcut.** Early calculus used **[[Glossary#Infinitesimal|infinitesimals]]**: quantities that are not zero but are smaller than any positive number. They worked, but nobody could say exactly what they were.
2. **The objection.** In *The Analyst* (1734), George Berkeley pointed out the inconsistency. A tiny increment is treated as nonzero so you can divide by it, then set to zero so it disappears. He asked whether these were "the ghosts of departed quantities." The 19th century settled things with **limits**, which is how calculus is usually taught today.
3. **The comeback.** In the **1960s, Abraham Robinson** used mathematical logic to build an extended number system. It has genuine infinitesimals and infinitely large numbers, and the usual rules of arithmetic still hold. This is **nonstandard analysis**. It proves the same theorems as standard calculus, and it gives Leibniz's intuition a sound footing.

## What it looks like

The derivative of *x*² becomes nearly literal. Compute ((*x* + *dx*)² − *x*²)/*dx* = 2*x* + *dx* for an infinitesimal *dx*. Then take the **standard part**, the ordinary real number it is infinitely close to: 2*x*. There is no limit to evaluate.

## A cousin

**Smooth infinitesimal analysis** (from F. W. Lawvere's ideas in the 1970s) takes another route. It uses infinitesimals that are not zero but whose square *is* zero, and in it every function is smooth. It relies on a different logic and is mostly of interest to specialists.

## Go deeper

- [Elementary Calculus: An Infinitesimal Approach](https://people.math.wisc.edu/~hkeisler/calc.html), H. Jerome Keisler. A full first-year textbook built on Robinson's infinitesimals (1976; 3rd edition Dover 2012). The online edition is free under CC BY-NC-SA, and the page notes a June 2026 revision.
- [Continuity and Infinitesimals](https://plato.stanford.edu/entries/continuity/), *Stanford Encyclopedia of Philosophy* (revised 2022). The long history, from Zeno through Berkeley to Robinson and Lawvere. Free, and a long read.

## Next stop

- [[Newton vs Leibniz]]: the infinitesimal's original champions
- [[Fundamental Theorem of Calculus]]: what both approaches end up proving
- [[Proof Assistants and Lean]]: another case of logicians shoring up calculus
- [[Frontiers]]
