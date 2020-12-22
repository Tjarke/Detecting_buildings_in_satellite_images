# Detecting_buildings_in_satellite_images

In this repo buildings will be detected in satellite images.  

## Make use of this repo:
The dataset is from the spacenet 7 challenge and the download explanations are here:  
https://spacenet.ai/sn7-challenge/  
For demonstration purposes 2 images are added in this repository. However, the notebook normally randomly selects images from the original dataset.  
To run the transfer learning part of this notebook solaris is used. According to the developers installing solaris might be tricky but the instructions are given here:  
https://solaris.readthedocs.io/en/latest/installation.html#installation 
I would advise the user to first install everything for the solaris environment and then add the libraries that are missing to run the notebook on top of that. The provided requirements.txt file is for comparison purposes only, as it will not work.  
To make use of the pretrained model it has to be reassembled with  
cat weight_split/* > xdxd_final.pth  
in CosmiQ_SN7_Baseline/models/sn7_baseline/

## Content
The dataset will be briefly investigated. Afterwards the segmentation problem will be solved with transfer learning, a small fully connected neural net and a small fully convolutional neural net.  
The results will be shown and analyzed quantitatively with the f1 score.  
In general the original model performs better than the CNN model and the CNN model outperforms the FNN model. But improving the original model was not the purpose of this exercise, just doing some lightweight image segmentation.  
