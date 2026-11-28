---
type: application
status: draft
updated: 2026-11-28
last_checked: 2026-11-28
tags: [machine-learning, stochastic-calculus, differential-equations, generative-ai]
sources: [arxiv.org (2011.13456, 2006.11239, 2112.10752), yang-song.net, github.com/CompVis]
---

# Diffusion Models

**Hook:** Many AI image generators work by taking a picture, dissolving it into static, and learning to run the film backwards. The "backwards" part is a stochastic differential equation.

## The idea

1. **Forward: add noise.** Take a real image and add a little random noise, over and over, until only static is left. Written as a continuous process, this is a **[[Glossary#Stochastic differential equation (SDE)|stochastic differential equation]]**: an ordinary drift plus random kicks, the same kind of equation as in [[Stochastic Calculus]].
2. **Backward: remove it.** A 1982 result by Anderson (cited by Song et al.) says the time-reversed process is also an SDE. The only thing it needs that you don't already know is the **score**: the [[Glossary#Gradient|gradient]] of the log-probability of the noisy images at each moment. Roughly, an arrow pointing toward "more like a real image."
3. **Learn the arrow.** Train a neural network to estimate the score, then start from fresh static and step the reverse SDE forward with a numerical solver, much like **Euler's method** with dice. Out comes a new image.

The same paper shows there is also a **non-random ODE** (the "probability flow") that turns noise into images along the same distributions, which allows exact likelihood calculations.

## The papers behind it

- **2020: DDPM.** Jonathan Ho, Ajay Jain, and Pieter Abbeel, "Denoising Diffusion Probabilistic Models" (arXiv preprint). Its abstract says the models are "inspired by considerations from nonequilibrium thermodynamics."
- **2021: the SDE view.** Yang Song and five co-authors, "Score-Based Generative Modeling through Stochastic Differential Equations" (ICLR 2021, oral). It unified earlier noise-and-denoise methods as discretizations of one SDE picture.
- **2022: making it cheap.** Robin Rombach and co-authors, "High-Resolution Image Synthesis with Latent Diffusion Models" (CVPR 2022), ran diffusion in a compressed "latent" space. The **Stable Diffusion** repository describes itself as a latent text-to-image diffusion model built on that work, with Stability AI and Runway.

## The fine print

The calculus is clean; the practice is engineering. Results depend heavily on network design, training data, and how the reverse equation is discretized. Image quality is reported with benchmark scores (FID, Inception score) that measure resemblance to training data, not correctness.

## Go deeper

- [Generative Modeling by Estimating Gradients of the Data Distribution](https://yang-song.net/blog/2021/score/), Yang Song's blog: the score, noise levels, and the reverse SDE, with animations. Free; assumes some probability.
- [Song et al. (2021) on arXiv](https://arxiv.org/abs/2011.13456): the primary paper.

## Next stop

- [[Stochastic Calculus]]: Itô's calculus for random paths, the language of step 1
- [[Backpropagation and the Chain Rule]]: how the score network gets trained
- [[Physics-Informed Neural Networks]]: another place where networks and differential equations meet
- [[Applications]]
