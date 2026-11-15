---
type: open-problem
status: draft
updated: 2026-11-15
last_checked: 2026-11-15
tags: [multivariable, algebra, ai, counterexample]
sources: [terrytao.wordpress.com, isa-afp.org, arxiv.org, smithsonianmag.com]
---

# Jacobian Conjecture

**Hook:** A napkin-sized claim about polynomial maps survived 87 years. In July 2026 it fell in three dimensions to an explicit counterexample found with AI help. The two-dimensional case is **still open**.

## The question

Take a polynomial map from n-dimensional space to itself. Its **[[Glossary#Jacobian|Jacobian determinant]]** measures how the map stretches or squashes volume at each point. Ottheinrich Keller asked in 1939 whether a nonzero *constant* determinant everywhere forces the map to have a polynomial inverse. That question became the Jacobian conjecture.

In calculus terms: if a map looks reversible **locally** at every single point, must it be reversible **globally**?

## Status (checked 2026-11-15)

| Dimension | Status |
|---|---|
| 1 | True (easy) |
| **2** | **Open** |
| 3 and up | **False.** Explicit counterexamples exist |

- **The counterexample (Jul 20, 2026):** mathematician **Levent Alpöge** (Anthropic; Harvard) announced a degree-7 polynomial map of three-dimensional complex space with Jacobian determinant exactly −2. The map is not one-to-one: three different points land on the same output. He credited an Anthropic Claude model with finding it and Akhil Mathew with suggesting the problem.
- **Checked:** the map is easy to verify, and several mathematicians did. [[Terence Tao]] posted a walkthrough the next day. An independent **Isabelle/HOL** formal proof confirms the counterexample and extends it to every dimension ≥ 3.
- **More counterexamples:** follow-up preprints report further families, including arXiv 2608.00222 by Shuhong Gao (not yet peer reviewed).
- **Reactions:** some called it the biggest conjecture AI has yet played a major role in. Andrew Blumberg (Columbia) noted that a counterexample shows *that* such maps exist but explains less than a proof would.

## Why it connects to calculus

The Jacobian is the multivariable [[Glossary#Derivative|derivative]]. The inverse function theorem says a nonzero Jacobian gives a local inverse near each point. The conjecture asked whether, for polynomials, local reversibility always becomes global. In three dimensions, it does not.

## Sources

- [A digestion of the Jacobian conjecture counterexample](https://terrytao.wordpress.com/2026/07/21/), Terence Tao's blog, Jul 21, 2026 (gives the explicit map)
- [Formal Verification of an Explicit Counterexample to the Jacobian Conjecture](https://isa-afp.org/entries/Jacobian_Counterexample.html), Archive of Formal Proofs, Jul 2026
- [Counterexamples to the Jacobian conjecture in dimensions greater than two](https://arxiv.org/abs/2608.00222), S. Gao, arXiv preprint
- [A.I. disproves a decades-old mathematical idea](https://www.smithsonianmag.com/smart-news/ai-disproves-a-decades-old-mathematical-idea-the-biggest-conjecture-that-the-tech-has-played-a-role-in-yet-180989189/), Smithsonian, Jul 27, 2026

## Next stop

- [[AI as Research Collaborator]]: where this fits in AI's 2026 run
- [[Proof Assistants and Lean]]: how a machine checks a counterexample
- [[Navier-Stokes Smoothness Problem]]: the other big 2026 claim
- [[Open Problems]]
