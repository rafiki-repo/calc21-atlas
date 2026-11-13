---
type: topic
status: draft
updated: 2026-11-13
last_checked: 2026-11-13
tags: [ai, proof-assistants, lean, education]
sources: [theregister.com, arxiv.org, teorth.github.io, math-inc.github.io, deepmind.google, techcrunch.com]
---

# Calculus and AI

**Hook:** A chatbot can now help with research-level analysis and still slip up on the arithmetic in a word problem. Both are true at once, and this note maps out how.

## Three fronts

| Front | What is happening | Where to go |
|---|---|---|
| **AI as solver and tutor** | Chatbots answer homework, explain steps, and grade solutions. Their accuracy is uneven. | [[#Where chatbots stumble]] below |
| **AI plus proof checkers** | AI writes proofs in **Lean**, a language in which a computer checks every logical step. | [[Proof Assistants and Lean]] |
| **AI in research** | AI systems search for examples, bounds, and blow-up solutions that mathematicians then study. | [[AI as Research Collaborator]] |

## Where chatbots stumble

The evidence is still thin and mostly from preprints or vendors, but some consistent patterns show up:

- **Arithmetic is still the weak link.** In the second round of the **ORCA benchmark** (500 practical math questions, run by researchers linked to Omni Calculator, a company with a stake in calculators; reported by *The Register*, Feb 2026), the best model scored about 73%. **Calculation errors** were the most common type of mistake (about 40%).
- **Answers wobble.** The same benchmark found that models often gave a *different* answer when asked the same question again. This happened mostly when the answer was wrong.
- **Small slips are more common than misunderstandings.** A 2025 arXiv preprint by Zhang and Graf (arithmetic, algebra, and number theory; GPT-4o, o1, DeepSeek models) found **procedural slips** were the most common error. Conceptual errors were rarer. Pairing two AI agents to check each other helped substantially.
- **The calculus-specific gap.** Studies that test AI on real Calc I–III exams, or as a *tutor* rather than a solver, are only starting to appear. Treat any single headline number with caution.

**A useful distinction:** a fluent explanation is not the same as a checked one. That gap is why proof assistants (next row) attract so much interest.

## Next stop

- [[Proof Assistants and Lean]]: how a computer can *check* a calculus proof
- [[AI as Research Collaborator]]: AlphaEvolve, fluid blow-ups, and a contested mass release of proofs
- [[Terence Tao]]: a central figure in both analysis and AI-assisted math
- [[Education]]: how calculus is taught, and how AI is changing it

## Sources (checked 2026-11-13)

- [AI models suck slightly less at math than they did last year](https://www.theregister.com/2026/02/26/ai_models_get_better_at/), *The Register*, Feb 2026 (ORCA benchmark round 2; vendor-affiliated, pre-publication)
- [Mathematical Computation and Reasoning Errors by Large Language Models](https://arxiv.org/abs/2508.09932), Zhang & Graf, arXiv preprint, Aug 2025
