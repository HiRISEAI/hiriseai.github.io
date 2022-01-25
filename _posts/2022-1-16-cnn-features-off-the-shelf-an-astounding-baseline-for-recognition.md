---
layout: post
title: "CNN Features Off-the-shelf: An Astounding Baseline for Recognition"
date: 2022-1-16
image: assets/images/ESP_025124_1985_000005.jpg
tags: [ AI, more ]
---

**Published in**:   
Proceedings of the 2014 IEEE Conference on Computer Vision and Pattern Recognition Workshops, 512-519

**Authors**:   
Ali Sharif Razavian, Hossein Azizpour, Josephine Sullivan, Stefan Carlsson

**Abstract**:   
Recent results indicate that the generic descriptors extracted from the convolutional neural networks are very powerful. This paper adds to the mounting evidence that this is indeed the case. We report on a series of experiments conducted for different recognition tasks using the publicly available code and model of the \overfeat network which was trained to perform object classification on ILSVRC13. We use features extracted from the \overfeat network as a generic image representation to tackle the diverse range of recognition tasks of object image classification, scene recognition, fine grained recognition, attribute detection and image retrieval applied to a diverse set of datasets. We selected these tasks and datasets as they gradually move further away from the original task and data the \overfeat network was trained to solve. Astonishingly, we report consistent superior results compared to the highly tuned state-of-the-art systems in all the visual classification tasks on various datasets. For instance retrieval it consistently outperforms low memory footprint methods except for sculptures dataset. The results are achieved using a linear SVM classifier (or L2 distance in case of retrieval) applied to a feature representation of size 4096 extracted from a layer in the net. The representations are further modified using simple augmentation techniques e.g. jittering. The results strongly suggest that features obtained from deep learning with convolutional nets should be the primary candidate in most visual recognition tasks. 
