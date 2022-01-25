---
layout: post
title: "SPOC: Deep Learning-based Terrain Classification for Mars Rover Missions"
date: 2022-1-16
image: assets/images/spoc.png
tags: [ AI, features, craters ]
---

**Published in**:   
Proceedings of the AIAA SPACE 2016-5539 13-16 Sep 2016  

**Authors**:   
Brandon Rothrock, Jeremie Papon, Ryan Kennedy, Masahiro Ono, Matt Heverly

**Abstract**:   
This paper presents Soil Property and Object Classification (SPOC), a novel software capability that can visually identify terrain types (e.g., sand, bedrock) as well as terrain features (e.g., scarps, ridges) on a planetary surface. SPOC works on both orbital and ground-bases images. Built upon a deep convolutional neural network (CNN), SPOC employs a machine learning approach, where it learns from a small volume of examples provided by human experts, and applies the learned model to a significant volume of data very efficiently. SPOC is important since terrain type is essential information for evaluating the traversability for rovers, yet manual terrain classification is very labor intensive. This paper presents the technology behind SPOC, as well as two successful applications to Mars rover missions. The first is the landing site traversability analysis for the Mars 2020 Rover (M2020) mission. SPOC identifies 17 terrain classes on full-resolution (25 cm/pixel) HiRISE (High Resolution Imaging Science Experiment) images for all eight candidate landing sites, each of which spans over ∼ 100km<sup>2</sup>. The other application is slip prediction for the Mars Science Laboratory (MSL) mission. SPOC processed several thousand NAVCAM (Navigation camera) images taken by the Curiosity rover. Predicted terrain classes were then correlated with observed wheel slip and slope angles to build a slip prediction model. In addition, SPOC was integrated into the MSL downlink pipeline to automatically process all NAVCAM images. These tasks were impractical, if not impossible, to perform manually. SPOC opens the door for big data analysis in planetary exploration. It has a promising potential for a wider range of future applications, such as the automated discovery of scientifically important terrain features on existing Mars orbital imagery, as well as traversability analysis for future surface missions to small bodies and icy worlds.
