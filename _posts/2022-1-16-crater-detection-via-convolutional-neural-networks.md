---
layout: post
title:  Crater Detection iva Convolutional Neural Networks
date: 2022-1-16
image: assets/images/wei.png
tags: [ AI, craters ]
---

[Crater Detection via Convolutional Neural Networks](https://arxiv.org/abs/1601.00978){:target="_blank"}  
Joseph Paul Cohen, Henry Z. Lo, Tingting Lu, Wei Ding

*Submitted to 47th Lunar and Planetary Science Conference (LPSC 2016)*

**Abstract** Craters are among the most studied geomorphic features in the Solar System because they yield important information about the past and present geological processes and provide information about the relative ages of observed geologic formations. We present a method for automatic crater detection using advanced machine learning to deal with the large amount of satellite imagery collected. The challenge of automatically detecting craters comes from their is complex surface because their shape erodes over time to blend into the surface. Bandeira provided a seminal dataset that embodied this challenge that is still an unsolved pattern recognition problem to this day. There has been work to solve this challenge based on extracting shape and contrast features and then applying classification models on those features. The limiting factor in this existing work is the use of hand crafted filters on the image such as Gabor or Sobel filters or Haar features. These hand crafted methods rely on domain knowledge to construct. We would like to learn the optimal filters and features based on training examples. In order to dynamically learn filters and features we look to Convolutional Neural Networks (CNNs) which have shown their dominance in computer vision. The power of CNNs is that they can learn image filters which generate features for high accuracy classification. 