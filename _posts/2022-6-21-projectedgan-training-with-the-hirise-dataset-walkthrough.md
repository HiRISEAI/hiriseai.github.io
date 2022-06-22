---
layout: post
title:  "ProjectedGAN Training with the HiRISE Dataset Walkthrough"
date: 2022-6-21
image: assets/images/Mars-MRO-orbiter-fresh-crater-sirenum-fossae_thumb.jpg
tags: [ imagery, exhibits, AI, MinLab ]
---

Emmett Seto, Skylar Villasenor, Paul Kim, Troy Harris, Nevin Jiang, Ping Wang, Dejia Xu  
Nova77 STEM Workshop  
June 2022  

<div><img src="/assets/images/Mars-MRO-orbiter-fresh-crater-sirenum-fossae.jpg" class="img-fluid" alt=" "></div>
<br>    
This HiRISE+AI project was funded by NASA (Grant Number: 80NSSC22K0440)  
Contact Us: pingwang@nova77.org  

**What you need**:
1.	Your Gmail account  
2.	The HiRISE dataset: [https://drive.google.com/file/d/15xdPhkbXiDTeEv4ZVDJzx1rpMUrLj9Zb/view?usp=sharing](https://drive.google.com/file/d/15xdPhkbXiDTeEv4ZVDJzx1rpMUrLj9Zb/view?usp=sharing){:target="_blank"}   
3.	The Colab (notebook): [https://github.com/rocks2021/training-gans/blob/main/train_projectedgan_fastgan_lite_hirise.ipynb](https://github.com/rocks2021/training-gans/blob/main/train_projectedgan_fastgan_lite_hirise.ipynb){:target="_blank"} 
4.	GPU(s): You need GPU(s) to train a GAN. You can either buy a $9.99 per month Colab pro plan or a $49.99 per month Colab pro+ plan.<br>  

**Getting started**:
1.	Login into your Gmail account.  

2.	Download the hirise_128gan.zip (the HiRISE dataset above) to your local computer and then upload to your Google Drive under My Drive.
- <div><img src="/assets/images/walk2.png" class="img-fluid" alt=" "></div>
<br> 
3.	Go to [https://github.com/rocks2021/training-gans/blob/main/train_projectedgan_fastgan_lite_hirise.ipynb](https://github.com/rocks2021/training-gans/blob/main/train_projectedgan_fastgan_lite_hirise.ipynb){:target="_blank"}
and click “Open in Colab”.  

    <div><img src="/assets/images/walk3.png" class="img-fluid" alt=" "></div>
<br> 

4.	Click “Copy to Drive”.  

    <div><img src="/assets/images/walk4.png" class="img-fluid" alt=" "></div>
<br> 

5.	Rename your Colab notebook. When renaming, keep “.ipynb” at the end.  

    <div><img src="/assets/images/walk5.png" class="img-fluid" alt=" "></div>
<br>

6.	Click “Runtime” from the menu bar of the Colab notebook, and then click “Change runtime type”.  

    <div><img src="/assets/images/walk6.png" class="img-fluid" alt=" "></div>
<br>

7.	Click the dropdown menu of “Hardware accelerator” and select “GPU” and “High-RAM”. Then, click save.  

    <div><img src="/assets/images/walk7.png" class="img-fluid" alt=" "></div>
<br> 

8.	Click the “Connect” button on the upper right and wait until a green check mark appears.  

    <div><img src="/assets/images/walk8.png" class="img-fluid" alt=" "></div>
<br>

9.	Click “Runtime” from the menu bar and choose “Restart and run all”, and then, wait.  

    <div><img src="/assets/images/walk9.png" class="img-fluid" alt=" "></div>
<br>

10.	There are seven cells of code that need to be run. When running the second cell, a popup appears. Choose “Connect to Google Drive”.  

    <div><img src="/assets/images/walk4.png" class="img-fluid" alt=" "></div>
<br>
Then, choose your Gmail account and click “Allow”.

11.	While the seventh cell is running, a “runs” folder will automatically be generated in “My Drive”. All the fake images and models will be saved in the “runs” folder.

12.	If you need to resume the training, delete the `#` before `--resume=/content/...`  and repeat steps 6 through 10.  

13.	Wait until the FID is below 10. 


