---
type: glossary
status: draft
updated: 2026-11-23
sources: unverified-seed
---

# Glossary

Plain-language definitions. Link to a term from any note with `[[Glossary#Term]]`. Back to [[Home]].

*(Keep entries to 1-3 sentences. Add alphabetically. Link to a fuller note in [[Concepts]] where one exists.)*

## A

### Antiderivative
A function whose derivative is the one you started with. Not unique: adding a constant gives another. See [[Fundamental Theorem of Calculus]].

### Autoformalization
Using AI to translate ordinary written math into a formal language that a [[Glossary#Proof assistant|proof assistant]] can check. See [[Proof Assistants and Lean]].

## B
### Brownian motion
The random, jittery path of a small particle knocked about by molecules, and the mathematical model of it. The path is continuous but has no slope anywhere. See [[Stochastic Calculus]].

## C

### Chain rule
The rule for differentiating a function inside another function: multiply the rates of change of each link in the chain. It is the engine of neural-network training; see [[Backpropagation and the Chain Rule]].

### Continuity
A function is continuous if you can draw its graph without lifting your pencil: small changes in the input cause only small changes in the output.

### Convergence
A sequence or series *converges* if it settles toward a single finite value. If it doesn't, it *diverges*. See [[Basel Problem]].

### Counterexample
A single specific case that shows a general claim is false. One is enough. See [[Jacobian Conjecture]].

## D

### Derivative
The instantaneous rate of change of a function; the slope of its graph at a point.

### Differential equation
An equation involving a function and its derivatives. Solving it means finding the function. Everyday examples: [[SIR Epidemic Model]], [[Weather Forecasting]]. See [[Navier-Stokes Smoothness Problem]] for a famous case, and a contested 2026 claim.

## E

### Euler's constant
The number γ ≈ 0.5772, the limit of (1 + 1/2 + ... + 1/n) − ln n. Nobody knows whether it is irrational. See [[Irrationality of Zeta Values]].

### Extreme value theorem
If a function is [[Glossary#Continuity|continuous]] on a closed interval [a, b], it reaches a largest and a smallest value somewhere on that interval. Drop "closed" or "continuous" and it can fail. See [[AP Calculus]], whose syllabus reworded it for Fall 2026.

## F

### Formal proof
A proof written in a precise language in which software can check every step. See [[Proof Assistants and Lean]].

### Fourier analysis
Breaking a complicated signal or function into a sum of simple waves (sines and cosines), then studying it piece by piece. The wider field is called *harmonic analysis*. See [[Kakeya Conjecture]].

### Fractional derivative
A derivative of non-whole order, such as a half derivative: do it twice and you get the ordinary derivative. Unlike the ordinary kind, it depends on the function's whole history back to a starting point. See [[Fractional Calculus]].

## G

### Gradient
For a function of several variables, the vector of its partial derivatives. It points in the direction of steepest increase. See [[CalcPlot3D]] to see one.

### Gradient descent
A way to minimize a function by repeatedly taking a small step in the direction opposite the [[Glossary#Gradient|gradient]], i.e. downhill. See [[Backpropagation and the Chain Rule]].

## H

### Hausdorff dimension
A way to give a size-exponent to irregular sets such as fractals: a line has dimension 1, a plane 2, and some fractals land in between. See [[Kakeya Conjecture]].

## I

### Infinitesimal
A quantity smaller than any positive number but not zero. Central to early calculus (see [[Newton vs Leibniz]]); modern treatments mostly replace it with limits, though [[Nonstandard Analysis]] revives it rigorously.

### Integral
The accumulated total of a changing quantity; the area under a curve. The *definite* integral gives a number; the *indefinite* integral gives a family of antiderivatives.

### Irrational number
A number that cannot be written as a fraction of whole numbers, such as √2 or π. Proving that a specific limit is irrational can be very hard. See [[Irrationality of Zeta Values]].

## J

### Jacobian
For a map with several inputs and outputs, the Jacobian is the grid (matrix) of all its partial derivatives, the multivariable version of the derivative. Its determinant measures how the map stretches or squashes volume near a point. See [[Jacobian Conjecture]].

## L

### Limit
The value a function approaches as its input approaches some point. The idea that makes "instantaneous" meaningful.

## M

### Method of exhaustion
The ancient Greek way to find a curved area or volume without limits: trap it between simpler shapes from inside and outside, and show that any other answer leads to a contradiction. Archimedes used it to prove results he had first found by slicing. See [[Archimedes Palimpsest]].

## P

### Partial derivative
The derivative of a multivariable function with respect to one variable, holding the others fixed.

### Partial differential equation (PDE)
A [[Glossary#Differential equation|differential equation]] whose unknown function depends on several variables, such as position and time. Heat, waves, and fluids are all described by PDEs. See [[Hilbert Sixth Problem]].

### Power series
An "infinite polynomial" a₀ + a₁x + a₂x² + ..., such as the series for sine or cosine. Found for trigonometric functions in Kerala around 1400 and in Europe in the 17th century. See [[Kerala School]] and [[Glossary#Series|Series]].

### Proof assistant
Software, such as Lean, that checks proofs step by step against strict logical rules. It confirms the logic, but not whether the statement says what was intended. See [[Proof Assistants and Lean]].

## R

### Riemann sum
An approximation of an integral made by chopping an interval into thin strips and adding up their areas. As the strips get thinner, the sum approaches the integral. Competition problems sometimes hide one inside a limit; see [[MIT Integration Bee]].

## S

### Series
A sum of infinitely many terms. See [[Basel Problem]].

### Singularity
A point or moment where a solution stops making sense, usually because some quantity becomes infinite. In fluids this is called **blow-up**. A blow-up is *unstable* if the tiniest change to the starting data makes it disappear. See [[Navier-Stokes Smoothness Problem]] and [[Tristan Buckmaster]].

### Smooth
Informally: having derivatives of all orders, with no jumps or kinks. See [[Navier-Stokes Smoothness Problem]].

## V

### Vector field
A rule that attaches an arrow (a vector) to every point in space, like wind speed and direction on a weather map. See [[CalcPlot3D]].

## W

### Weak solution
A looser kind of solution to a differential equation. It only has to satisfy the equation "on average" (after integrating against test functions), so it may have kinks or jumps where derivatives do not exist. Weak solutions of fluid equations can be strangely non-unique; see [[Tristan Buckmaster]].
