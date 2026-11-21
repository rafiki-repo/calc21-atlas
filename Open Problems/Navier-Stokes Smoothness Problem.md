---
type: open-problem
status: draft
updated: 2026-11-21
last_checked: 2026-11-18
tags: [pde, millennium-prize, ai]
sources: [claymath.org, quantamagazine.org, sciencenews.org, scientificamerican.com, arxiv.org]
---

# Navier-Stokes Smoothness Problem

**Hook:** The equations for how water and air flow are nearly two centuries old and used every day. In September 2026, an AI-driven team claimed to show that they can break down. The claim is not yet confirmed, and mathematicians are still checking it.

## The question

The Navier-Stokes equations model fluid motion. In three dimensions, can a smooth starting flow develop a **singularity** (a point where speed or another quantity becomes infinite) in finite time, or do solutions always stay smooth? Proving either answer is one of the Clay Mathematics Institute's seven **Millennium Prize Problems** ($1 million). The official problem allows a proof of breakdown in which a smooth **outside force** pushes on the fluid.

## Status: claimed, under review

- **The claim (Sep 8, 2026):** OpenAI announced a proof of finite-time blow-up for the 3D equations **with a smooth outside force** (the "forced" version). It came with a 166-page paper and a **Lean** formalization. Quanta reports the work came from about 10,000 AI agents running an unreleased model for 88 hours.
- **Built on human work:** both Quanta and Science News report that the AI efforts leaned heavily on a strategy by **Diego Córdoba** and **Luis Martínez-Zoroa** (see [[Cordoba and Martinez-Zoroa]]). Charles Fefferman, who wrote the official problem statement, credited them as "the heroes".
- **A day earlier:** [[Tristan Buckmaster]] (NYU) and [[Levent Alpoge|Levent Alpöge]] (Anthropic) reported AI-assisted, Lean-checked blow-up for the related **forced Euler** equations (fluids without viscosity).
- **Checking:** a Lean check confirms only the statement that was formalized. People still have to confirm that it matches the intended theorem. A preprint by Bastounis, Circelli and Hansen ([arXiv 2610.08144](https://arxiv.org/abs/2610.08144), Oct 6, 2026; not peer reviewed) argues that OpenAI's Lean formalization **does not match** its written proof. It also argues, more generally, that Lean checking of AI translations gives little confidence in the original text. As of Science News's report, no one had finished a full human review.
- **Prize:** OpenAI says it will not claim the prize. On Sep 11, 2026, Clay [posted a short statement](https://www.claymath.org/news/navier-stokes-announcement/) about the announcement that the problem "has apparently been settled". It named no one and said its evaluation process "is deliberately unhurried". Clay requires peer-reviewed publication and still lists the problem as **"active"**, with no solver acknowledged as of last check.
- **Credit:** there is a public dispute over priority and over whether the work drew on other researchers' AI sessions. OpenAI denies that it did.
- **Not settled:** whether *unforced* blow-up happens, the version many analysts consider the heart of the matter. *Scientific American* (Sep 21, 2026) reports that the forced result, if it holds, fits Clay's 2000 wording, which allows an outside force. It also quotes Luis Silvestre (University of Chicago): "The most important problem is unsolved." The same article reports a separate proof, posted the week before, that OpenAI's method cannot be extended to the unforced case. Córdoba counters that "all fluids we know of are under some kind of external force."

**Earlier AI work (not a solution):** In Sep 2025, a Google DeepMind-led team including [[Tristan Buckmaster]] and [[Javier Gomez-Serrano|Javier Gómez-Serrano]] found *unstable* blow-up candidates in related fluid equations (arXiv 2509.14185). See [[AI as Research Collaborator]].

**Related but different:** [[Hilbert Sixth Problem]] asks where these equations *come from* (colliding particles), not whether their solutions stay smooth.

## Why it connects to calculus

It is a question about **[[Glossary#Partial differential equation (PDE)|PDEs]]** and about what "[[Glossary#Smooth|smooth]]" really guarantees. Physically, little changes: real fluids are made of molecules, so the equations already stop applying at tiny scales.

## Sources (checked 2026-11-15; Clay and arXiv items 2026-11-17; Scientific American 2026-11-18)

- [Clay Institute problem page](https://www.claymath.org/millennium/navier-stokes-equation/) (status "active") and [Clay's Sep 11, 2026 announcement](https://www.claymath.org/news/navier-stokes-announcement/)
- [Navier-Stokes lost in translation](https://arxiv.org/abs/2610.08144), Bastounis, Circelli, Hansen, arXiv preprint, Oct 6, 2026
- [AI Has Solved One of Math's $1 Million Millennium Prize Problems](https://www.quantamagazine.org/ai-has-solved-one-of-maths-1-million-millennium-prize-problems-20260908/), Quanta, Sep 8, 2026. The headline says "solved", but the article says the result still has to hold up to scrutiny.
- [Did OpenAI solve the wrong Navier-Stokes problem?](https://scientificamerican.com/article/did-openai-solve-the-wrong-navier-stokes-problem), Joseph Howlett, Scientific American, Sep 21, 2026. The forced-vs-unforced question.
- [AI may have solved one of math's biggest puzzles, raising controversy](https://www.sciencenews.org/article/ai-math-puzzle-navier-stokes-openai), Science News, Sep 9, 2026

## Next stop

- [[Weather Forecasting]]: where cousins of these equations are solved numerically every day
- [[AI as Research Collaborator]]: how AI got here
- [[Proof Assistants and Lean]]: what a Lean check does and doesn't prove
- [[Jacobian Conjecture]]: another 2026 AI-assisted shock, this one a counterexample
- [[Open Problems]]
