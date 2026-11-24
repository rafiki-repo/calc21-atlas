---
type: topic
status: draft
updated: 2026-11-24
last_checked: 2026-11-24
tags: [ai, tutoring, randomized-trial, education]
sources: [pnas.org, knowledge.wharton.upenn.edu, pmc.ncbi.nlm.nih.gov, nber.org, the74million.org, arxiv.org]
---

# AI Tutors in Math Class

**Hook:** Give a student a chatbot and their homework scores go up. Take it away at exam time and, in one trial, they did *worse* than students who never had it. The randomized evidence on AI tutors is now arriving, and it is more mixed than the headlines.

## The short version

- **Practice scores and real learning are different things.** Several trials show big gains *while* the AI is available and little or none on a later test without it.
- **Design matters.** Tutors built to give hints instead of answers do better than an open chatbot.
- **Students often don't use them.** Access alone has produced small effects.
- **Almost none of it is about calculus yet.** Most trials are in middle or high school math, or in physics.

## Five studies worth knowing

| Study | Who | What happened |
|---|---|---|
| **Bastani et al., *PNAS* (Jun 2025)** | ~1,000 high school math students, Turkey, randomized | An open GPT-4 chat ("GPT Base") gave **48%** better practice scores, then **17% worse** exam scores without AI. A hint-giving version ("GPT Tutor") gave 127% better practice scores and about the same exam scores as the control group. The authors' reading: students used the open version as a crutch. |
| **Kestin et al., *Scientific Reports* (Jun 2025)** | 194 students in Harvard's intro physics for life sciences, randomized crossover | A GPT-4 tutor with expert-written, step-by-step prompts produced learning gains reported as **more than double** those of an in-class active-learning lesson, in less time (median 49 minutes). Authors list caveats: one course, pre-written answers, months of setup, and some authors also wrote the active-learning research it was compared with. |
| **Oreopoulos & Low, NBER (Aug 2026)** | 18 Tennessee middle schools, two-year cluster randomized trial of Khanmigo | About **0.06-0.08 standard deviations** per year, similar to Khan Academy *without* the AI. The median student messaged the tutor on only a third of practice days. The authors call engagement "the binding constraint." Working paper. |
| **Oreopoulos et al., NBER (Aug 2026)** | 6,000+ middle schoolers on the NUMI platform, randomized | AI help made students slower but more accurate after mistakes. The best delayed-test result (marginal) came from AI combined with mastery-based progression. Working paper. |
| **Eedi and Google DeepMind (reported Oct 2026)** | 1,179 UK secondary students, randomized | AI and human tutors both lifted in-the-moment accuracy (56-58% vs 43%), but **neither improved standardized test scores** over standard practice. 7 AI messages with false math reached students (human tutors also made 7 math errors). Reported by *The 74*; the study's own report was not checked here. |

## And calculus?

The closest thing so far is a **case study, not a trial**: a 2026 arXiv preprint (Barghorn et al.) on a small language model that answered forum questions in a large university **Calculus I** course. It was trained on 2,588 past student-instructor exchanges. It got **75.3%** of a 150-question benchmark right and matched or beat the instructor's answer in 36% of cases. Students surveyed (105) liked the speed but still waited for the instructor to confirm.

**Open question:** whether any of the school-math results carry over to limits, related rates, and integration. No randomized trial of an AI tutor in a college calculus course turned up as of this check.

## Next stop

- [[Calculus and AI]]: where chatbots get calculus wrong
- [[Active Learning in Calculus]]: the human-only version of "stop lecturing," also tested in a randomized trial
- [[Widening Access to Calculus]]: AI tutors in free courseware
- [[Education]]

## Sources (checked 2026-11-24)

- [Generative AI without guardrails can harm learning: evidence from high school mathematics](https://knowledge.wharton.upenn.edu/article/without-guardrails-generative-ai-can-harm-education), Wharton summary of Bastani et al., *PNAS* 122(26), 2025, doi 10.1073/pnas.2422633122
- [AI tutoring outperforms in-class active learning](https://pmc.ncbi.nlm.nih.gov/articles/PMC12179260/), Kestin et al., *Scientific Reports*, 2025 (open access)
- [One Click Away: AI Tutoring with Khanmigo in a Two-Year School Experiment](https://www.nber.org/papers/w35620), NBER working paper 35620, Aug 2026
- [Making AI Tutoring Productive](https://www.nber.org/papers/w35621), NBER working paper 35621, Aug 2026
- [Five things you should know about new AI tutor study](https://www.the74million.org/article/five-things-you-should-know-about-new-ai-tutor-study/), *The 74*, Oct 29, 2026
- [AI Meets Mathematics Education: a case study](https://arxiv.org/abs/2603.26679), Barghorn et al., arXiv preprint, Mar 2026
