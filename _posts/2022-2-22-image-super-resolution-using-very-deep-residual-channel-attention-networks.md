---
layout: post
title:  "Image Super-Resolution Using Very Deep Residual Channel Attention Networks"
date: 2022-2-22
image: assets/images/yulun.png
tags: [ imagery, AI ]
---

[Image Super-Resolution Using Very Deep Residual Channel Attention Networks](https://arxiv.org/pdf/1807.02758.pdf){:target="_blank"}  

**Published in**:   
ECCV 2018 

**Authors**:   
Yulun Zhang, Kunpeng Li, Kai Li, Lichen Wang, Bineng Zhong, Yun Fu

**Abstract**:   
Convolutional neural network (CNN) depth is of crucial importance for image super-resolution (SR). However, we observe that deeper networks for image SR are more difficult to train. The low-resolution inputs and features contain abundant low-frequency information, which is treated equally across channels, hence hindering the representational ability of CNNs. To solve these problems, we propose the very deep residual channel attention networks (RCAN). Specifically, we propose a residual in residual (RIR) structure to form very deep network, which consists of several residual groups with long skip connections. Each residual group contains some residual blocks with short skip connections. Meanwhile, RIR allows abundant low-frequency information to be bypassed through multiple skip connections, making the main network focus on learning high-frequency information. Furthermore, we propose a channel attention mechanism to adaptively rescale channel-wise features by considering interdependencies among channels. Extensive experiments show that our RCAN achieves better accuracy and visual improvements against state-of-the-art methods.  

**Code**:
[https://github.com/yulunzhang/RCAN](https://github.com/yulunzhang/RCAN){:target="_blank"}