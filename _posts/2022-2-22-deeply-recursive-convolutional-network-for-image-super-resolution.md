---
layout: post
title:  "Deeply-Recursive Convolutional Network for Image Super-Resolution"
date: 2022-2-22
image: assets/images/deeply.png
tags: [ imagery, AI ]
---

[Deeply-Recursive Convolutional Network for Image Super-Resolution](https://arxiv.org/pdf/1511.04491.pdf){:target="_blank"}  

**Published in**:   
CVPR 2016 Oral

**Authors**:   
Jiwon Kim, Jung Kwon Lee, Kyoung Mu Lee

**Abstract**:   
We propose an image super-resolution method (SR) using a deeply-recursive convolutional network (DRCN). Our network has a very deep recursive layer (up to 16 recursions). Increasing recursion depth can improve performance without introducing new parameters for additional convolutions. Albeit advantages, learning a DRCN is very hard with a standard gradient descent method due to exploding/vanishing gradients. To ease the difficulty of training, we propose two extensions: recursive-supervision and skip-connection. Our method outperforms previous methods by a large margin. 

**Code**:
[https://github.com/jiny2001/deeply-recursive-cnn-tf](https://github.com/jiny2001/deeply-recursive-cnn-tf){:target="_blank"}