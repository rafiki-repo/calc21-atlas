---
type: topic
status: draft
updated: 2026-11-26
last_checked: 2026-11-26
tags: [ai, research, analysis, pde]
sources: [arxiv.org, deepmind.google, tech-insider.org]
---

# AI as Research Collaborator

**Hook:** AI is no longer just doing calculus homework. It is turning up strange functions and blow-up solutions that professional analysts hadn't found, and the field is still arguing about what that's worth.

## Six episodes to know

**1. AlphaEvolve and the inequality hunters (Nov 2025, preprint)**
Georgiev, [[Javier Gomez-Serrano|Gómez-Serrano]], [[Terence Tao]], and Wagner pointed Google DeepMind's **AlphaEvolve** at 67 problems in analysis, combinatorics, geometry, and number theory. The system writes code that searches for examples, tests them, and refines them. It reportedly matched the best known results in most cases and **improved several**, including bounds on autocorrelation inequalities, a classic type of analysis problem. Most of these are *constructions and bounds*, not new proofs.

**2. Blow-ups in fluid equations (Sep 2025, preprint)**
A DeepMind-led team, working with researchers at Brown, NYU, and Stanford (including [[Tristan Buckmaster]] and [[Javier Gomez-Serrano|Javier Gómez-Serrano]]), used neural networks with very high numerical precision to find new families of **unstable singularities** (solutions that blow up, but only if the starting conditions are exactly right). They found these in equations closely related to Navier-Stokes. They describe the precision as a step toward computer-assisted proofs, but such proofs are not complete. Quanta (Jan 2026) traces the project to 2021 and reports the approximations became about a billion times more accurate since the team's first attempts. This is **not** a resolution of the [[Navier-Stokes Smoothness Problem]].

**3. The mass release (Oct 2026)**
OpenAI published hundreds of manuscripts from an unreleased internal model, claiming full or partial solutions to open problems, including some in differential equations. According to secondary reporting, about **42%** of top-line results had Lean-checked proofs as of Oct 7, three manuscripts were withdrawn after a sign error, and the totals vary by outlet. Mathematicians quoted in coverage raised concerns about credit, overlap with unpublished human work, and how much the field can realistically review. **Status: claims under community review.**

**4. A conjecture falls (Jul 2026)**
[[Levent Alpoge|Levent Alpöge]] announced a counterexample to the 87-year-old [[Jacobian Conjecture]] in three dimensions, found with an Anthropic Claude model. It is a short polynomial map that anyone can check, and several mathematicians and an Isabelle formal proof did. The two-dimensional case remains open.

**5. The Navier-Stokes claim (Sep 2026)**
OpenAI claimed a Lean-checked proof that the forced 3D Navier-Stokes equations can blow up. The work built on a human strategy by [[Cordoba and Martinez-Zoroa|Córdoba and Martínez-Zoroa]] and arrived amid a credit dispute with [[Tristan Buckmaster|Buckmaster]] and Alpöge's forced-Euler result. **Status: claimed, under review.** See [[Navier-Stokes Smoothness Problem]].

**6. The Riemann hypothesis claim (Nov 2026)**
[[Levent Alpoge|Alpöge]] posted a claimed proof of the [[Riemann Hypothesis]], made "working with Claude," as about 17 million lines of Lean. The Lean FRO and Mathlib Initiative certified the Lean proof a day later. It followed two AI-linked steps on the same problem: an Anthropic model's 67.2% bound for zeros on the critical line (Aug) and OpenAI's quasi-Riemann hypothesis (Oct). **Status: formally verified, not yet understood or peer reviewed by humans.**

## The pattern

AI is strongest at **search**: trying vast numbers of candidate functions, constants, or constructions. A counterexample, once found, is easy to check. A 166-page proof is not. By November 2026 a new pattern appeared: a proof that a computer has checked but that no human yet understands. People still decide which questions matter, check the results, and turn numerical evidence into proofs.

## Next stop

- [[Proof Assistants and Lean]]: how claimed proofs get machine-checked
- [[Navier-Stokes Smoothness Problem]]: the prize problem behind the fluid work
- [[Jacobian Conjecture]]: what's left after the counterexample
- [[Riemann Hypothesis]]: episode 6 in full
- [[Open Problems]]
- [[Calculus and AI]]: the overview
- [[Javier Gomez-Serrano]] and [[Tristan Buckmaster]]: the mathematicians in episodes 1-2

## Sources (checked 2026-11-13)

- [Mathematical exploration and discovery at scale](https://arxiv.org/abs/2511.02864), Georgiev, Gómez-Serrano, Tao, Wagner, arXiv preprint (v3 Dec 2025)
- [Discovering new solutions to century-old problems in fluid dynamics](https://deepmind.google/blog/discovering-new-solutions-to-century-old-problems-in-fluid-dynamics/), Google DeepMind blog, Sep 2025 (paper: arXiv 2509.14185)
- [OpenAI math repository formalizes about 42% in Lean](https://tech-insider.org/openai-math-papers-lean-verification-42-percent-2026/), tech-insider.org, Oct 2026 (secondary reporting; OpenAI's own page could not be fetched)
- [Using AI, Mathematicians Find Hidden Glitches in Fluid Equations](https://www.quantamagazine.org/using-ai-mathematicians-find-hidden-glitches-in-fluid-equations-20260109/), Quanta, Jan 9, 2026 (checked 2026-11-21)
- Episodes 4-5 (checked 2026-11-15): see the sources listed in [[Jacobian Conjecture]] and [[Navier-Stokes Smoothness Problem]]
- Episode 6 (checked 2026-11-26): see the sources listed in [[Riemann Hypothesis]]
