---
toc: false
layout: post
description: Paper summary
categories: [image_restoration, disentanglement, cvpr]
title: Learning Invariant Representation for Unsupervised Image Restoration
---

# Learning Invariant Representation for Unsupervised Image Restoration

Du, W., Chen, H. and Yang, H.  
In Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition 2020.

## Main contribution
Learn disentangled intermediate representations of noise and content from noisy inputs
and reconstruct clean observations.

## Technical details
![](2021-05-24-du-unsupevised-image-restoration/method_overview.png)  

### Loss functions
1. $mathcal{L}$