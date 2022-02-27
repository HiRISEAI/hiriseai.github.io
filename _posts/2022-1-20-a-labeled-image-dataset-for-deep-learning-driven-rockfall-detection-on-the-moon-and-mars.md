---
layout: post
title:  "A Labeled Image Dataset for Deep Learning-Driven Rockfall Detection on the Moon and Mars"
date: 2022-1-20
image: assets/images/labeled.png
tags: [ imagery, AI ]
---

**Published in**:   
Frontiers in Remote Sensing Volume 2, Feb 2021

**Authors**:   
V. T. Bickel, L. Mandrake, G. Doran

**Abstract**:   

The term rockfall describes the rapid displacement of a large, usually meter–sized block of rock down–slope, triggered by, for example, endogenic or exogenic events like impacts, quakes or rainfall (Hungr et al., 2014; Xiao et al., 2013). In a remote sensing context, the term rockfall is also being used to describe the characteristic geomorphic deposit of a rockfall event that can be identified from an air- or space–borne perspective, i.e., the combination of a displaced boulder and the track it carved into the slope substrate while bouncing, rolling, and sliding over the surface (also called “boulder with track” or “rolling boulder”) (Hovland and Mitchell, 1973; Filice, 1967; Moore, 1970) (see Figure 1). In planetary science, the spatial distribution and frequency of rockfalls provide insights into the global erosional state and activity of a planetary body (Bickel et al., 2020a; Tesson et al., 2020) while their tracks act as tools that allow for the remote estimation of the surface strength properties of yet unexplored regions in preparation of future ground exploration missions (Eggleston et al., 1968), such as the lunar pyroclastic (Bickel et al., 2019), polar sunlit (Bickel and Kring, 2020) and permanently shadowed regions of the Moon (Sargeant et al., 2020). Due to their small physical size (meters), the identification and mapping of rockfalls in planetary satellite imagery is challenging and very time–consuming, however. For this reason, Bickel et al. (2018) and Bickel et al. (2020b) trained convolutional neural networks to automate rockfall mapping in lunar and martian satellite imagery. Parts of the unpublished datasets used for earlier work have now been complemented with newly labeled data to create a well-balanced dataset of 2,822 lunar and martian rockfall labels (which we call “RMaM–2020”—Rockfall Mars Moon 2020, 416 MB in total, available here: https://edmond. mpdl.mpg.de/imeji/collection/DowTY91csU3jv9S2) that can be used for deep learning and other data science applications. Here, balanced means that the labels have been derived from imagery with a wide and continuous range of properties like spatial resolution, solar illumination, and others. So far, this dataset has been used to analyze the benefits of multi–domain learning on rockfall detector performance (Mars & Moon vs. Moon–only or Mars–only), but there are numerous other (non–planetary science) applications such as for featurization, feature or target recognition (aircraft/spacecraft autonomy), and data augmentation experiments. All labels represent the localization of a rockfall instance in a satellite image, i.e., mark the position of the characteristic combination of boulder and track in an image (see e.g., Bickel et al., 2018).

