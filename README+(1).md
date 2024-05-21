# Convolutional Neural Network Model for Skin Cancer (Melanoma) Detection
To build a CNN based model which can accurately detect **melanoma**. Melanoma is a type of cancer that can be deadly if not detected early. It accounts for 75% of skin cancer deaths. A solution which can evaluate images and alert the dermatologists about the presence of melanoma has the potential to reduce a lot of manual effort needed in diagnosis.


## Table of Contents
*  General Info
* Project Pipeline
* Conclusions



## General Information
- The dataset consists of 2357 images of malignant and benign oncological diseases, which were formed from the International Skin Imaging Collaboration (ISIC). All images were sorted according to the classification taken with ISIC, and all subsets were divided into the same number of images, with the exception of melanomas and moles, whose images are slightly dominant.

- The data set contains the following diseases:
a. Actinic keratosis
b. Basal cell carcinoma
c. Dermatofibroma
d. Melanoma
e. Nevus
f. Pigmented benign keratosis
g. Seborrheic keratosis
h. Squamous cell carcinoma
i. Vascular lesion

## Project Pipeline
a. Data Reading/Data Understanding → Defining the path for train and test images 
b. Dataset Creation→ Create train & validation dataset from the train directory with a batch size of 32. Also, make sure you resize your images to 180*180.
c. Dataset visualisation → Create a code to visualize one instance of all the nine classes present in the dataset 
d. Model Building & training : 
    - Create a CNN model, which can accurately detect 9 classes present in the dataset. While building the model, rescale images to normalize pixel values between (0,1).
    - Choose an appropriate optimiser and loss function for model training
    - Train the model for ~20 epochs
    - Write your findings after the model fit. You must check if there is any evidence of model overfit or underfit.
    - Chose an appropriate data augmentation strategy to resolve underfitting/overfitting
e. Chose an appropriate data augmentation strategy to resolve underfitting/overfitting 
f. Model Building & training on the augmented data :
    - Create a CNN model, which can accurately detect 9 classes present in the dataset. While building the model rescale images to normalize pixel values between (0,1).
    - Choose an appropriate optimiser and loss function for model training
    - Train the model for ~20 epochs
    - Write your findings after the model fit, see if the earlier issue is resolved or not?
g. Class distribution: Examine the current class distribution in the training dataset 
    - Which class has the least number of samples?
    - Which classes dominate the data in terms of the proportionate number of samples?
h. Handling class imbalances: Rectify class imbalances present in the training dataset with Augmentor library.
i. Model Building & training on the rectified class imbalance data :
    - Create a CNN model, which can accurately detect 9 classes present in the dataset. While building the model, rescale images to normalize pixel values between (0,1).
    - Choose an appropriate optimiser and loss function for model training
    - Train the model for ~30 epochs
    - Write your findings after the model fit, see if the issues are resolved or not?

## Conclusions
- Conclusion from the analysis 1
    In the first model,there is a noticable difference between training and validation accuracy. Training accuaracy is close to 90% whereas validation accuarcy is close to 50% only.It signifies that there is overfitting
- Conclusion from the analysis 2
    In the second model after applying some augmentation strategy, the training and validation accuaracy are almost same. However, the accuaracy are quite low. The model needs to be trained with more number of epochs after handling of class imbalance if any.
- Conclusion from the analysis 3
    The accuracy of both Training and and validation dataset has incresed. The differnce in acurracy between the two is also negligible. The 3rd model with class imbalance handling and increased number of epochs seems to be a good model.



## Contact
Created by ABHINAV KUMAR RAI (raiabhinav9)


