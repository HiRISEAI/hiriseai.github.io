---
layout: post
title:  "Image Super-Resolution via Deep Recursive Residual Network"
date: 2022-2-22
image: assets/images/ESP_011268_2485_000019.jpg
tags: [ imagery, AI ]
---

[Image Super-Resolution via Deep Recursive Residual Network](http://cvlab.cse.msu.edu/pdfs/Tai_Yang_Liu_CVPR2017.pdf){:target="_blank"}  

**Published in**:   
CVPR 2017

**Authors**:   
Ying Tai, Jian Yang, Xiaoming Liu

**Abstract**:   
Recently, Convolutional Neural Network (CNN) based models have achieved great success in Single Image Super-Resolution (SISR). Owing to the strength of deep networks, these CNN models learn an effective nonlinear mapping from the low-resolution input image to the high-resolution target image, at the cost of requiring enormous parameters. This paper proposes a very deep CNN model (up to 52 convolutional layers) named Deep Recursive Residual Network (DRRN) that strives for deep yet concise networks. Specifically, residual learning is adopted, both in global and local manners, to mitigate the difficulty of training very deep networks, recursive learning is used to control the model parameters while increasing the depth. Extensive benchmark evaluation shows that DRRN significantly outperforms state of the art in SISR, while utilizing far fewer parameters. 

**Code**:
[https://github.com/tyshiwo/DRRN_CVPR17](https://github.com/tyshiwo/DRRN_CVPR17){:target="_blank"}