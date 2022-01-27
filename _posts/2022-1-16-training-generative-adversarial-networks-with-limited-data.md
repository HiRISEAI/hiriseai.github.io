---
layout: post
title:  "Training Generative Adversarial Networks with Limited Data"
date: 2022-1-16
image: assets/images/s3.png
tags: [ AI ]
---

[Training Generative Adversarial Networks with Limited Data](https://arxiv.org/pdf/2006.06676.pdf){:target="_blank"}

**Published in**:   
CVPR 2020

**Authors**:   
Tero Karras, Miika Aittala, Janne Hellsten, Samuli Laine, Jaakko Lehtinen, Timo Aila

**Abstract**:   
Training generative adversarial networks (GAN) using too little data typically leads to discriminator overfitting, causing training to diverge. We propose an adaptive discriminator augmentation mechanism that significantly stabilizes training in limited data regimes. The approach does not require changes to loss functions or network architectures, and is applicable both when training from scratch and when fine-tuning an existing GAN on another dataset. We demonstrate, on several datasets, that good results are now possible using only a few thousand training images, often matching StyleGAN2 results with an order of magnitude fewer images. We expect this to open up new application domains for GANs. We also find that the widely used CIFAR-10 is, in fact, a limited data benchmark, and improve the record FID from 5.59 to 2.42. 