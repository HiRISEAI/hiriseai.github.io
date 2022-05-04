---
layout: post
title:  "Towards Faster and Stabilized GAN Training for High-fidelity Few-shot Image Synthesis"
date: 2022-2-27
image: assets/images/ESP_011335_1005_000004.jpg
tags: [ AI, MinLab, articles ]
---

[Towards Faster and Stabilized GAN Training for High-fidelity Few-shot Image Synthesis](https://arxiv.org/pdf/2101.04775.pdf){:target="_blank"}  

**Published in**:   
ICLR 2021 

**Authors**:   
Bingchen Liu, Yizhe Zhu, Kunpeng Song, Ahmed Elgammal

**Abstract**:   
Training Generative Adversarial Networks (GAN) on high-fidelity images usually requires large-scale GPU-clusters and a vast number of training images. In this paper, we study the few-shot image synthesis task for GAN with minimum computing cost. We propose a light-weight GAN structure that gains superior quality on 1024*1024 resolution. Notably, the model converges from scratch with just a few hours of training on a single RTX-2080 GPU, and has a consistent performance, even with less than 100 training samples. Two technique designs constitute our work, a skip-layer channel-wise excitation module and a self-supervised discriminator trained as a feature-encoder. With thirteen datasets covering a wide variety of image domains (The datasets and code are available at: this https URL), we show our model's superior performance compared to the state-of-the-art StyleGAN2, when data and computing budget are limited. 

**Code**:
[https://github.com/odegeasslbc/FastGAN-pytorch](https://github.com/odegeasslbc/FastGAN-pytorch){:target="_blank"}