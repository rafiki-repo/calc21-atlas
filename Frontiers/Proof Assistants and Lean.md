---
type: topic
status: draft
updated: 2026-11-13
last_checked: 2026-11-13
tags: [ai, lean, formalization, proof-assistants]
sources: [leanprover-community.github.io, teorth.github.io, math-inc.github.io, techcrunch.com]
---

# Proof Assistants and Lean

**Hook:** What if a computer refused to accept a proof until every single step, down to "why is this limit allowed?", had been justified?

## The idea

A **proof assistant** is software that checks a proof line by line against strict logical rules. If the check passes, the logic is valid. **Lean** is one of the most widely used, and it is where much of the current AI-and-math work happens. Its community library, **Mathlib**, collects formalized mathematics, including a large amount of real and complex analysis: limits, derivatives, integrals, and series.

**Formalizing** means translating ordinary math into this checkable form. **Autoformalization** means having AI do the translating.

## Why calculus people care

- Calculus is full of fine print (continuity, convergence, swapping limits and integrals). A proof assistant won't let you skip any of it.
- AI-generated proofs can be machine-checked, which is the main proposed answer to "how do we trust a chatbot's math?"

## Milestones worth knowing

- **Analysis I, in Lean (2025).** [[Terence Tao]] released a Lean companion to his undergraduate analysis textbook. It covers material from constructing the real numbers through derivatives, Riemann integration, and the [[Fundamental Theorem of Calculus]]. See [[Lean Companion to Analysis I]].
- **Strong Prime Number Theorem (2025).** Math Inc. reports that its agent, **Gauss**, completed a challenge set by Tao and Alex Kontorovich in about three weeks. The result is roughly **25,000 lines** of Lean, including the complex-analysis groundwork the proof needed. Humans supplied the plan (a "blueprint") and reviewed key lemmas. The speed claims are the company's own.
- **The Stacks Project (Nov 2026).** The startup Axiom Math says its agents turned this roughly 7,600-page algebraic geometry reference into about 16 million lines of Lean (reported by *TechCrunch*). It is not calculus, but it shows how quickly the scale is growing. The claims are the company's own.

**Want to try it?** Tao's **Lean Grimoire** (Nov 2026) is a browser logic game that can show the Lean proof behind each move. It covers logic, not calculus, but it's a gentle way in. [Play it](https://teorth.github.io/tao-web/apps/grimoire.html).

## The fine print

- Lean checks that a proof proves **the statement as written in Lean**. If that statement mistranslates the original theorem, the check is meaningless. Reviewing the statements is still human work.
- Formal proof says nothing about originality or who deserves credit.

## Next stop

- [[Lean Companion to Analysis I]]: see a real calculus course, machine-checked
- [[AI as Research Collaborator]]: where AI produces new math, not just checks it
- [[Calculus and AI]]: the overview
- [[Glossary#Proof assistant]]

## Sources (checked 2026-11-13)

- [Lean community and Mathlib](https://leanprover-community.github.io/)
- [Strong PNT project page](https://math-inc.github.io/strongpnt), Math Inc. (self-reported)
- [Axiom Math wants to keep AI slop out of mathematics](https://techcrunch.com/2026/11/05/axiom-math-wants-to-keep-ai-slop-out-of-mathematics/), *TechCrunch*, Nov 5, 2026
