# Artificial Intelligence (CSE518)

## Introduction

The project is about early dectection of Alzheimer's Disease using concepts of Artifical Intelligence. 

Current MRI-based methods can be generally categorized into four classes:
- Voxel based method
- Region-of-interest (ROI) based method
- Whole-image based method
- Patch based method

Voxel-based  methods  requires  cortical  thickness,  brain tissue  density  and  volume  to  measure  the  morphological changes  of  brain.  While,  ROI  based  methods  technically needs  prior  knowledge  about  the  regions  associated  with disease.  These  methods  naturally  lose  some  useful  information.  The  whole-image  based  methods  use  the  whole  image  volume,  which  makes  harder  to  detect  the  precise structural  abnormality  and  in  patch  based  method,  we  take small  patches  as  input,  but  they  are  highly  relied  on  the discovery of anatomical landmarks.  Generally, conventional machine learning (ML) methods re-quire complex pre-processing to get features for classification. Whereas,  a  typical  deep  learning  (DL)  based  method,  convolutional  neural  network  (CNN)  can  hierarchically  extract the most discriminative feature. CNN  has  shown  great  power  in  end-to-end  AD  analysis. For instance, 2D CNNs have achieved excellent performance for  AD  detection.  However,  2D  slices  of  MRI  data  lose spatial information in brain cube, which affects the detection performance.  Therefore,  more  and  more  studies  focus  on developing  3D  CNNs  to  achieve  better  results.  Recurrent neural network (RNN) is another typical deep learning based architecture.  Recently,  some  studies  attempt  to  leverage  3DCNN architecture to extract low-level features, and then use long short-term memory (LSTM) to learn high level semantic information for final classification. But classic LSTM ignores the spatial information of input data. Although these methods have gained performance improvement, accurate AD detection is still at primary stage and needs in-depth study.


