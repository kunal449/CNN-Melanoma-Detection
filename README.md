# CNN-Melanoma-Detection
A repository for Melanoma Detection Assignment



### Problem statement: 
In this assignment, you will build a multiclass classification model using a custom convolutional neural network in tensorflow. 

To build a CNN based model which can accurately detect melanoma. Melanoma is a type of cancer that can be deadly if not detected early. It accounts for 75% of skin cancer deaths. A solution which can evaluate images and alert the dermatologists about the presence of melanoma has the potential to reduce a lot of manual effort needed in diagnosis.


The dataset consists of 2357 images [2239 Training and 118 Test] of the 9 classes, which were formed from the International Skin Imaging Collaboration (ISIC). The data set contains the following diseases:

1. Actinic keratosis
2. Basal cell carcinoma
3. Dermatofibroma
4. Melanoma
5. Nevus
6. Pigmented benign keratosis
7. Seborrheic keratosis
8. Squamous cell carcinoma
9. Vascular lesion
 

NOTE: You don't have to use any pre-trained model using Transfer learning. All the model building process should be based on a custom model.

 

### Project Pipeline
- Data Reading/Data Understanding → Defining the path for train and test images 
- Dataset Creation→ Create train & validation dataset from the train directory with a batch size of 32. Also, make sure you resize your images to 180*180.
- Dataset visualisation → Create a code to visualize one instance of all the nine classes present in the dataset 
- Base Model Building & training : 
    Create a CNN model, which can accurately detect 9 classes present in the dataset. While building the model rescale images to normalize pixel values between (0,1).
- Choose an appropriate optimiser and loss function for model training
- Train the model for ~20 epochs
- Write your findings after the model fit, see if there is evidence of model overfit or underfit
- Choose an appropriate data augmentation strategy to resolve underfitting/overfitting 
**Model Building & training on the augmented data [Address class imbalance]**
  - Create a CNN model, which can accurately detect 9 classes present in the dataset. While building the model rescale images to normalize pixel values between (0,1).
  - Choose an appropriate optimiser and loss function for model training
  - Train the model for ~20 epochs
  - Write your findings after the model fit, see if the earlier issue is resolved or not?
**Class distribution: **
  - Examine the current class distribution in the training dataset 
  - Which class has the least number of samples?
  - Which classes dominate the data in terms of the proportionate number of samples?
**Handling class imbalances:** 
  - Rectify class imbalances present in the training dataset with Augmentor library.
**Model Building & training on the rectified class imbalance data & augmentation:**
  - Create a CNN model, which can accurately detect 9 classes present in the dataset. While building the model rescale images to normalize pixel values between (0,1).
  - Choose an appropriate optimiser and loss function for model training
  - Train the model for ~20 epochs
  - Write your findings after the model fit, see if the issues are resolved or not?
 
## Conclusions
- The final model used the Augmentor library to artificially generate enough samples to come up with a model that can detect a correct cancer type with a validation accuracy around 93 %. 
- The validation loss for the final model was 0.17

 

The model training may take time to train and hence you can use Google colab.


## Contact
Created by [@kunal449] - feel free to contact me!