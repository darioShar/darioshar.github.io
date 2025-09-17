---
title: "Denoising Levy Probabilistic Models (DLPM)"
collection: mini_projects
category: preprints
permalink: /mini-projects/2024-07-26-DLPM
excerpt: 'This paper introduces a novel framework to use heavy-tailed noise in the denoising diffusion paradigm, which constitutes a generalization of the original DDPM method. Using heavy-tailed noise is shown to bring benefits in various contexts: heavy-tailed data distributions, better robustness to class imbalance, and smaller computational time.'
date: 2024-07-26
venue: 'arxiv'
slidesurl: '/files/DLPM_Presentation.pdf' # 'http://academicpages.github.io/files/slides1.pdf'
paperurl: 'https://arxiv.org/abs/2407.18609'
author: 'Shariatian, D., Simsekli, U., & Durmus, A.O. (2024). Denoising Lévy Probabilistic Models. ArXiv, abs/2407.18609.'
---

Investigating noise distribution beyond Gaussian in diffusion generative models is an open problem. The Gaussian case has seen success experimentally and theoretically, fitting a unified SDE framework for score-based and denoising formulations. Recent studies suggest heavy-tailed noise distributions can address mode collapse and manage datasets with class imbalance, heavy tails, or outliers. Yoon et al. (NeurIPS 2023) introduced the Lévy-Ito model (LIM), extending the SDE framework to heavy-tailed SDEs with $\alpha$-stable noise. Despite its theoretical elegance and performance gains, LIM's complex mathematics may limit its accessibility and broader adoption. This study takes a simpler approach by extending the denoising diffusion probabilistic model (DDPM) with $\alpha$-stable noise, creating the denoising Lévy probabilistic model (DLPM). Using elementary proof techniques, we show DLPM reduces to running vanilla DDPM with minimal changes, allowing the use of existing implementations with minimal changes. DLPM and LIM have different training algorithms and, unlike the Gaussian case, they admit different backward processes and sampling algorithms. Our experiments demonstrate that DLPM achieves better coverage of data distribution tail, improved generation of unbalanced datasets, and faster computation times with fewer backward steps.
