# Artificial Intelligence (CSE518)

## Early Detection of Alzheimer's Disease Using Artificial Intelligence

### Introduction
The project focuses on the early detection of Alzheimer's Disease (AD) using artificial intelligence concepts.

Alzheimer’s disease is an irreversible neurodegenerative disorder affecting millions worldwide. Currently, over 50 million people are diagnosed with dementia, and this number is expected to rise to 132 million by 2050. Mild Cognitive Impairment (MCI) is the initial stage of AD, where early symptoms become noticeable. Identifying pathological changes during this phase is crucial for early intervention.

So far, various studies on AD detection have relied on structural Magnetic Resonance Imaging (sMRI) due to its effectiveness in visually analysing structural changes in the brain.

---

### Approach
MRI-based methods for AD detection can be classified into four categories:

1. **Voxel-based method:** Measures morphological changes in the brain, including cortical thickness, brain tissue density, and volume.
2. **Region-of-Interest (ROI) based method:** Focuses on predefined brain regions associated with the disease but may overlook some valuable information.
3. **Whole-image-based method:** Utilises the entire image volume, making it challenging to pinpoint precise structural abnormalities.
4. **Patch-based method:** Processes small image patches but is highly dependent on identifying anatomical landmarks.

Traditional machine learning (ML) methods require extensive preprocessing to extract features for classification. In contrast, deep learning (DL) approaches, particularly Convolutional Neural Networks (CNNs), hierarchically extract discriminative features, offering a robust end-to-end analysis of AD.

CNNs have demonstrated exceptional performance in AD detection, with 2D CNN models achieving notable success.

---

### Implementation
The implementation involves key functions and dependencies from **TensorFlow** and **Keras**. The critical processes include:

- **Dropout Layer:** Reduces overfitting in trained networks.
- **Max Pool 2D:** Down-samples the input representation.
- **Conv 2D:** Uses convolutional filters to scan across an image.
- **Separable Conv 2D:** Splits convolutional kernels into two steps: depth-wise convolution and pointwise convolution.
- **Batch Normalization:** Standardises inputs within a deep learning model.
- **Dense Layer:** Classifies images based on convolutional output.
- **Flattening Layer:** Converts convolutional outputs into a single feature vector.
- **Adam Optimizer:** An adaptive optimisation algorithm suited for large datasets.
- **Binary Cross-Entropy (Loss Function):** A loss function ideal for binary classification problems.

---

### Results
The results of the model training are illustrated in the graphs below:

#### Validation Accuracy vs. Epoch
![Validation Accuracy Graph](https://user-images.githubusercontent.com/68604113/143392241-7d7e0e29-3ea0-44d8-a3ae-186421e925ea.jpeg)

#### Rate Loss vs. Epoch
![Loss Rate Graph](https://user-images.githubusercontent.com/68604113/143392247-32d950fd-a1d2-4ac6-8796-d8a4eeda13fe.jpeg)

#### Evaluation Metrics
![Evaluation Results](https://user-images.githubusercontent.com/68604113/143392251-e677f793-5064-4ab6-b24f-437aff266f11.jpeg)

---

### Installation Guidelines
Follow the steps below to run the project:

1. Download the `CoreFour_FinalCode.ipynb` file.
2. Download the dataset from Kaggle: [Alzheimer’s Dataset (4 classes of images)](https://www.kaggle.com/datasets/marcopinamonti/alzheimer-mri-4-classes-dataset).
3. Upload the dataset to Google Drive under the folder **CNN_AD**.
4. Upload the downloaded `CoreFour_FinalCode.ipynb` file to Google Colab.
5. Run the code in Colab.

---

### References
1. **L. J. Herrera, I. Rojas, H. Pomares, A. Guillén, O. Valenzuela, and O. Baños.**  
   *"Classification of MRI Images for Alzheimer's Disease Detection,"* 2013 International Conference on Social Computing, pp. 846-851, 2013.  
   DOI: [10.1109/SocialCom.2013.127](https://doi.org/10.1109/SocialCom.2013.127).

2. **Wang, C. (2018, August 14).**  
   *"A Basic Introduction to Separable Convolutions."* Towards Data Science, Medium.  
   [Read Article](https://towardsdatascience.com/a-basic-introduction-to-separable-convolutions-b99ec3102728).

3. **Mayo Clinic (2021, June 26).**  
   *"Alzheimer’s Disease - Symptoms and Causes."*  
   [Read Article](https://www.mayoclinic.org/diseases-conditions/alzheimers-disease/symptoms-causes/syc-20350447).

4. **Kaggle (2019, December 26).**  
   *"Alzheimer’s Dataset (4 classes of images)."*  
   [View Dataset](https://www.kaggle.com/tourist55/alzheimers-dataset-4-class-of-images).
