---
type: resource
status: draft
updated: 2026-11-25
last_checked: 2026-11-25
cost: mostly free; Wolfram|Alpha step-by-step is paid
tags: [software, graphing, computer-algebra, cas, tools]
sources: [amplify.com, blog.desmos.com, apcentral.collegeboard.org, geogebra.org, sagemath.org, sympy.org, wolframalpha.com]
---

# Graphing and Computer Algebra Tools

**Hook:** The graphing calculator used to be a pricey handheld. Now a free browser tab draws the curve, a second one does the algebra, and in 2027 one of them is built into the AP Calculus exam.

## Two kinds of tool

- **Graphing** tools *show*: type a function, get a picture, drag a slider. Good for seeing what a derivative or an integral means.
- **Computer algebra systems (CAS)** *manipulate symbols*: they return the exact derivative, antiderivative, limit, or series, not just a number. Good for checking work and handling messy algebra.

## The shelf

| Tool | Kind | Cost | What stands out |
|---|---|---|---|
| **[Desmos](https://www.desmos.com/calculator)** | Graphing (2D, [3D](https://www.desmos.com/3d), geometry) | Free | Sliders make it easy to animate an idea, such as a secant line turning into a tangent. Built into College Board's Bluebook app for the calculator parts of the 2027 AP Calculus exams |
| **[GeoGebra](https://www.geogebra.org/calculator)** | Graphing + geometry + CAS | Free for non-commercial use | One suite does pictures *and* symbolic algebra; over a million user-made classroom activities, by its own count |
| **[SageMath](https://www.sagemath.org/)** | Full CAS | Free, open source (GPL) | Bundles many open-source packages (SymPy, Maxima, NumPy, and others) behind one Python-style language. Runs online in [SageMathCell](https://sagecell.sagemath.org/), no install |
| **[SymPy](https://www.sympy.org/)** | CAS as a Python library | Free, open source (BSD) | For anyone already writing Python; [try it in the browser](https://live.sympy.org/) |
| **[Wolfram\|Alpha](https://www.wolframalpha.com/)** | Answer engine (commercial) | Free answers; step-by-step is paid (Pro) | Plain-English input ("integrate x sin x"). Step-by-step solutions sit behind the Pro subscription |

## Fine print

- **Who runs them.** Desmos split in 2022: Amplify bought the curriculum side, and the calculators went to **Desmos Studio**, a public benefit corporation led by founder Eli Luberoff, which said they would stay free for students and teachers. GeoGebra has been part of India's **BYJU'S** group since 2021. BYJU'S Indian parent is in insolvency proceedings, and a list of its assets for sale published in Oct 2025 includes its stake in GeoGebra GmbH (per *Insolvency Tracker*). GeoGebra's own page says its apps remain free for the public. This check found no report that this has changed.
- **A CAS answer is not a proof.** CAS output can differ from a textbook answer by a constant or a branch choice, and it can quietly assume things like *x* > 0. For machine-*checked* reasoning, see [[Proof Assistants and Lean]].
- **Exams differ.** On the 2027 AP Calculus exams, Desmos is available only in the calculator-required parts, and students may also bring up to two approved handhelds (College Board policy for 2026-27).

## Good for / not good for

- **Good for:** seeing ideas move (Desmos, GeoGebra), checking a messy antiderivative (any CAS), and computing at scale (SageMath, SymPy).
- **Not good for:** learning *why* a step works. For that, pair a tool with a course, such as [[MIT OCW Single Variable Calculus]].

## Sources (checked 2026-11-25)

- [Amplify acquires Desmos curriculum; Desmos calculators to remain independent and free](https://amplify.com/news/amplify-acquires-desmos-curriculum-to-build-the-future-of-math-instruction-desmos-calculators-to-remain-independent-and-free-to-all/), Amplify, May 18, 2022
- [Introducing Desmos Studio's 3D Calculator (Beta)](https://blog.desmos.com/articles/beta-3d-release), Desmos blog, Sep 28, 2023
- [AP Exams Calculator Policy](https://apcentral.collegeboard.org/exam-administration-ordering-scores/administering-exams/exam-policies/calculator-policy), AP Central (2026-27)
- [About GeoGebra](https://www.geogebra.org/about); [List of Byju's assets up for sale](https://insolvencytracker.in/2025/10/05/list-of-byjus-assets-up-for-sale-under-insolvency-resolution-process/), *Insolvency Tracker*, Oct 5, 2025
- [sagemath.org](https://www.sagemath.org/) (version 10.10 listed); [sympy.org](https://www.sympy.org/); [Wolfram|Alpha Pro](https://www.wolframalpha.com/pro)

## Next stop

- [[CalcPlot3D]]: a free 3D plotter built specifically for Calc III
- [[Calculus and AI]]: what happens when the "tool" is a chatbot instead of a CAS
- [[AP Calculus]]: the exam that now ships with a calculator inside
- [[Resources]]
