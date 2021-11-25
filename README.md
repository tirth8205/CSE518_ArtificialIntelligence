# Artificial Intelligence (CSE518)

## Introduction

The project is about early dectection of Alzheimer's Disease using concepts of Artifical Intelligence. 

Alzheimer’s disease  (AD)  is an irreversible neurodegenerative disease.  Over 50  million people reported worldwide have dementia,  and these figures are expected to touch  132  million by  2050.  Mild cognitive impairment  (MCI)  is the stage of  AD  from when initial symptoms are observed,  and it is crucial to analyze pathological changes in this stage. Up-till now, various studies for  AD  detection have been developed via sMRI, which are based on analysis since it provides an intuitive way to observe the structural changes of the brain.

## Approach

Current MRI-based methods can be generally categorized
into four classes:
- Voxel-based method
- Region-of-interest (ROI) based method
- Whole-image based method
- Patch-based method


Voxel-based methods require cortical thickness, brain tissue density and volume to measure the morphological changes of the brain. While ROI based methods technically needs prior knowledge about the regions associated with disease. These methods naturally lose some helpful information. The whole-image based methods use the whole image volume, which makes it harder to detect the precise structural abnormality and in patch-based approach, we take small patches as input, but they have highly relied on the discovery of anatomical landmarks. Generally, conventional machine learning (ML) methods require complex preprocessing to get features for classification. Whereas a typical deep learning (DL) based method, convolutional neural network (CNN) can hierarchically extract the most discriminative feature.
CNN has shown great power in end-to-end AD analysis. For instance, 2D CNNs have achieved excellent performance for AD detection.

We will be using some functions and dependencies of TensorFlow and Keras, some of the critical processes are as follows:
Dropout layer: The purpose of the dropout layer is to minimize the effect of overfitting within a trained network.
Max pool 2D: Objective maxpool2D is to down-sample an input representation.
Conv 2D: Conv2D are generally smaller than the input image, so we move them across the whole picture.
Separable Conv 2D: A separable convolution splits a kernel into two separate kernels that do two convolutions: the depth-wise convolution and the pointwise convolution.
Batch Normalization: Batch normalization is designed to automatically standardize the inputs to a layer in a deep learning neural network.
Dense Layer: Dense Layer is used to classify images based on output from convolutional layers.
Flattening Layer: Flattening layer is used to flatten the convolutional layers' production to create a single long feature vector.
Adam Optimizer: Adam is an optimization solver for the Neural Network algorithm that is computationally efficient, requires little memory, and is well suited for problems that are significant in terms of data or parameters or both. Adam is a popular extension to stochastic gradient descent.
Binary cross-entropy(Loss Function): The binary cross entropy is very convenient to train a model to solve many classification problems at the same time, if each classification can be reduced to a binary choice (i.e., yes or no, A or B, 0 or 1)

## Results


- Validation accuracy vs. Epoch

![WhatsApp Image 2021-11-24 at 8 39 01 PM](https://user-images.githubusercontent.com/68604113/143392241-7d7e0e29-3ea0-44d8-a3ae-186421e925ea.jpeg)

- Rate Loss vs. Epoch

![WhatsApp Image 2021-11-24 at 8 39 44 PM](https://user-images.githubusercontent.com/68604113/143392247-32d950fd-a1d2-4ac6-8796-d8a4eeda13fe.jpeg)

- Evaluation

![WhatsApp Image 2021-11-24 at 8 40 14 PM](https://user-images.githubusercontent.com/68604113/143392251-e677f793-5064-4ab6-b24f-437aff266f11.jpeg)

## Installation Guidelines

- Download the CoreFour_FinalCode.ipynb file.
- Downlaod the Dataset from Kaggle (https://www.kaggle.com/tourist55/alzheimers-dataset-4-class-of-images)
- Upload the dataset in Google Drive in folder CNN_AD
- Upload the downloaded CoreFour_FinalCode.ipynb file in Collab
- Run the code

## References

- L. J. Herrera, I. Rojas, H. Pomares, A. Guillén, O. Valenzuela and O. Baños, "Classification of MRI Images for Alzheimer's Disease Detection," 2013 International Conference on Social Computing, 2013, pp. 846-851, doi: 10.1109/SocialCom.2013.127.L. J. Herrera, I. Rojas, H. Pomares, A. Guillén, O. Valenzuela and O. Baños, "Classification of MRI Images for Alzheimer's Disease Detection," 2013 International Conference on Social Computing, 2013, pp. 846-851, doi: 10.1109/SocialCom.2013.127.
- Wang, C. (2018, August 14). A Basic Introduction to Separable Convolutions - Towards Data Science. Medium. https://towardsdatascience.com/a-basic-introduction-to-separable-convolutions-b99ec3102728 
- Alzheimer’s disease - Symptoms and causes. (2021, June 26). Mayo Clinic. https://www.mayoclinic.org/diseases-conditions/alzheimers-disease/symptoms-causes/syc-20350447 
- Alzheimer’s Dataset ( 4 class of Images). (2019, December 26). Kaggle. https://www.kaggle.com/tourist55/alzheimers-dataset-4-class-of-images 
