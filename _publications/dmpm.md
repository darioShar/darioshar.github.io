---
title: "Denoising Markov Probabilistic Models (DMPM)"
collection: publications
category: preprints
permalink: /publication/2025-02-11-DMPM
excerpt: 'This paper introduces a novel framework for discrete data generation on the hypercube $\{0, 1\}^d$. We establish theoretical and methodological alignment with classical continuous score-based modesls. We demonstrate the effectiveness of this approach on low and high dimensional datasets (Binary MNIST), beating other state-of-the-art methods like Discrete Flow Matching'
date: 2025-02-11
venue: Arxiv
# slidesurl: '/files/DLPM_Presentation.pdf' # 'http://academicpages.github.io/files/slides1.pdf'
paperurl: 'https://www.arxiv.org/abs/2502.07939'
github: 'https://github.com/darioShar/DMPM'
citation: 'Shariatian D., Pham L.T.N., Ocello A., Conforti G., Durmus A.O. (2025). Denoising Markov Probabilistic Models. ArXiv, abs/2502.07939.'
---

This paper introduces the Discrete Markov Probabilistic Model (DMPM), a novel algorithm for discrete data generation. The algorithm operates in the space of bits $\{0,1\}^d$, where the noising process is a continuous-time Markov chain that can be sampled exactly via a Poissonian clock that flips labels uniformly at random. The time-reversal process, like the forward noise process, is a jump process, with its intensity governed by a discrete analogue of the classical score function. Crucially, this intensity is proven to be the conditional expectation of a function of the forward process, strengthening its theoretical alignment with score-based generative models while ensuring robustness and efficiency. We further establish convergence bounds for the algorithm under minimal assumptions and demonstrate its effectiveness through experiments on low-dimensional Bernoulli-distributed datasets and high-dimensional binary MNIST data. The results highlight its strong performance in generating discrete structures. This work bridges theoretical foundations and practical applications, advancing the development of effective and theoretically grounded discrete generative modeling.