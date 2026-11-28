---
type: application
status: draft
updated: 2026-11-28
last_checked: 2026-11-28
tags: [engineering, control, feedback, derivatives, integrals, history]
sources: [ieeexplore (Bennett 1984, via ntnu.no), Åström & Hägglund 2006 (via ntnu.no), fbswiki.org]
---

# PID Controller

**Hook:** Refineries, paper mills, even the motor in a DVD player: a huge share of the machines that hold something steady run on one formula, and it has an integral and a derivative right in its name.

## The idea

A controller watches the **error** *e*(*t*): the gap between where a system is and where it should be (the target temperature minus the actual one, say). It then pushes back with three terms added together:

$$u(t) = K_p\,e(t) \;+\; K_i\int_0^t e(\tau)\,d\tau \;+\; K_d\,\frac{de}{dt}$$

- **P (proportional): the present.** Push harder the farther off you are.
- **I (integral): the past.** Add up the error over time. A small, stubborn offset keeps growing this term until it gets fixed. (Åström and Hägglund: integral action removes "steady-state offsets.")
- **D (derivative): the future.** If the error is shrinking fast, ease off before you overshoot. It "can anticipate the future," in the same authors' words.

Tuning the three dials *K*ₚ, *K*ᵢ, *K*_d is the craft. Too much P or I and the system oscillates; too little and it is sluggish.

## Where it came from: steering a battleship

- **1922.** Nicolas Minorsky published "Directional stability of automatically steered bodies," an analysis of automatic ship steering for the US Navy. According to control historian S. Bennett (*IEEE Control Systems Magazine*, 1984), Minorsky started from how a good helmsman behaves, and turned "properly timed" rudder action into the three-term rule.
- **1923.** He tested it on the battleship USS *New Mexico* (reported only in 1930). Bennett writes that the first version settled into a ±2° wobble, and Minorsky added acceleration control while at sea.
- **Commercial loser, theoretical winner.** The Sperry company's system won in the market. A Sperry director called its check-helm method "frankly a dodge." Minorsky's paper stayed little known outside naval engineering for years. Industrial three-term controllers are said to start with the Taylor Instrument Company in 1936 (Bennett reports this as a claim).

## How common is it?

Karl Åström and T. Hägglund (*Advanced PID Control*, 2006) write that in process control, "more than 95 percent of the control loops are of PID type," and most of those are actually PI (no derivative). They cite industry surveys: a 1989 Japanese study (over 90%) and a 2002 survey of US process plants (97%). Even CD and DVD players, they note, run three PID loops for speed, focus, and tracking.

## Go deeper

- [Feedback Systems](https://fbswiki.org/wiki/index.php/Feedback_Systems:_An_Introduction_for_Scientists_and_Engineers), Karl Åström and Richard Murray (2nd ed., Princeton University Press): free PDF from the authors' site; Chapter 11 is "PID Control." Assumes differential equations.
- [Nicolas Minorsky and the Automatic Steering of Ships](https://skoge.folk.ntnu.no/puublications_others/1984_Bennett-PID%20history.pdf), S. Bennett, *IEEE Control Systems Magazine* (1984): scanned PDF of the history, hosted on an NTNU course site.

## Next stop

- [[Fundamental Theorem of Calculus]]: why "add up the past" and "rate of change now" are two sides of one coin
- [[Weather Forecasting]]: the other big way engineers use derivatives to look ahead
- [[Glossary#Feedback|Feedback]] and [[Glossary#Derivative|Derivative]]
- [[Applications]]
