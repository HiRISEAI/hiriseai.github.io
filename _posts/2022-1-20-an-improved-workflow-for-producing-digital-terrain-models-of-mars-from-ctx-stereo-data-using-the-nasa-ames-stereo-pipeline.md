---
layout: post
title:  "An Improved Workflow for Producing Digital Terrain Models of Mars from CTX Stereo Data Using the NASA Ames Stereo Pipeline"
date: 2022-1-20
image: assets/images/mayer_dtm.png
tags: [ landforms, DTM ]
---

[An Improved Workflow for Producing Digital Terrain Models of Mars from CTX Stereo Data Using the NASA Ames Stereo Pipeline](https://www.hou.usra.edu/meetings/lpsc2018/pdf/1604.pdf){:target="_blank"}  


**Published in**:   
49th Lunar and Planetary Science Conference 2018 (LPI Contrib. No. 2083) Abstract #1604 

**Authors**:   
D. P. Mayer

**Abstract**:   
Stereo images represent a key dataset for producing digital terrain models (DTMs) of planetary surfaces. Nearly all of the high-resolution (<10 meters/pixel) stereo image data of Mars come from the CTX and HiRISE sensors. However, CTX
DTMs are not routinely produced, and are not currently released through the Planetary Data System (PDS). This often requires researchers who wish to incorporate CTX elevation data in their work to produce their own. The NASA Ames Stereo Pipeline (ASP) is a free software package that can be used to create DTMs from stereo image data collected by a
variety of sensors, including CTX [1, 2]. This abstract presents an update to the workflow described in [3] for producing CTX DTMs using ASP. The updated workflow takes advantage of new features in ASP since version 2.6.0 [4] in order to improve stereo correlation over areas of low image texture and to more effectively manage blunders and
artifacts in the disparity map.