---
toc: false
layout: post
description: Essence
categories: [essence, representation learning, fine tuning, classification, transformer, iclr]
title: An Image is Worth 16x16 Words Transformers for Image Recognition at Scale
---

Dosovitskiy, A., Beyer, L., Kolesnikov, A., Weissenborn, D., Zhai, X., Unterthiner, T., Dehghani, M., Minderer, M.,
Heigold, G., Gelly, S., Uszkoreit, J. and Houlsby, N.  
In International Conference on Learning Representations 2020

Paper - [arXiv](https://arxiv.org/abs/2010.11929)  
Code - [GitHub](https://github.com/google-research/vision_transformer)


## Contribution
- Application of Transformers to image recognition.
- Image is interpreted as a sequence of patches and processed by a standard Transformer encoder as used in NLP.
- No image-specific inductive biases are introduced into the architecture apart from the initial patch extraction step.

## Results
- When trained on mid-sized datasets such as ImageNet Vision Transformers yield modest accuracies
  of a few percentage points below ResNets of comparable size.
- When pre-trained at sufficient scale Vision Transformer matches or exceeds the state of the art on many 
  image classification datasets, while been relatively cheap to pre-train.
  
![]({{ site.baseurl }}/images/2021-07-06-dosovitskiy-vit/model_overview.png)