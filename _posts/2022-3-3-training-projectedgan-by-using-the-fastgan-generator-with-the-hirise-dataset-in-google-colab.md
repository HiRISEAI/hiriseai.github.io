---
layout: post
title:  "Training ProjectedGAN by Using the FastGAN Generator with the HiRISE Dataset in Google Colab"  
date: 2022-3-3  
image: assets/images/ESP_011527_1325_000005.jpg  
tags: [ AI, MinLab, imagery ]
---

<img width=700 class="img-fluid" src="/assets/images/hirise_projectedgan.gif">

<br>
**Generative Adversarial Networks (GANs)**  
[Goodfellow et al, 2014] introduced Generative Adversarial Networks (GANs) in 2014. Since then, GANs have been shown to successfully learn features of the training dataset and generate convincingly fake images with no counterparts in the training dataset. However, training GANs is known to be fickle and hard. Up until now most GAN methods are based on best practices.

**The Training Code**  
The training code used here is based on the ProjectedGAN ([https://github.com/autonomousvision/projected_gan](https://github.com/autonomousvision/projected_gan){:target="_blank"}) merged with the code provided by FastGAN Generator ([https://github.com/odegeasslbc/FastGAN-pytorch](https://github.com/odegeasslbc/FastGAN-pytorch){:target="_blank"}). The Colab for this training can be found here ([https://github.com/rocks2021/Colabs-for-HiRISEAI/blob/main/t1_train_projectedgan_fastganG_hirise128.ipynb](https://github.com/rocks2021/Colabs-for-HiRISEAI/blob/main/t1_train_projectedgan_fastganG_hirise128.ipynb){:target="_blank"}). 

**The HiRISE Dataset**  
The HiRISE dataset is created based on the Mars image content classification [Wagstaff et al., 2021]. Images of RSL and Martian pole ice cap features are also added into the dataset. All the original images downloaded from the HiRISE website are of 512x512 pixel resolution; and then they are resized to be of 128x128 pixel resolution in order to save computing time. The HiRISE dataset includes 8888 square images of Martian landscaspes.

**The Training Resources**  
The Google Colab Pro which enables to access a Tesla P100 GPU by Nvidia with 16Gb of vram and 25GB of RAM is used for the training. With the given resources, the training takes around 10 hours and the final FID reaches 8.76.

**The Training Steps**  
1. Clone the ProjectedGAN repository  
`!git clone https://github.com/autonomousvision/projected_gan.git`

2. Install dependencies  
`!pip install timm`  
`import timm`  

3. Train ProjectedGAN  
`!python train.py --outdir=/content/drive/MyDrive/runs/ --cfg=fastgan_lite --data=/content/drive/MyDrive/hirise_128gan.zip --gpus=1 --batch=64 --batch-gpu=8 --snap=20 --kimg=10000`

4. Resume training  
`!python train.py --outdir=/content/drive/MyDrive/runs/ --cfg=fastgan_lite --data=/content/drive/MyDrive/hirise_128gan.zip --gpus=1 --batch=64 --batch-gpu=8 --snap=20 --kimg=10000 --resume=/content/drive/MyDrive/best_model.pkl`

**References**  

A. Sauer, K. Chitta, J. Muller, and A. Geiger. Projected GANs converge faster. In Neural Information Processing Systems (NeurIPS), 2021. 

B. Liu, Y. Zhu, K. Song, and A. Elgammal. Towards faster and stabilized gan training for high-fidelity few-shot image synthesis. In Proc. of the International Conf. on Learning Representations (ICLR), 2021.


