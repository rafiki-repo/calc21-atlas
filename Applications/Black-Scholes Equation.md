---
type: application
status: draft
updated: 2026-11-18
last_checked: 2026-11-18
tags: [finance, economics, pde, stochastic-calculus]
sources: [frbsf.org, ocw.mit.edu, tobydriscoll.net, mathunion.org, news.mit.edu]
---

# Black-Scholes Equation

**Hook:** In 1973 a partial differential equation came out of finance that is, after a change of variables, the heat equation from physics. Two of its creators later shared the economics Nobel.

## The question

An **option** is a contract giving the right, but not the obligation, to buy (or sell) a stock at a set price on a set date. What is that right worth today, when the stock price moves at random?

## The idea

- **Model the stock** as a random walk with drift (geometric Brownian motion), using [[Stochastic Calculus|Itô's calculus]].
- **Hedge.** Combine the option with just the right amount of stock so that the randomness cancels. A riskless portfolio has to earn the risk-free interest rate, or someone could make money for nothing. That condition fixes the price, whatever an investor's attitude to risk.
- **The result is a PDE** for the option value *v*(*S*, *t*), where *S* is the stock price, *r* the interest rate, and σ the volatility:

$$\frac{\partial v}{\partial t} + \tfrac12\sigma^2 S^2 \frac{\partial^2 v}{\partial S^2} + rS\frac{\partial v}{\partial S} - rv = 0$$

It is solved **backward in time** from the known payoff at the expiry date. A change of variables turns it into the **heat equation**, which has a known solution. That solution gives the Black-Scholes formula.

## Who and when

- **1973:** Fischer Black and Myron Scholes published the formula. Robert C. Merton published a paper the same year with the formula and extensions. Organized options trading began in Chicago that year too.
- **1997:** Merton and Scholes received the Nobel Memorial Prize in Economic Sciences. Fischer Black, who taught at MIT's Sloan School from 1975 to 1984, had died in 1995 at 57, and Nobel Prizes are not awarded posthumously ([MIT News, 1997](https://news.mit.edu/1997/nobels-1022)).

## The fine print

The model assumes, among other things, **continuous trading** and a **known, constant volatility**. Real markets don't fully cooperate, and even the Federal Reserve Bank of San Francisco's 1998 explainer notes that derivatives-based hedging "is not always foolproof." Practitioners use many extensions of the model.

## Go deeper

- [The 1997 Nobel Prize in Economics](https://www.frbsf.org/research-and-insights/publications/economic-letter/1998/02/the-1997-nobel-prize-in-economics/), John Krainer, FRBSF Economic Letter (1998). Plain-language explanation of the hedging idea, with a worked toy example. Free.
- [MIT 18.642, Week 14](https://ocw.mit.edu/courses/18-642-topics-in-mathematics-with-applications-in-finance-fall-2024/pages/week-14/), MIT OCW (2024). Lecture 25 derives the equation and connects it to the heat equation. Free.
- [Black–Scholes equation](https://tobydriscoll.net/fnc-julia/diffusion/blackscholes.html), from *Fundamentals of Numerical Computation* by Driscoll and Braun. Shows how to solve it numerically on a computer. Readable online.

## Next stop

- [[Stochastic Calculus]]: the calculus underneath
- [[Weather Forecasting]]: another PDE solved step by step on a computer
- [[Glossary#Partial differential equation (PDE)]]
- [[Applications]]
