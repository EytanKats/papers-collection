---
toc: false
layout: post
description: Essence
categories: [essence, detection, classification, medical, ultrasound, miccai]
title: Computer-Aided Tumor Diagnosis in Automated Breast Ultrasound using 3D Detection Network
---

Yu, J., Chen, C., Yang, X., Wang, Y., Yan, D., Zhang, J. and Ni, D.  
In International Conference on Medical Image Computing and Computer-Assisted Intervention 2020

Paper - [arXiv](https://arxiv.org/abs/2007.16133)

## Contribution 
- 3D Region Proposal Network (RPN) to simultaneously detect and classify breast lesions in Automated Breast Ultrasound (ABUS) images.
- Intersection-over-Union (IoU) balanced classification loss to enlarge contribution of detections with good regression to learning process comparing to those with bad regression.
- Similarity loss between feature vectors corresponding to detections to increase intra-category correlation and inter-category discrimination.

![]({{ site.baseurl }}/images/2021-06-24-yu-tumor-diagnosis-in-breast-ultrasound/architecture.png)
