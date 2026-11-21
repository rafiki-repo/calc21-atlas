---
type: open-problem
status: draft
updated: 2026-11-21
last_checked: 2026-11-21
tags: [series, zeta, irrationality, number-theory, lean]
sources: [github.com, isa-afp.org, functor.network, arxiv.org, epoch.ai]
---

# Irrationality of Zeta Values

**Hook:** Euler showed that 1 + 1/4 + 1/9 + ... equals π²/6. Swap the squares for cubes or fifth powers and nobody can find a formula. For centuries, nobody could even prove these sums are irrational. In Sept 2026 a preprint claimed ζ(5), and proof-checking software has already been through it.

## The question

The **zeta values** are infinite sums: ζ(s) = 1 + 1/2ˢ + 1/3ˢ + ... For which whole numbers s is ζ(s) **irrational**, meaning not a fraction?

- **Even s: settled.** Euler found ζ(2), ζ(4), ζ(6), ... as rational multiples of powers of π (see [[Basel Problem]]). Because powers of π are irrational, so are these sums.
- **Odd s: hard.** No formula like Euler's is known, so each one has to be attacked directly.

## Status (checked 2026-11-20)

| Value | Status |
|---|---|
| ζ(3) | **Irrational.** Roger Apéry proved it in 1978 |
| ζ(5) | **Proof claimed (Sep 2026).** A preprint by Aabir Fauzan, now formally verified (conditions below) and already being built on. Not yet peer reviewed |
| ζ(7), ζ(9), ... | **Open** individually. Work by Ball and Rivoal (around 2000) shows that infinitely many odd zeta values are irrational, without saying which ones |

**The ζ(5) claim in more detail:**

- **Where:** Fauzan posted *ζ(5) is irrational* on **Zenodo** on Sep 17, 2026, rather than on arXiv. The method uses carefully chosen determinants of polynomials, multiple-integral bounds, and prime-by-prime bookkeeping.
- **Machine-checked:** Within weeks there were several **formalizations**. Dan Romik's Lean 4 version reports no gaps ("no `sorry`"). It takes one input as an axiom, the prime number theorem, which Lean's main library does not yet contain. Its README says Claude models wrote the Lean code under Romik's direction. An Isabelle/HOL port entered the Archive of Formal Proofs in Oct 2026. These confirm the argument as formalized. They are not a substitute for peer review.
- **Being built on:** an Oct 2026 arXiv preprint (Li Lai) adapts Fauzan's method to prove 1, ζ(3), ζ(4) linearly independent. Another (Nov 2026) improves a bound and states plainly that it is "conditional on Fauzan's preprint."

## The same family: Euler's constant

**Euler's constant** γ ≈ 0.5772 is what is left when you subtract ln n from 1 + 1/2 + ... + 1/n and let n grow. Nobody knows whether it is irrational. Jeffrey Lagarias's 100-page survey calls this "a long-standing open problem." Epoch AI's open-problems list still names γ as an unsolved target, along with ζ(7).

## A disputed cousin: Catalan's constant

**Catalan's constant** G = 1 − 1/3² + 1/5² − 1/7² + ... ≈ 0.9160 is another series nobody has proved irrational. A Sep 2026 arXiv preprint by Zhi-Wei Sun claims a proof. Two weeks later a short note by Dane Wachs reported exact computations that contradict a key estimate. It concludes that the proof as written is incomplete, and it takes no side on the answer. **Status (checked 2026-11-21): claimed and disputed. G is still treated as open.**

## Why it connects to calculus

Every number here is a **limit**: an infinite [[Glossary#Series|series]] or a sum minus a logarithm. Proving irrationality usually means building very good fraction approximations, often out of integrals, and showing they are *too* good for any fraction to allow.

## Sources

- [zeta5-irrationality](https://github.com/danromik/zeta5-irrationality), Dan Romik's Lean 4 formalization (links the Zenodo preprint), Sep 2026
- [The Irrationality of ζ(5)](https://isa-afp.org/entries/Zeta_5_Irrational.html), Archive of Formal Proofs, Oct 2026
- [Zeta(5) is irrational](https://functor.network/user/3333/entry/1997), Bogdan Grechuk's explainer, Sep 29, 2026
- [The linear independence of 1, ζ(3), and ζ(4)](https://arxiv.org/abs/2610.06838), L. Lai, arXiv preprint, Oct 2026
- [A new upper bound for the irrationality exponent of ζ(5)](https://arxiv.org/abs/2611.01708), D. Niedbala Giraudin, arXiv preprint, Nov 2026
- [Catalan's constant is irrational](https://arxiv.org/abs/2609.04176), Z.-W. Sun, arXiv preprint, Sep 3, 2026, and [A note on a recent claimed proof...](https://arxiv.org/abs/2609.22339), D. Wachs, arXiv, Sep 16, 2026
- [Euler's constant: Euler's work and modern developments](https://arxiv.org/abs/1303.1856), J. Lagarias, *Bull. AMS* 50 (2013)
- [Apéry-Style Irrationality Proofs](https://epoch.ai/frontiermath/open-problems/apery-irrationality), Epoch AI FrontierMath open problems

## Next stop

- [[Basel Problem]]: the ζ(2) story that started it all
- [[Proof Assistants and Lean]]: how a 29,000-line proof check works
- [[Moving Sofa Problem]]: another claimed proof waiting on referees
- [[Open Problems]]
