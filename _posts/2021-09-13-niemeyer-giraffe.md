---
toc: false
layout: post
description: Summary
categories: [summary, image synthesis, cvpr]
title: GIRAFFE Representing Scenes as Compositional Generative Neural Feature Fields
---

Niemeyer, M. and Geiger, A.  
In Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition 2021

Paper - [CVF](https://openaccess.thecvf.com/content/CVPR2021/papers/Niemeyer_GIRAFFE_Representing_Scenes_As_Compositional_Generative_Neural_Feature_Fields_CVPR_2021_paper.pdf)  
Code - [GitHub](https://github.com/autonomousvision/giraffe)


## Contribution

The paper proposes method to train the model for generating photorealistic scenes when training on unstructured image collection.
The method is based on Neural Radiance Fields (NeRF).  

**Canonical form** of feature field is generated **separately** for each object in the scene as well as for background.
**Separate** feature fields are farther **transformed** using affine transformation and **merged** in single feature field representing entire scene. 

This **compositional** scene representation allows controlling pose, appearance and shape of **individual** objects.

![]({{ site.baseurl }}/images/2021-07-06-post/contribution.png)


## Problem Description


## Method


## Results

### Experiment_1

### Experiment_2

### Experiment_3

### Ablation study


