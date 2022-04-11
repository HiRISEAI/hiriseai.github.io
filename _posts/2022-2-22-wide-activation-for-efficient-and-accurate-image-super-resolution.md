---
layout: post
title:  "Wide Activation for Efficient and Accurate Image Super-Resolution"
date: 2022-2-22
image: assets/images/ESP_011264_1090_0_5.jpg
tags: [ AI, MinLab ]
---

[Wide Activation for Efficient and Accurate Image Super-Resolution](https://arxiv.org/abs/1808.08718){:target="_blank"}  

**Published in**:   
CVPR 2018 

**Authors**:   
Jiahui Yu, Yuchen Fan, Jianchao Yang, Ning Xu, Zhaowen Wang, Xinchao Wang, Thomas Huang 

**Abstract**:   
In this report we demonstrate that with same parameters and computational budgets, models with wider features before ReLU activation have significantly better performance for single image super-resolution (SISR). The resulted SR residual network has a slim identity mapping pathway with wider (\(2\times\) to \(4\times\)) channels before activation in each residual block. To further widen activation (\(6\times\) to \(9\times\)) without computational overhead, we introduce linear low-rank convolution into SR networks and achieve even better accuracy-efficiency tradeoffs. In addition, compared with batch normalization or no normalization, we find training with weight normalization leads to better accuracy for deep super-resolution networks. Our proposed SR network \textit{WDSR} achieves better results on large-scale DIV2K image super-resolution benchmark in terms of PSNR with same or lower computational complexity. Based on WDSR, our method also won 1st places in NTIRE 2018 Challenge on Single Image Super-Resolution in all three realistic tracks. Experiments and ablation studies support the importance of wide activation for image super-resolution.

**Code**:
[https://github.com/JiahuiYu/wdsr_ntire2018](https://github.com/JiahuiYu/wdsr_ntire2018){:target="_blank"}