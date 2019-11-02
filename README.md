# CNN_coffee_ring_effect
This project uses CNN model to analyze water samples of coffee ring effect

Dataset:
Two set of images collected from same 30 water samples on two different days.
First set images is 150 images consisting of 5 replicates of 30 water samples on 6/13/2017.
Second set of images is 150 images consisting of 5 replicates of 30 water samples on 8/14/2017.
Two sets of datasets created by these collected 300 images.

The first dataset is training dataset consisting of 180 images. Consisting three replicates of each water sample images in 6/13/2017 dataset and three replicates of each water sample images in second dataset.

The Second dataset is testing dataset consisting of 180 images. Consisting two replicates of each water sample images in 8/14/2017 dataset and two replicates of each water sample images in second dataset.

The training datset and testing dataset were created by ramdomly selecting images from 6/13/2017 and 8/14/2017 images.

Preprocessing images:

RGB_noemalize.m
  This file normalize images colors to smooth images and the smoothed images increased accuracy.

Function files:
  1, read_images_to_pkl.py
    This file read images from folder and converted images from RGB to black and white and save all the images in one pkl file.

  1, load train data.py
    This files reads images pkl file and return training data, training data labels in torch format
    
  2, load test data.py
    This files reads images pkl file and return training data, training data labels in torch format
    


1, run the CNN_main.py first. The file includes the model. read data and train the model by training data.

