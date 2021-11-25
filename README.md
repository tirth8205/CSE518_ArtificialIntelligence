# Artificial Intelligence (CSE518)

## Introduction

The project is about early dectection of Alzheimer's Disease using concepts of Artifical Intelligence. 

Alzheimer’s disease  (AD)  is an irreversible neurodegenerative disease.  Over 50  million people reported worldwide have dementia,  and these figures are expected to touch  132  million by  2050.  Mild cognitive impairment  (MCI)  is the stage of  AD  from when initial symptoms are observed,  and it is crucial to analyze pathological changes in this stage. Up-till now, various studies for  AD  detection have been developed via sMRI, which are based on analysis since it provides an intuitive way to observe the structural changes of the brain.

Current MRI-based methods can be generally categorized into four classes:
- Voxel-based method
- Region-of-interest (ROI) based method
- Whole-image based method
- Patch-based method

Voxel-based methods require cortical thickness,  brain tissue density, and volume to measure the morphological changes of the brain.  While ROI-based methods technically need prior knowledge about the regions associated with the disease.  These methods naturally lose some helpful information.  The whole-image-based methods use the whole image volume, making it harder to detect the specific structural abnormality. We take small patches as input in the patch-based process,  but they are highly relied on discovering anatomical landmarks.  Generally, conventional machine learning (ML) methods require complex pre-processing to get features for classification. A typical deep learning  (DL)  based method,  convolutional neural network  (CNN), can hierarchically extract the most discriminative feature. CNN  has shown great power in end-to-end  AD  analysis. For instance, 2D CNNs have achieved excellent performance for  AD  detection.  However,  2D  slices of  MRI  data lose spatial information in the brain cube, which affects the detection performance.  Therefore,  more and more studies focus on developing  3D  CNNs to achieve better results.  Recurrent neural network (RNN) is another typical deep learning-based architecture.  Recently,  some studies have attempted to leverage  3DCNN architecture to extract low-level features and then use long short-term memory (LSTM) to learn high-level semantic information for final classification. But classic LSTM ignores the spatial information of input data. Although these methods have improved performance, accurate AD detection is still at the primary stage and needs in-depth study.


## Results

![WhatsApp Image 2021-11-24 at 8 39 01 PM](https://user-images.githubusercontent.com/68604113/143392241-7d7e0e29-3ea0-44d8-a3ae-186421e925ea.jpeg)
![WhatsApp Image 2021-11-24 at 8 39 44 PM](https://user-images.githubusercontent.com/68604113/143392247-32d950fd-a1d2-4ac6-8796-d8a4eeda13fe.jpeg)
![WhatsApp Image 2021-11-24 at 8 40 14 PM](https://user-images.githubusercontent.com/68604113/143392251-e677f793-5064-4ab6-b24f-437aff266f11.jpeg)
