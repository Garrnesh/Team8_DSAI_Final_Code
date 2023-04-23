# Lab137_Team8_DSAI_Final_Code
# Overview
Our project aims to improve breast cancer prediction on whether the diagnosis is malignant or benign. We performed exploratory data analysis to help us better visualise the data and clean it for the training of our models. We also used 4 different machine models and a few model metrics to pick our choice of model.

# Problem objective
* Predict whether the cancer is malignant or benign more efficiently and accurately using machine learning based on strong predictors or variables

# File Description

1. "Exploratory_Data_Analysis.ipynb" contains out EDA for our Dataset.
2. "Machine_Learning_Models.ipynb" contains our training of our Machine Learning Models
3. "cancer.csv" is the CSV file of our dataset.

# Dataset


# Exploratory Data Analysis
1. Data Cleaning
2. Data visualisation
3. Heatmap and correlation

We dropped the columns that are unncessary for the training of our models and did standard scaling to scale the larger values so that the models are not dominated by it. We also found out through violin plots of individual variables that those variables with easily separable values could mean that the variables have some predictive power for classification. Through using a heatmap, we also found out which are the highly correlated variables to diagnosis as they are the stronger predictors.

# Machine Learning Models
1. Decision Tree
2. Random Forest
3. Logistic Regression
4. Support Vector Machine

We used 4 model metrics to pick our final model. Accuracy, Precision, Recall and F1 Score. The Accuracy and Recall metrics are the more important ones as it tells us the percentage of data that are classified accurately and the percentage of true positives (cancer being detected as malignant correctly). Using those metrics we found that logistic regression yields the best results for Accuracy and Recall. 

# What we learnt from this project
1. Cleaning of unnecessary data
2. Standard scaling to scale large values
3. Heatmap to find highly correlated variables


# Contributions


# References
* https://www.kaggle.com/datasets/uciml/breast-cancer-wisconsin-data
* https://www.bmj.com/content/353/bmj.i2314#:~:text=Principal%20findings,with%20a%20stable%20alcohol%20intake. 
* https://www.cancer.org/cancer/breast-cancer/about/how-common-is-breast-cancer.html#:~:text=Breast%20cancer%20mainly%20occurs%20in,cancer%20are%20younger%20than%2045. 
* https://www.cdc.gov/cancer/breast/young_women/bringyourbrave/breast_cancer_young_women/index.htm#:~:text=About%201%20in%208%20women,than%2045%20years%20of%20age.



