---
type: puzzle
status: draft
updated: 2026-11-27
last_checked: 2026-11-27
tags: [competition, proofs, ai]
sources: [kskedlaya.org, news.mit.edu, matharena.ai, math.gatech.edu, math.toronto.edu]
---

# Putnam Competition

**Hook:** Six hours, twelve problems, and every answer must be a proof. This is North America's best-known undergraduate math contest, and in 2025 AI took it too.

## What it is

The **William Lowell Putnam Mathematical Competition** is run by the Mathematical Association of America (MAA). It is held on the first Saturday of December for college students in the US and Canada. Through 2025 the exam had two 3-hour sessions (A and B) of six problems each. Each answer is graded as a **full proof**, out of 10 points. Calculus and real analysis are regular ingredients, alongside algebra, number theory, and combinatorics. Top individuals are named **Putnam Fellows**. More than 4,300 students took the 2025 exam, and the median score was 2 out of 120 (per Virginia Tech's math department).

## New in 2026: four short sessions

The **87th Putnam is on Saturday, Dec 5, 2026**, and the format changes. University pages at Georgia Tech and Toronto (checked 2026-11-27) say there are now **four 90-minute sessions of three problems each**, replacing the two 3-hour sessions. Georgia Tech reports that the MAA says the changes were made "in anticipation of challenges posed by AI to competition security." The MAA's own page could not be fetched (403), so the wording comes from those university pages.

## The 86th Putnam (Dec 6, 2025)

- **Top team:** MIT, for the sixth year in a row, followed by Chicago, Harvard, Stanford, and Caltech (per MAA and MIT News).
- **Putnam Fellows:** MIT News reports four of the five were from MIT: Cheng Jiang, Luke Robitaille, Chunji Wang, and Zixiang Zhou. MIT's **Jessica Wan** won the Elizabeth Lowell Putnam Prize, awarded to a top-scoring woman.

## The AI angle

**MathArena** (an AI evaluation group) submitted anonymized solutions from six AI systems, and the official Putnam graders scored them with the usual rubrics. According to MathArena, the best system, a DeepSeek-based agent, scored **103/120**. That would place it in the top 3 of 4,329 human participants and above the Fellow cutoff. The caveats, also from MathArena: graders found many AI solutions verbose, the evaluation was partly funded by a Google DeepMind grant, and graders knew which solutions came from AI. See [[Calculus and AI]].

## Try one: 2025, problem A2

> Find the largest *a* and the smallest *b* such that *a*·*x*(π − *x*) ≤ sin *x* ≤ *b*·*x*(π − *x*) for every *x* between 0 and π.

In plain words: squeeze the sine arch between two upside-down parabolas. It is a first-semester calculus problem in disguise, since the solution in Kedlaya's archive studies the ratio sin *x* / (*x*(π − *x*)) and its derivative.

<details><summary>Answer</summary>

*a* = 1/π and *b* = 4/π². The ratio climbs from 1/π (its limit at *x* = 0) to 4/π² at the midpoint *x* = π/2. Full solutions: [2025 solutions PDF](https://kskedlaya.org/putnam-archive/2025s.pdf) (by Manjul Bhargava, Kiran Kedlaya, and Lenny Ng; unofficial).
</details>

## Play along

- [Kiran Kedlaya's Putnam archive](https://kskedlaya.org/putnam-archive/): problems from 1985 to 2025, with solutions for most years (unofficial, free)

## Next stop

- [[MIT Integration Bee]]: the faster, flashier cousin
- [[Calculus and AI]]: what "AI aced an exam" does and doesn't mean
- [[Basel Problem]]: a 17th-century Putnam-style puzzle
- [[Puzzles]]
