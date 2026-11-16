---
type: application
status: draft
updated: 2026-11-16
last_checked: 2026-11-16
tags: [physics, pde, numerical-methods, machine-learning, history]
sources: [metoffice.gov.uk, ecmwf.int, arxiv.org]
---

# Weather Forecasting

**Hook:** A weather forecast is a set of differential equations, stepped forward in time. One man tried it by hand in 1922. A century later, machine-learning models trained on those equations' output are being run alongside them.

## The idea

The atmosphere is a fluid, so it obeys the [[Glossary#Partial differential equation (PDE)|partial differential equations]] of fluid flow and heat (close cousins of the equations in the [[Navier-Stokes Smoothness Problem]]). Nobody can solve them exactly. Instead, forecasters:

1. Cover the globe with a grid of points and measure the current state at each one.
2. Use the equations to estimate the **rate of change** at each point.
3. Step forward a few minutes, then repeat thousands of times.

This is **Euler's method** in spirit: a [[Glossary#Derivative|derivative]] used as a short-range predictor ("next value ≈ current value + rate × time step"), repeated at enormous scale.

## Three moments

- **1922: the hand-cranked forecast.** Lewis Fry Richardson published *Weather Prediction by Numerical Process*. According to the UK Met Office, his trial took **more than six weeks** to produce a six-hour forecast for one location, and it was inaccurate because of data limitations. He imagined a "forecast factory" of about **64,000 human computers** in a great hall, each calculating one patch of the world.
- **After World War II: machines take over.** Electronic computers made his method practical, and it is the basis of today's physics-based forecasting.
- **2025-26: learning from the equations.** On 25 Feb 2025, the European Centre for Medium-Range Weather Forecasts (ECMWF) made its machine-learning model **AIFS** operational, running alongside its physics-based model (IFS). AIFS is trained on decades of past atmospheric data produced with physics models. ECMWF reports gains of up to 20% on some measures (including cyclone tracks) and about 1,000 times less energy per forecast. Its own technical paper also lists weak spots: forecasts blur at longer lead times and cyclone intensity is underestimated. ECMWF calls the two systems "complementary". In May 2026 it stopped running four external AI models (including Google DeepMind's GraphCast), saying they had been overtaken by newer ones.

## Go deeper

- [Celebrating 100 years of scientific forecasting](https://www.metoffice.gov.uk/about-us/who/our-history/celebrating-100-years-of-scientific-forecasting), UK Met Office: Richardson's story
- [ECMWF's AI forecasts become operational](https://www.ecmwf.int/en/about/media-centre/news/2025/ecmwfs-ai-forecasts-become-operational), ECMWF news (Feb 2025)
- [AIFS: ECMWF's data-driven forecasting system](https://arxiv.org/abs/2406.01465), arXiv preprint (2024): design, scores, and limitations
- [Farewell to the external AI models](https://www.ecmwf.int/en/about/media-centre/aifs-blog/2026/farewell-external-ai-models), ECMWF blog (May 2026)

## Next stop

- [[Navier-Stokes Smoothness Problem]]: the fluid equations mathematicians still can't fully tame
- [[Backpropagation and the Chain Rule]]: how models like AIFS learn
- [[SIR Epidemic Model]]: forecasting outbreaks instead of storms
- [[Applications]]
