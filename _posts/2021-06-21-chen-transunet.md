---
toc: false
layout: post
description: Main contribution
categories: [main contribution, segmentation, transformer, medical, ct, mri, preprint]
title: TransUNet Transformers Make Strong Encoders for Medical Image Segmentation
---

Chen, J., Lu, Y., Yu, Q., Luo, X., Adeli, E., Wang, Y., Lu, L., Yuille, A.L. and Zhou, Y.  
arXiv 2021

[arXiv](https://arxiv.org/abs/2102.04306) [GitHub](https://github.com/Beckschen/TransUNet)


## Main contribution
Hybrid CNN-Transformer architecture in which Transformer block replaces the last convolution block in U-Net encoder.  
This architecture allows to leverage both detailed high-resolution spatial information from CNN features
and the global context encoded by Transformer.

![]({{ site.baseurl }}/images/2021-06-21-chen-transunet/architecture.png)