---
type: open-problem
status: draft
updated: 2026-11-26
last_checked: 2026-11-26
tags: [complex-analysis, number-theory, zeta-function, ai, lean, millennium-prize]
sources: [quantamagazine.org, scientificamerican.com, leanprover-community.github.io, anthropic.com, math.uwaterloo.ca, claymath.org]
---

# Riemann Hypothesis

**Hook:** Since 1859, one question about where a single function equals zero has topped mathematics' wish list. In November 2026, a 17-million-line computer proof said "done." Humans are still reading it.

**Status (as of 2026-11-26): claimed proof.** The Lean code has been certified by the people who maintain Lean and its main library, Mathlib. Mathematicians do not yet understand the argument, and there is no peer-reviewed paper.

## The question

- **Start with a sum you may know.** 1 + 1/2² + 1/3² + ... = π²/6 is the [[Basel Problem]]. Swap the 2 for any power *s* and you get the **zeta function**, ζ(*s*). See [[Glossary#Riemann zeta function]].
- **Riemann's move (1859):** he extended ζ to complex numbers *s*, where the sum alone no longer works, and tied its zeros to how the **prime numbers** are spread out.
- **The hypothesis:** apart from the "trivial" zeros at −2, −4, −6, ..., every zero of ζ has real part exactly **½**. That vertical line is the **critical line**. All of those zeros were already known to lie in the strip between real parts 0 and 1.
- **Why anyone cares:** the zeros control how far the actual count of primes strays from its predicted count. Many results in number theory are proved only on the assumption that it is true. It was on Hilbert's 1900 list (problem 8), and it is one of Clay's seven **$1 million Millennium Prize Problems**.

**Where calculus comes in:** the zeta function is an infinite [[Glossary#Series|series]], and the standard tools are complex analysis, which is calculus with complex numbers: contour integrals, analytic continuation, and careful bounds on sums.

## 2026: three steps in four months

| When | What was claimed | Who | Status |
|---|---|---|---|
| **Aug 10** | At least **67.2%** of the zeros lie on the critical line (up from 41.6%, per Anthropic) | An unreleased Anthropic Claude model; checked by Anthropic mathematicians [[Levent Alpoge\|Levent Alpöge]] and Ralph Furman | Paper and Lean formalization; Brian Conrey and Dan Goldston examined it on short notice. Not peer reviewed. Anthropic said it did not expect the method to lead to a full proof |
| **Oct 6** | The **quasi-Riemann hypothesis**: every zero has real part between 1/12 and 11/12 (a narrower strip than 0 to 1) | OpenAI, in its batch of AI-generated papers | The 49-page version is not formally verified; an earlier 199-page version, Lean-verified, gave 1/8 to 7/8. Experts quoted by *Quanta* largely think the result is correct; Peter Sarnak won't call it "a Theorem" until humans check every detail |
| **Nov 20** | **The full hypothesis**, and its generalization to Dirichlet L-functions | Levent Alpöge, "working with Claude": a four-page paper plus about 17 million lines of Lean | **Nov 21:** the Lean FRO and the Mathlib Initiative certified that "both the statement and the proof of the Riemann Hypothesis are correct." The certification covers the classical hypothesis. No peer review yet; no Clay ruling |

## What "certified" does and does not mean

- **Does:** the theorem in Alpöge's library is exactly Mathlib's standard statement of the hypothesis (checked by two comparison tools), dozens of people compiled it, and several independent proof checkers accepted it. Andrew Sutherland (MIT) ran the first independent compile on Nov 20. See [[Proof Assistants and Lean]].
- **Does not:** explain *why* it is true. Maksym Radziwiłł (NYU) told *Quanta* the write-up contains "nonsensical statements" and that the proof "doesn't answer" the "why?" question. Alpöge predicts the argument "will be massively simplified."
- **Work in progress:** a human-readable guide for the zeta case, prepared "at the behest of" Michael Rubinstein (Waterloo) with AI models (working draft, Nov 21), still takes its central inequality from the Lean code rather than proving it on paper.
- **The prize:** Clay's rules ask for publication in a qualifying outlet, **at least two years** of waiting, and "general acceptance" by mathematicians. So a decision cannot come soon.

**A separate claim:** on the same day, Ravi Vakil posted a 940-page, human-written manuscript by Alessandro Masullo claiming the generalized hypothesis. *Quanta* reports that number theorists are withholding judgment.

## Go deeper

- [*Quanta*'s running coverage](https://www.quantamagazine.org/updates/transformation/) of the November claim, with the timeline and expert reactions
- ["AI Proved the Quasi-Riemann Hypothesis. What Happens Now?"](https://www.quantamagazine.org/ai-proved-the-quasi-riemann-hypothesis-what-happens-now-20261019/), *Quanta*, Oct 19, 2026
- [Lean verification of the Riemann Hypothesis](https://leanprover-community.github.io/blog/posts/riemann-hypothesis/), the Lean FRO and Mathlib Initiative statement, Nov 21, 2026
- ["Anthropic mathematician claims to prove Riemann hypothesis"](https://www.scientificamerican.com/article/anthropic-mathematician-claims-to-prove-riemann-hypothesis-most-famous-problem-in-all-of-math/), *Scientific American*, Nov 20, 2026 (updated Nov 21)
- [The 67.2% result](https://www.anthropic.com/research/riemann-zeta), Anthropic research post, Aug 10, 2026 (company source)
- [Rubinstein's working guide](https://www.math.uwaterloo.ca/~mrubinst/alpoge_claude_grh/zeta-paper.pdf) (PDF draft; heavy going)
- [Millennium Prize rules](https://www.claymath.org/millennium-problems/rules/), Clay Mathematics Institute

## Next stop

- [[Basel Problem]]: the friendly sum where ζ begins
- [[Irrationality of Zeta Values]]: a different question about the same function
- [[Levent Alpoge]]: the claimant, and his 2026 run
- [[AI as Research Collaborator]]: the year AI started claiming big theorems
- [[Open Problems]]
