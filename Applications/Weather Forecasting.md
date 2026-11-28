---
type: application
status: draft
updated: 2026-11-28
last_checked: 2026-11-28
tags: [physics, pde, numerical-methods, machine-learning, history]
sources: [metoffice.gov.uk, ecmwf.int, arxiv.org, maths.ucd.ie]
---

# Weather Forecasting

**Hook:** A weather forecast is a set of differential equations, stepped forward in time. One man tried it by hand in 1922. A century later, machine-learning models trained on those equations' output are being run alongside them.

## The idea

The atmosphere is a fluid, so it obeys the [[Glossary#Partial differential equation (PDE)|partial differential equations]] of fluid flow and heat (close cousins of the equations in the [[Navier-Stokes Smoothness Problem]]). Nobody can solve them exactly. Instead, forecasters:

1. Cover the globe with a grid of points and measure the current state at each one.
2. Use the equations to estimate the **rate of change** at each point.
3. Step forward a few minutes, then repeat thousands of times.

This is **Euler's method** in spirit: a [[Glossary#Derivative|derivative]] used as a short-range predictor ("next value ≈ current value + rate × time step"), repeated at enormous scale.

## Four moments

- **1922: the hand-cranked forecast.** Lewis Fry Richardson published *Weather Prediction by Numerical Process*. According to the UK Met Office, his trial took **more than six weeks** to produce a six-hour forecast for one location, and it was inaccurate because of data limitations. He imagined a "forecast factory" of about **64,000 human computers** in a great hall, each calculating one patch of the world.
- **What went wrong, worked out decades later.** Richardson's test (using observations from 20 May 1910) predicted a surface pressure jump of **145 hPa in six hours**, a wildly unrealistic value. Peter Lynch (then at Met Éireann) rebuilt the calculation on a computer and reproduced the 145. He traced it to an imbalance between the starting winds and pressures, which sets off fast, spurious gravity waves. After smoothing the starting data ("initialization," with a digital filter), the same method gave a realistic change of about **3 hPa**. In Lynch's account, the method held up and the starting data were the problem.
- **After World War II: machines take over.** Electronic computers made his method practical, and it is the basis of today's physics-based forecasting.
- **2025-26: learning from the equations.** On 25 Feb 2025, the European Centre for Medium-Range Weather Forecasts (ECMWF) made its machine-learning model **AIFS** operational, running alongside its physics-based model (IFS). AIFS is trained on decades of past atmospheric data produced with physics models. ECMWF reports gains of up to 20% on some measures (including cyclone tracks) and about 1,000 times less energy per forecast. Its own technical paper also lists weak spots: forecasts blur at longer lead times and cyclone intensity is underestimated. ECMWF calls the two systems "complementary". In May 2026 it stopped running four external AI models (including Google DeepMind's GraphCast), saying they had been overtaken by newer ones.

## Go deeper

- [Celebrating 100 years of scientific forecasting](https://www.metoffice.gov.uk/about-us/who/our-history/celebrating-100-years-of-scientific-forecasting), UK Met Office: Richardson's story
- [Richardson's Marvellous Forecast](https://maths.ucd.ie/~plynch/Publications/RicMarFor_abs.html), Peter Lynch (1999, AMS volume): abstract of the re-run. The full story is in his book *The Emergence of Numerical Weather Prediction: Richardson's Dream* (Cambridge, 2006).
- [ECMWF's AI forecasts become operational](https://www.ecmwf.int/en/about/media-centre/news/2025/ecmwfs-ai-forecasts-become-operational), ECMWF news (Feb 2025)
- [AIFS: ECMWF's data-driven forecasting system](https://arxiv.org/abs/2406.01465), arXiv preprint (2024): design, scores, and limitations
- [Farewell to the external AI models](https://www.ecmwf.int/en/about/media-centre/aifs-blog/2026/farewell-external-ai-models), ECMWF blog (May 2026)

## Next stop

- [[Navier-Stokes Smoothness Problem]]: the fluid equations mathematicians still can't fully tame
- [[Backpropagation and the Chain Rule]]: how models like AIFS learn
- [[SIR Epidemic Model]]: forecasting outbreaks instead of storms
- [[PID Controller]]: derivatives used to look ahead, in machines instead of skies
- [[Applications]]
