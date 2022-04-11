---
layout: post
title:  "Deep Learning-Driven Detection and Mapping of Rockfalls on Mars"
date: 2022-1-20
image: assets/images/rockfall.png
tags: [ AI, MinLab ]
---

**Published in**:   
IEEE JOURNAL OF SELECTED TOPICS IN APPLIED EARTH OBSERVATIONS AND REMOTE SENSING, VOL. 13, 2020

**Authors**:   
Valentin Tertius Bickel, Susan J. Conway, Pierre-Antoine Tesson, Andrea Manconi, Simon Loew, and Urs Mall

**Abstract**:   
The analysis of rockfall distribution and magnitude is a useful tool to study the past and current endogenic and exo- genic activity of Mars. At the same time, tracks left by rockfalls provide insights into the mechanical properties of the Martian surface. While a wealth of high-resolution spaceborne image data are available, manual mapping of displaced boulders with tracks is inefficient and slow, resulting in: 1) a small total number of mapped features; 2) inadequate statistics; and 3) a suboptimal utilization of the available big data. This study implements a deep learning-driven approach to automatically detect and map Martian boulders with tracks in high resolution imaging science experiment (HiRISE) imagery. Six off-the-shelf neural networks have been trained either on Martian or lunar rockfall data, or a combination of both, and are able to achieve a maximum overall recall of up to 0.78 and a maximum overall precision of up to 1.0, with a mean average precision of 0.71. The fusion of training data from different planets and sensors results in an increased detection precision, highlighting the value of domain generalization and multidomain learning. Average processing time per HiRISE image is ∼45 s using an NVIDIA Titan Xp, which is more than one order of magnitude faster than a human operator. The developed deep learning-driven infrastructure can be deployed to map Martian rockfalls on a global scale and within a realistic timeframe.