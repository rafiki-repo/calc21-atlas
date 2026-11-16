---
type: application
status: draft
updated: 2026-11-16
last_checked: 2026-11-16
tags: [machine-learning, chain-rule, derivatives, gradient]
sources: [3blue1brown.com]
---

# Backpropagation and the Chain Rule

**Hook:** Every time a neural network "learns", it is running a first-year calculus rule millions of times over. Modern AI is built on the **chain rule**.

## The idea

A neural network is a long chain of simple functions: multiply by weights, add a bias, squash through a nonlinear function, repeat. At the end, a **cost** measures how wrong the output is.

To improve, the network needs to know **how sensitive the cost is to each weight**. That is a [[Glossary#Partial derivative|partial derivative]]. Because the weight affects the cost only *through* a chain of intermediate steps, the derivative is a **product of local rates of change**:

$$\frac{\partial C}{\partial w} = \frac{\partial z}{\partial w}\cdot\frac{\partial a}{\partial z}\cdot\frac{\partial C}{\partial a}$$

(weight → weighted sum *z* → activation *a* → cost *C*). That is the chain rule from a calculus course, written for one link in the chain.

**Backpropagation** is the bookkeeping trick. It starts at the output and works *backward*, reusing each computed rate for the layer before. Collect all those partial derivatives and you have the [[Glossary#Gradient|gradient]]. Then **gradient descent** nudges every weight a little way downhill, and the process repeats.

## Worth noticing

- **Errors drive learning.** The output-layer derivative is proportional to the gap between the actual and the desired output, so big mistakes produce big corrections.
- **Many paths add up.** A neuron deep in the network affects the cost through many routes. The chain rule sums over all of them.
- **Nobody does this by hand.** Software libraries compute these derivatives automatically (*automatic differentiation*). The calculus is still the engine.

## Go deeper

- [Backpropagation calculus](https://3blue1brown.com/lessons/backpropagation-calculus), 3Blue1Brown (Grant Sanderson): the chain-rule version, built up from a one-neuron-per-layer network. Free video and text.

## Next stop

- [[Grant Sanderson]]: the explainer behind that lesson
- [[Calculus and AI]]: what happens when AI is asked to *do* calculus
- [[Glossary#Chain rule]]
- [[Applications]]
