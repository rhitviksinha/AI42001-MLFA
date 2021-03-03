# LAB 6

## Wednesday, 4<sup>th</sup> November, 2 - 5 PM

# Assignment 6

The third assignment is **Hand gesture Classification using SVM**.

### Dataset

There is a dataset provided of sign language using hand gestures ([Link](https://drive.google.com/file/d/1wK-AS0h_n-5L-5gYiKV3VlR4Wlp25aoC/view?usp=sharing)). So there are 10 classes each classes having 3000 images. All the images are in RGB format. You need to perform the following steps.

### Description:

1. Convert the image into binary image. From each class in the dataset use 70% for training and 30% for testing.

2. Extract features from these and store them in a csv file (features should be chosen by you - eg. binary pixel vectors, total number of white pixels, local binary patterns). Represent each image using such features. **[2 marks]**

3. Use the features for classification using SVM (default setting). Print classification report. **[3 marks]**

4. Apply grid search for hyper-parameter tuning.(eg: kernel, C, gamma). **[3 marks]**

5. Report the model with best accuracy. **[2 marks]**

*Rescale the image as per requirement.*