---
layout: post
title:  "Projected GANs Converge Faster"
date: 2022-2-27
image: assets/images/ESP_011326_1700_000001.jpg
tags: [ AI, MinLab, articles ]
---

[Projected GANs Converge Faster](https://arxiv.org/pdf/2111.01007.pdf){:target="_blank"}  

**Published in**:   
NeurIPS 2021 

**Authors**:   
Axel Sauer, Kashyap Chitta, Jens Müller, Andreas Geiger

**Abstract**:   
Generative Adversarial Networks (GANs) produce high-quality images but are challenging to train. They need careful regularization, vast amounts of compute, and expensive hyper-parameter sweeps. We make significant headway on these issues by projecting generated and real samples into a fixed, pretrained feature space. Motivated by the finding that the discriminator cannot fully exploit features from deeper layers of the pretrained model, we propose a more effective strategy that mixes features across channels and resolutions. Our Projected GAN improves image quality, sample efficiency, and convergence speed. It is further compatible with resolutions of up to one Megapixel and advances the state-of-the-art Fréchet Inception Distance (FID) on twenty-two benchmark datasets. Importantly, Projected GANs match the previously lowest FIDs up to 40 times faster, cutting the wall-clock time from 5 days to less than 3 hours given the same computational resources. 

**Code**:
[https://github.com/autonomousvision/projected_gan](https://github.com/autonomousvision/projected_gan){:target="_blank"}