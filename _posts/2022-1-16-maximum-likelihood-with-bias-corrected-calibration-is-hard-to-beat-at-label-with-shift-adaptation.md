---
layout: post
title: "Maximum likelihood with Bias-corrected Calibration is Hard-to-beat at Label Shift Adaptation"
date: 2022-1-16
image: assets/images/ESP_025124_1985_000012.jpg
tags: [ AI ]
---

[Maximum Likelihood with Bias-Corrected Calibration is Hard-To-Beat at Label Shift Adaptation](https://arxiv.org/abs/1901.06852){:target="_blank"}  

**Published in**:   
Proceedings of the 37th International Conference on Machine Learning, Vienna, Austria, PMLR 119, 2020

**Authors**:   
Amr Alexandari, Anshul Kundaje, Avanti Shrikumar

**Abstract**:   
Label shift refers to the phenomenon where the prior class probability p(y) changes between the training and test distributions, while the conditional probability p(x|y) stays fixed. Label shift arises in settings like medical diagnosis, where a classifier trained to predict disease given symptoms must be adapted to scenarios where the baseline prevalence of the disease is different. Given estimates of p(y|x) from a predictive model, Saerens et al. proposed an efficient maximum likelihood algorithm to correct for label shift that does not require model retraining, but a limiting assumption of this algorithm is that p(y|x) is calibrated, which is not true of modern neural networks. Recently, Black Box Shift Learning (BBSL) and Regularized Learning under Label Shifts (RLLS) have emerged as state-of-the-art techniques to cope with label shift when a classifier does not output calibrated probabilities, but both methods require model retraining with importance weights and neither has been benchmarked against maximum likelihood. Here we (1) show that combining maximum likelihood with a type of calibration we call bias-corrected calibration outperforms both BBSL and RLLS across diverse datasets and distribution shifts, (2) prove that the maximum likelihood objective is concave, and (3) introduce a principled strategy for estimating source-domain priors that improves robustness to poor calibration. This work demonstrates that the maximum likelihood with appropriate calibration is a formidable and efficient baseline for label shift adaptation.