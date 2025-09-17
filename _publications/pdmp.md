---
title: "Piecewise Deterministic Generative Models"
collection: publications
category: conferences
permalink: /publication/2024-07-28-PDMP
excerpt: 'We introduce a novel class of generative models based on piecewise deterministic Markov processes (PDMPs), which combine deterministic motion with random jumps. Like diffusions, PDMPs can be reversed in time. We derive explicit expressions for jump rates and kernels in the time-reversed processes and propose efficient training methods and approximate simulation techniques. Additionally, we provide bounds on the total variation distance between the data and model distributions, supported by promising numerical simulations.'
date: 2024-07-26
venue: NeurIPS 2024
slidesurl: # 'http://academicpages.github.io/files/slides1.pdf'
paperurl: 'https://arxiv.org/abs/2407.19448'
github: 'https://github.com/darioShar/PDMP'
author: 'Bertazzi A., Shariatian D., Durmus A.O., Simsekli U., Moulines É.'
---

We introduce a novel class of generative models based on piecewise deterministic Markov processes (PDMPs), a family of non-diffusive stochastic processes consisting of deterministic motion and random jumps at random times. Similarly to diffusions, such Markov processes admit time reversals that turn out to be PDMPs as well. We apply this observation to three PDMPs considered in the literature: the Zig-Zag process, Bouncy Particle Sampler, and Randomised Hamiltonian Monte Carlo. For these three particular instances, we show that the jump rates and kernels of the corresponding time reversals admit explicit expressions depending on some conditional densities of the PDMP under consideration before and after a jump. Based on these results, we propose efficient training procedures to learn these characteristics and consider methods to approximately simulate the reverse process. Finally, we provide bounds in the total variation distance between the data distribution and the resulting distribution of our model in the case where the base distribution is the standard d-dimensional Gaussian distribution. Promising numerical simulations support further investigations into this class of models.