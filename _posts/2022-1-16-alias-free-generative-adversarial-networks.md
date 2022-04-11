---
layout: post
title:  "Alias-Free Generative Adversarial Networks"
date: 2022-1-16
image: assets/images/stylegan3.png
tags: [ AI, MinLab ]
---

[Alias-Free Generative Adversarial Networks](https://arxiv.org/pdf/2106.12423.pdf){:target="_blank"}

**Published in**:   
CVPR 2021 

**Authors**:   
Tero Karras, Miika Aittala, Samuli Laine, Erik Härkönen, Janne Hellsten, Jaakko Lehtinen, Timo Aila

**Abstract**:   
We observe that despite their hierarchical convolutional nature, the synthesis process of typical generative adversarial networks depends on absolute pixel coordinates in an unhealthy manner. This manifests itself as, e.g., detail appearing to be glued to image coordinates instead of the surfaces of depicted objects. We trace the root cause to careless signal processing that causes aliasing in the generator network. Interpreting all signals in the network as continuous, we derive generally applicable, small architectural changes that guarantee that unwanted information cannot leak into the hierarchical synthesis process. The resulting networks match the FID of StyleGAN2 but differ dramatically in their internal representations, and they are fully equivariant to translation and rotation even at subpixel scales. Our results pave the way for generative models better suited for video and animation. 
