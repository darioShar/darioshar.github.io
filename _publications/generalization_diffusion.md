---
title: "Algorithm and Data Dependent Generalization Bounds for Score-Based Generative Models"
collection: publications
category: conferences
permalink: /publication/2025-09-19-Generalization
excerpt: 'This paper studies the generalization property of diffusion models through the lens of statistical learning. We develop a perspective that enables using existing tools to characterize the generalization ability of these generative models.'
date: 2025-09-19
venue: NeurIPS 2025
# slidesurl: '/files/DLPM_Presentation.pdf' # 'http://academicpages.github.io/files/slides1.pdf'
paperurl: 'https://www.arxiv.org/abs/2506.03849'
github: 'https://github.com/darioShar/GeneralizationDiffusion'
author: 'Shariatian D.*, Dupuis B.*, Haddouche M.*, Durmus A.O., Simsekli U.'
---

Score-based generative models (SGMs) have emerged as one of the most popular classes of generative models. A substantial body of work now exists on the analysis of SGMs, focusing either on discretization aspects or on their statistical performance. In the latter case, bounds have been derived, under various metrics, between the true data distribution and the distribution induced by the SGM, often demonstrating polynomial convergence rates with respect to the number of training samples. However, these approaches adopt a largely approximation theory viewpoint, which tends to be overly pessimistic and relatively coarse. In particular, they fail to fully explain the empirical success of SGMs or capture the role of the optimization algorithm used in practice to train the score network. To support this observation, we first present simple experiments illustrating the concrete impact of optimization hyperparameters on the generalization ability of the generated distribution. Then, this paper aims to bridge this theoretical gap by providing the first algorithmic- and data-dependent generalization analysis for SGMs. In particular, we establish bounds that explicitly account for the optimization dynamics of the learning algorithm, offering new insights into the generalization behavior of SGMs. Our theoretical findings are supported by empirical results on several datasets.
