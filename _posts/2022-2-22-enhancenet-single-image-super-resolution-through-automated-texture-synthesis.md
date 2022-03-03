---
layout: post
title:  "EnhanceNet: Single Image Super-Resolution Through Automated Texture Synthesis"
date: 2022-2-22
image: assets/images/enhancenet.png
tags: [ imagery, AI ]
---

[EnhanceNet: Single Image Super-Resolution Through Automated Texture Synthesis](https://arxiv.org/pdf/1612.07919.pdf){:target="_blank"}  

**Published in**:   
CVPR 2016 Oral

**Authors**:   
Mehdi S. M. Sajjadi, Bernhard Schölkopf, Michael Hirsch

**Abstract**:   
Single image super-resolution is the task of inferring a high-resolution image from a single low-resolution input. Traditionally, the performance of algorithms for this task is measured using pixel-wise reconstruction measures such as peak signal-to-noise ratio (PSNR) which have been shown to correlate poorly with the human perception of image quality. As a result, algorithms minimizing these metrics tend to produce over-smoothed images that lack high-frequency textures and do not look natural despite yielding high PSNR values.
We propose a novel application of automated texture synthesis in combination with a perceptual loss focusing on creating realistic textures rather than optimizing for a pixel-accurate reproduction of ground truth images during training. By using feed-forward fully convolutional neural networks in an adversarial training setting, we achieve a significant boost in image quality at high magnification ratios. Extensive experiments on a number of datasets show the effectiveness of our approach, yielding state-of-the-art results in both quantitative and qualitative benchmarks.  

**Code**:
[https://github.com/msmsajjadi/EnhanceNet-Code](https://github.com/msmsajjadi/EnhanceNet-Code){:target="_blank"}