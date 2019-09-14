---
title: "Unified Probabilistic Deep Continual Learning through Generative Replay and Open Set Recognition"
collection: publications
permalink: /publication/6/
excerpt: "We introduce a unified probabilistic approach for deep continual learning based on variational Bayesian inference with open set recognition. Our model combines a probabilistic encoder with a generative model and a generative linear classifier that get shared across tasks. The open set recognition bounds the approximate posterior by fitting regions of high density on the basis of correctly classified data points and balances open-space risk with recognition errors. Catastrophic inference for both generative models is significantly alleviated through generative replay, where the open set recognition is used to sample from high density areas of the class specific posterior and reject statistical outliers. Our approach naturally allows for forward and backward transfer while maintaining past knowledge without the necessity of storing old data, regularization or inferring task labels. We demonstrate compelling results in the challenging scenario of incrementally expanding the single-head classifier for both class incremental visual and audio classification tasks, as well as incremental learning of datasets across modalities."
date: 2019-05-28
venue: 'Somewhere'
paperurl: 'https://arxiv.org/abs/1905.12019'

citation: 'Martin Mundt, <b>Sagnik Majumder</b>, Iuliia Pliushch, Visvanathan Ramesh, &quot;Unified Probabilistic Deep Continual Learning through Generative Replay and Open Set Recognition&quot; In: ArXiv.
'

<!-- #  <i>Published in ICCV SDLCV 2019, Seoul, South Korea</i>.
 -->
 ---
Abstract: We introduce a unified probabilistic approach for deep continual learning based on variational Bayesian inference with open set recognition. Our model combines a probabilistic encoder with a generative model and a generative linear classifier that get shared across tasks. The open set recognition bounds the approximate posterior by fitting regions of high density on the basis of correctly classified data points and balances open-space risk with recognition errors. Catastrophic inference for both generative models is significantly alleviated through generative replay, where the open set recognition is used to sample from high density areas of the class specific posterior and reject statistical outliers. Our approach naturally allows for forward and backward transfer while maintaining past knowledge without the necessity of storing old data, regularization or inferring task labels. We demonstrate compelling results in the challenging scenario of incrementally expanding the single-head classifier for both class incremental visual and audio classification tasks, as well as incremental learning of datasets across modalities.

[Download paper here](https://arxiv.org/pdf/1905.12019.pdf)