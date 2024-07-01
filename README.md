
# Principal Component Analysis on Heart Disease Dataset

  

## Overview:

This project explores the application of Principal Component Analysis (PCA) on a heart disease dataset obtained from Kaggle. The objective is to reduce the dimensionality of the dataset and assess the impact on model performance using various classifiers.

## Dataset:

Kaggle: [Heart Disease Dataset](https://www.kaggle.com/fedesoriano/heart-failure-prediction)


## Data Preprocessing:

  

#### 1. Outlier Removal:

- Outliers were identified and removed using the Z-score method. Data points with Z-scores above 3 or below -3 were excluded to ensure the dataset's integrity.

  

#### 2. Standardization:

- Numerical features were standardized to have a mean of 0 and a standard deviation of 1. This step is crucial for PCA to ensure that each feature contributes equally to the analysis.

  

#### 3. Categorical Data Handling:

- Categorical variables were converted into numerical format using one-hot encoding (dummies).

  

## PCA Application:

  

- PCA was applied iteratively, varying the number of components from 1 to 10. The aim was to determine the optimal number of components that balance dimensionality reduction with model performance.

  

## Model Training and Evaluation:

Three classifiers were used to evaluate the performance of the reduced dataset:

  

1. Logistic Regression

2. K-Nearest Neighbors Classifier (KNN)

3. Random Forest Classifier

  

## Results:

  

#### Logistic Regression:

- Using 5 principal components resulted in an accuracy score of 85%.

- Using all original features (13), the accuracy score was approximately 86.6%.

  

## Conclusion:

The PCA effectively reduced the dataset's dimensionality while maintaining a comparable model performance. Logistic Regression, with 5 principal components, achieved a high accuracy close to the full feature set, demonstrating the effectiveness of PCA in simplifying the dataset without significant loss of information.