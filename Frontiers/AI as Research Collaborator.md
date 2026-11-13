---
type: topic
status: draft
updated: 2026-11-13
last_checked: 2026-11-13
tags: [ai, research, analysis, pde]
sources: [arxiv.org, deepmind.google, tech-insider.org]
---

# AI as Research Collaborator

**Hook:** AI is no longer just doing calculus homework. It is turning up strange functions and blow-up solutions that professional analysts hadn't found, and the field is still arguing about what that's worth.

## Three episodes to know

**1. AlphaEvolve and the inequality hunters (Nov 2025, preprint)**
Georgiev, Gómez-Serrano, [[Terence Tao]], and Wagner pointed Google DeepMind's **AlphaEvolve** at 67 problems in analysis, combinatorics, geometry, and number theory. The system writes code that searches for examples, tests them, and refines them. It reportedly matched the best known results in most cases and **improved several**, including bounds on autocorrelation inequalities, a classic type of analysis problem. Most of these are *constructions and bounds*, not new proofs.

**2. Blow-ups in fluid equations (Sep 2025, preprint)**
A DeepMind-led team, working with researchers at Brown, NYU, and Stanford, used neural networks with very high numerical precision to find new families of **unstable singularities** (solutions that blow up, but only if the starting conditions are exactly right). They found these in equations closely related to Navier-Stokes. They describe the precision as a step toward computer-assisted proofs, but such proofs are not complete. This is **not** a resolution of the [[Navier-Stokes Smoothness Problem]].

**3. The mass release (Oct 2026)**
OpenAI published hundreds of manuscripts from an unreleased internal model, claiming full or partial solutions to open problems, including some in differential equations. According to secondary reporting, about **42%** of top-line results had Lean-checked proofs as of Oct 7, three manuscripts were withdrawn after a sign error, and the totals vary by outlet. Mathematicians quoted in coverage raised concerns about credit, overlap with unpublished human work, and how much the field can realistically review. **Status: claims under community review.**

## The pattern

AI is strongest at **search**: trying vast numbers of candidate functions, constants, or constructions. People still decide which questions matter, check the results, and turn numerical evidence into proofs.

## Next stop

- [[Proof Assistants and Lean]]: how claimed proofs get machine-checked
- [[Navier-Stokes Smoothness Problem]]: the prize problem behind the fluid work
- [[Open Problems]]
- [[Calculus and AI]]: the overview

## Sources (checked 2026-11-13)

- [Mathematical exploration and discovery at scale](https://arxiv.org/abs/2511.02864), Georgiev, Gómez-Serrano, Tao, Wagner, arXiv preprint (v3 Dec 2025)
- [Discovering new solutions to century-old problems in fluid dynamics](https://deepmind.google/blog/discovering-new-solutions-to-century-old-problems-in-fluid-dynamics/), Google DeepMind blog, Sep 2025 (paper: arXiv 2509.14185)
- [OpenAI math repository formalizes about 42% in Lean](https://tech-insider.org/openai-math-papers-lean-verification-42-percent-2026/), tech-insider.org, Oct 2026 (secondary reporting; OpenAI's own page could not be fetched)
