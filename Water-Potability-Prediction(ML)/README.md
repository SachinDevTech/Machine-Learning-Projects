# Water Potability Prediction

## Introduction
In this project, we aim to predict the potability of water using various parameters. We have performed Exploratory Data Analysis (EDA), data partitioning, normalization, and built models using Decision Tree and K-Nearest Neighbors (KNN) algorithms.

## Data Overview
The dataset contains information on 10 parameters:
- pH
- Hardness
- Solids
- Chloramines
- Sulfate
- Conductivity
- Organic_carbon
- Trihalomethanes
- Turbidity
- Potability (target variable: 1 if potable, 0 otherwise)

## Libraries Used
- Pandas
- Scikit-learn
- Seaborn

## Exploratory Data Analysis (EDA)
We performed EDA to understand the characteristics of our dataset. This involved:
- Checking for missing values
- Visualizing distributions and relationships among variables using Seaborn

## Data Preprocessing
- Partitioning the data into training and testing sets
- Normalizing the data to ensure all features have the same scale

## Model Building
### Decision Tree
We trained a Decision Tree classifier on the normalized data.
```python
# Code snippet for training Decision Tree
from sklearn.tree import DecisionTreeClassifier
dt_classifier = DecisionTreeClassifier()
dt_classifier.fit(X_train, y_train)
```


# K-Nearest Neighbors (KNN)
## We also trained a KNN classifier on the normalized data.
```python
#code 
from sklearn.neighbors import KNeighborsClassifier
knn_classifier = KNeighborsClassifier()
knn_classifier.fit(X_train, y_train) 
```

# Conclusion
After building and training our models, we evaluated their performance. The K-Nearest Neighbors (KNN) algorithm achieved an `accuracy of 0.923 on the training set` and `0.588 on the test set`, showing promising results for predicting water potability. Further optimizations and fine-tuning could enhance the model's performance further.
