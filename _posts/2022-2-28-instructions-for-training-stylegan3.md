---
layout: post
title:  "Instructions for Training StyleGAN3"
date: 2022-2-28
image: assets/images/synthetic.jpg
tags: [ AI, tutorials ]
---

**Prerequisites**:
- Access to a command-line prompt on the cluster that has the GPU
- Command-line navigation (useful tips- <a href="https://help.ubuntu.com/community/UsingTheTerminal#File_.26_Directory_Commands" target="_blank">https://help.ubuntu.com/community/UsingTheTerminal#File_.26_Directory_Commands</a>)  
- Access to Github repo: [https://github.com/doinksta/stylegan3](https://github.com/doinksta/stylegan3){:target="_blank"}
- Access to data (currently on Google Drive: [https://drive.google.com/drive/folders/13c83PksoW83rGS85W9KpAKw8SSuqid_Z?usp=sharing](https://drive.google.com/drive/folders/13c83PksoW83rGS85W9KpAKw8SSuqid_Z?usp=sharing){:target="_blank"} )


**Note**:
- Steps 1-4 only need to be completed once, as these steps are setting up a code environment that contains all the necessary code installed in it.
- If steps 1-4 have been completed already, the way to get to training code is to cd into the folder “stylegan3” and then activate the code environment with all the packages installed previously (using the command conda activate stylegan3 from step 5)

**Instructions**:
1. Open command-line prompt and navigate to a folder you want to download / put project files in (use cd command)  

2. Clone Github repo by typing  
   <code>git clone https://github.com/doinksta/stylegan3.git</code>  
   into the command-line prompt and hitting enter. This will download code into a folder called stylegan3.<br>  

   <div><img src="/assets/images/Picture1.png" class="img-fluid" alt="Picture1" /></div><br>

3. In command-line prompt, open newly created “stylegan3” folder by typing  
   <code>cd stylegan3/</code>  
   and hitting enter. You can view the contents of this folder by typing  
   <code>ls</code>  

   <div><img src="/assets/images/Picture2.png" class="img-fluid" alt="Picture2" /></div><br>

4. We will now use anaconda to install necessary software requirements. To do this, run the following command:  
   <code>conda env create -f environment.yml</code>  

   This makes the compute follow the instructions in “environment.yml” to download necessary code packages (for free) and puts them into a custom coding environment.

    <div><img src="/assets/images/Picture3.png" class="img-fluid" alt="Picture3" /></div><br>

5. Once the above command has finished running, we need to activate the coding environment that contains the packages needed to run the code. We do this by running the command  
   <code>conda activate stylegan3</code>

6.	We will now run a small test using a small dataset. This dataset is contained in the zip file “test_data.zip” (located directly in the stylegan3 folder), and it contains 50 images selected from the HIRISE dataset. To start training, run the following code (all on one line)  
   <code>python train.py --outdir=training_runs --data=test_data.zip --cfg=stylegan3-r --gpus=8 --batch=32 --gamma=8 --metrics=none</code>  

    If things go well, the code will create a folder called “training_runs” within the “stylegan3” folder, and no errors or exceptions should occur.  
    
    Please contact Erich if anything seems wrong, or send screenshots of what is in the folders to double check if things are working correctly.

7.	To train on the full dataset:  

    a. Download all the images from the dataset as a .zip file: [https://drive.google.com/drive/u/1/folders/13c83PksoW83rGS85W9KpAKw8SSuqid_Z](https://drive.google.com/drive/u/1/folders/13c83PksoW83rGS85W9KpAKw8SSuqid_Z){:target="_blank"}  

    b. Rename the zip file to “full_data.zip” and place it in the stylegan3 folder (use mv command if you are doing this from command line)  

    c. Run the following code (all on one line)

    <code>python train.py --outdir=training_runs --data=full_data.zip --cfg=stylegan3-r --gpus=8 --batch=32 --gamma=8 --metrics=none</code>  

    Using the estimates from [https://github.com/doinksta/stylegan3/blob/main/docs/configs.md](https://github.com/doinksta/stylegan3/blob/main/docs/configs.md){:target="_blank"}, the small test dataset might take around 4 seconds to train, and the full dataset might take around 0.63 hours.




