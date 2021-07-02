---
toc: false
layout: post
description: Essence
categories: [essence, classification, medical, ultrasound, scientific reports]
title: Evaluation of Deep Convolutional Neural Networks for Automatic Classification of Common Maternal Fetal Ultrasound Planes
---

Burgos-Artizzu, X.P., Coronado-Gutiérrez, D., Valenzuela-Alcaraz, B., Bonet-Carne, E., Eixarch, E., Crispi, F. and Gratacós, E.  
Scientific Reports 2020

Paper - [Scientific Reports](https://www.nature.com/articles/s41598-020-67076-5)  
Data - [Zenodo](https://zenodo.org/record/3904280#.YN9mshMzZhE)


## Contribution
- The collection of a large maternal-fetal ultrasound image dataset comprised of more than twelve thousand 
  images from 1,792 patients in a real clinical setting. The dataset is publicly available.
- The direct comparison between deep learning techniques and the classification performed by research technicians
  who perform the task daily in our hospitals.
  
## Results
- Results on general classification show that computational model was able to classify US images almost on par
  with research technicians fully trained to perform the task.
- Results on brain fne-grained categorization show that computational models are still far from human technicians
  on this (much harder) task, where small details make all the difference.
- A computational model learned using exclusively images from one operator or US machine cannot be 
  directly transferred to images from other operators or US machines.  

![]({{ site.baseurl }}/images/2021-06-30-burgos-artizzu-fetal-uls-planes-classification/general_results.png)  

![]({{ site.baseurl }}/images/2021-06-30-burgos-artizzu-fetal-uls-planes-classification/fine_grained_results.png)