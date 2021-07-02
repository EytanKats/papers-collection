---
toc: false
layout: post
description: Essence
categories: [essence, representation learning, fine tuning, preprint]
title: Big Transfer (BiT) General Visual Representation Learning
---

Kolesnikov, A., Beyer, L., Zhai, X., Puigcerver, J., Yung, J., Gelly, S. and Houlsby, N.  
arXiv 2019

Paper - [arXiv](https://arxiv.org/abs/1912.11370)  
Code - [GitHub](https://github.com/google-research/big_transfer)


## Contribution
- Study of the importance of dataset size and architecture size (during pre-training) in the context of transfer learning,
including transfer to tasks with very few datapoints.
- Procedure for training from large datasets.
- Simple fine-tuning protocol that applies to many diverse downstream tasks and yields good performance on all of these tasks.

![]({{ site.baseurl }}/images/2021-06-25-kolesnikov-big-transfer/transfer_performance.png)