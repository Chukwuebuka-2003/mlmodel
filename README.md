# mlmodel
Supervised Learning Model test


# Logistic Regression and RandomForestClassifier Model for Diabetes Prediction

This repository contains a simple implementation of a logistic regression and RandomForestClassifier model for predicting diabetes based on various features. The model is trained on a dataset containing information related to diabetes symptoms.

## Dataset

The dataset used for training the model includes the following features:

['Age', 'Gender', 'Polyuria', 'Polydipsia', 'sudden weight loss',
       'weakness', 'Polyphagia', 'Genital thrush', 'visual blurring',
       'Itching', 'Irritability', 'delayed healing', 'partial paresis',
       'muscle stiffness', 'Alopecia', 'Obesity', 'class']

The target variable is the 'class', indicating the presence or absence of diabetes.

I started by training the RandomForestClassifier model on the data based on the available features. A classification report and confusion matrix was done. The result was this: 

![image](https://github.com/Chukwuebuka-2003/mlmodel/assets/56232734/d25d33cf-d744-4fd9-b11f-400f44381dcb)

I now used feature importance to select the best features and trained another RandomForestClassifier Model on the data now based on the selected features (these features were selected on a threshold of >0.05). 
A classification report and confusion matrix was done on it, below is the result:

![image](https://github.com/Chukwuebuka-2003/mlmodel/assets/56232734/02ea1cb8-7417-40fe-9a25-b9a1e1f4960e)

The next method i implemented was SelectFromModel. I used this on the data set and RandomForestClassifier. 
SelectFromModel is used to automatically select features based on their importance scores with a specified threshold.
A classification report, the features selected and confusion matrix was done. Below is the result:

![image](https://github.com/Chukwuebuka-2003/mlmodel/assets/56232734/01b5152e-ea5f-4be9-888b-ebb366767657)

![image](https://github.com/Chukwuebuka-2003/mlmodel/assets/56232734/c1a79cbe-9c6d-4890-88e1-e6ab32bfa1c5)

The complete analysis can be found in the notebook in this repository
