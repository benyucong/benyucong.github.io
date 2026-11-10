---
title: "How Much Training-Inference Mismatch Can On-Policy Distillation Tolerate?"
collection: publications
authors: 'Cong Yu, Ziting Wang, Songlin Jiang, Sitong Zhang, Chengliang Chai, Youhe Jiang, Eiko Yoneki, Tuo Shi'
permalink: /publication/2026-11-08-OPD-Mismatch
date: 2026-11-08
venue: 'arXiv preprint'
paperurl: 'https://arxiv.org/abs/2611.11450'
---

On-policy distillation (OPD) trains a student language model on its own responses under a fixed teacher, but the quantized inference and asynchronous rollouts used to make this affordable introduce a training-inference mismatch between the rollout engine and the model being trained. We investigate how much mismatch OPD can tolerate, where its effects arise, and how training systems can exploit this tolerance, finding that OPD absorbs substantial mismatch before training quality degrades, revealing an empirical mismatch budget. We introduce a lightweight admission check that screens rollout configurations against a calibrated budget without a full training run, and model-specific FP8 recipes that preserve training quality while providing capacity for at least 1.93× as many KV-cache tokens as BF16; combined with asynchronous rollouts, FP8 reaches the same training quality 1.62× sooner than synchronous BF16.

**[Download paper](https://arxiv.org/pdf/2611.11450){:target="_blank"}**
