---
type: application
status: draft
updated: 2026-11-16
last_checked: 2026-11-16
tags: [biology, epidemiology, differential-equations]
sources: [plus.maths.org]
---

# SIR Epidemic Model

**Hook:** Three letters, three differential equations, and a 1927 result that explains why an epidemic can burn out before everyone catches it.

## The idea

Split a population into three groups and track how people flow between them:

- **S**usceptible: can catch it
- **I**nfectious: has it and can pass it on
- **R**ecovered (or removed): no longer part of the spread

In the simplest version (fixed population, no births or deaths), the rates of change are:

$$\frac{dS}{dt} = -\beta SI,\qquad \frac{dI}{dt} = \beta SI - gI,\qquad \frac{dR}{dt} = gI$$

Here *β* is the contact rate and 1/*g* is how long someone stays infectious. New infections need **both** a susceptible and an infectious person, hence the *SI* product.

## What the calculus tells you

- **A threshold.** The **basic reproduction number** *R₀* = *β*/*g* is the average number of people one case infects in a fully susceptible population. If *R₀* > 1, cases grow at first. If *R₀* < 1, the outbreak fizzles.
- **Not everyone gets it.** W. O. Kermack and A. G. McKendrick (1927) showed that the long-run fraction who escape infection, *S∞*, satisfies *S∞* = exp[(*S∞* − 1)*R₀*]. That equation has no closed-form solution, but numerically *R₀* = 2 leaves about **20%** untouched and *R₀* = 5 about **0.7%**.
- **Herd immunity.** Adding births and deaths gives a long-term balance with susceptible fraction 1/*R₀*. So vaccinating a fraction 1 − 1/*R₀* is enough to stop sustained spread. Not everyone needs to be vaccinated.

## The fine print

Real epidemics break the model's assumptions: people mix unevenly, immunity can wane, and behavior changes. Working epidemiologists use many extended versions (SEIR, age-structured models, networks). SIR is the skeleton they build on.

## Go deeper

- [The mathematics of diseases](https://plus.maths.org/content/mathematics-diseases), Matt Keeling, *Plus* magazine (2001): the equations, *R₀*, final size, and vaccination thresholds, in plain language. Free.

## Next stop

- [[Glossary#Differential equation]]
- [[Weather Forecasting]]: another case of calculus predicting the future, step by step
- [[Applications]]
