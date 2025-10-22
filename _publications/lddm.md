---
title: "Latent Discrete Diffusion Models"
collection: publications
category: preprints
permalink: /publication/2025-10-18-LDDM
excerpt: 'Couples a masked discrete diffusion over tokens with a continuous latent process to preserve cross-token dependencies and improve few-step generation.'
date: 2025-10-18
paperurl: 'https://arxiv.org/abs/2510.18114'
author: 'Shariatian D., Durmus A., Peluchetti S.'
---

We study discrete diffusion for language and other categorical data and focus on a common limitation of masked denoisers: reverse transitions typically factorize across positions, which can weaken joint structure and degrade quality in few-step generation. We propose *Latent Discrete Diffusion Models* (LDDMs), which couple a masked discrete diffusion over tokens with a continuous diffusion over latent embeddings. The latent channel provides a softer signal and carries cross-token dependencies that help resolve ambiguities. We present two instantiations: (i) FUJI-LDDMs, which perform fully joint denoising of tokens and latents, and (ii) SEQ-LDDMs, which sequentially resolve the latent and then the discrete chain conditionally on it. For both variants we derive ELBO-style objectives and discuss design choices to learn informative latents yet amenable to diffusion modeling. In experiments, LDDMs yield improvements on unconditional generation metrics as compared to state-of-the-art masked discrete diffusion baselines, and are effective at lower sampling budgets, where unmasking many tokens per step is desirable.
