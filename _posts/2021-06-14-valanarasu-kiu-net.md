---
toc: false
layout: post
description: Summary
categories: [segmentation, medical, ultrasound, histopathology, retinal images, miccai]
title: KiU-Net Towards Accurate Segmentation of Biomedical Images Using Over-complete Representations
---

Valanarasu, J.M.J., Sindagi, V.A., Hacihaliloglu, I. and Patel, V.M.  
In International Conference on Medical Image Computing and Computer-Assisted Intervention 2020

[arXiv](https://arxiv.org/abs/2006.04878) [GitHub](https://github.com/jeya-maria-jose/KiU-Net-pytorch)


## Main contribution
Paper proposes a novel architecture combining the features of both under-complete and over-complete deep networks.  
This architecture captures finer details better than the standard encoder-decoder architecture of U-Net
thus aiding in precise segmentation.


## Intuition
The standard encoder-decoder architecture of U-Net belongs to the family of under-complete convolution auto-encoders.
The increasing receptive field size over the depth of the network constrains it to focus more
on the higher-level features.  
However, it is important to note that tiny structures require smaller receptive fields.  
In over-complete architectures the data is projected onto a higher dimension in the intermediate layers.
The filters in this type of architecture learn finer low-level features due to the decreasing size
of receptive field as we go deeper in the encoder network.
![]({{ site.baseurl }}/images/2021-06-14-valanarasu-kiu-net/receptive_field.png)


## Technical details

### Architecture
Model (KiU-Net) consists of two branches when one of them is an over-complete network (KiNet)
and other - under-complete network (UNet).  
Features from two branches combined at each block level by cross residual fusion block (CRFB).
This block extracts complementary features from both network branches and forwards to both of them respectively.  
Finally, the features from both branches are added and forwarded through 1x1 convolution layer
to produce the segmentation mask.

![]({{ site.baseurl }}/images/2021-06-14-valanarasu-kiu-net/architecture.png)


## Results

### Filter responses

![]({{ site.baseurl }}/images/2021-06-14-valanarasu-kiu-net/filter_responses.png)

### 2D Ultrasound brain scans of preterm neonates
The dataset was collected during the study.
Ventricles and septum pellecudi were manually annotated by an expert ultrasonographer.

Qualitative comparison:  
![]({{ site.baseurl }}/images/2021-06-14-valanarasu-kiu-net/us_dataset_qualitative_results.png)

Quantitative comparison:  
![]({{ site.baseurl }}/images/2021-06-14-valanarasu-kiu-net/us_dataset_quantitative_results.png)

### GLAnd Segmentation (GLAS) dataset
GLAnd Segmentation (GLAS) dataset contains microscopic images of Hematoxylin and Eosin (H&E) stained slides
and the corresponding ground truth annotations by expert pathologists.

Qualitative comparison:  
![]({{ site.baseurl }}/images/2021-06-14-valanarasu-kiu-net/glas_dataset_qualitative_results.png)

Quantitative comparison:  
![]({{ site.baseurl }}/images/2021-06-14-valanarasu-kiu-net/glas_dataset_quantitative_results.png)

### Retinal Images vessel Tree Extraction (RITE) dataset:
RITE dataset contains segmentation of arteries and veins on retinal fundus images.

Qualitative comparison:  
![]({{ site.baseurl }}/images/2021-06-14-valanarasu-kiu-net/rite_dataset_qualitative_results.png)

Quantitative comparison:  
![]({{ site.baseurl }}/images/2021-06-14-valanarasu-kiu-net/rite_dataset_quantitative_results.png)

### Ablation study

![]({{ site.baseurl }}/images/2021-06-14-valanarasu-kiu-net/ablation_study.png)

UC - Under-Complete architecture  
OC - Over-Complete architecture  
SK - SKip connections

