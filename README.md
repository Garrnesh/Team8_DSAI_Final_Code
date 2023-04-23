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

# Machine Learning Models (Contrubtued by S Jivaganesh)
1. Decision Tree

For the decision tree, we used a RandomSearchCV to be able to find the most optimal depth of our tree, so that our model will be able to perform optimally.
We identified that a depth of 3 is the most optimal depth and used it in the model and obtained the required metrics.

3. Random Forest

For the random forest, we used a RandomSearchCV to be able to find the optimal depth of tree and optimal number of trees. The optimal depth was 10 and the number of trees were 340. We then used it in the model and obtained the required metrics.

5. Logistic Regression

For the logistic regression, we used a GridSearchCV instead to do a full extensive search for the most optimal hyperparameter combination. For this model we tuned the "C" hyperparameter, which is regularisaiton strength, and obtained the solver used to optimise our loss function. The hyperparameters were 0.1 and "liblinear" respectively. We then built the model and obtained the required metrics.

7. Support Vector Machine

For SVM, we also used a GridSearchCV to tune the hyperparameters which are the "C" value and the kernal, which is used to determine how the data will be transformed into a higher-dimensional feature space. The hyperparameters were 1 and "rbf" respectively


We used 4 model metrics to pick our final model. Accuracy, Precision, Recall and F1 Score. We picked Accuracy and Recall to be the most important metrics used to evaluate our model. Accuracy is able to tell us how well our model was able to correctly classify the tumors. Recall gives us an indication of how well the model is able to avoid False Negatives, which is imperative for cancer diagnosis as we want to coorectly idenfiy cancerous tumor so that we can provide immediate care for the patient. Using those metrics we found that logistic regression yields the best results for Accuracy and Recall, where Accuracy was 99.13% and Recall was 96.67%.

# What we learnt from this project
1. Cleaning of unnecessary data
2. Standard scaling to scale large values
3. Heatmap to find highly correlated variables
4. Using standard scaling to fit data into Logistic Regression and SVM
5. Implementing Decision Tree, Random Forest, SVM and Logistic Regression classification Models
6. Hyperparameter tuning for Machine Learning Models
7. Evaluating models based on Accuracy, Precision, Recall and F1 Score


# Contributions


# References
* https://www.kaggle.com/datasets/uciml/breast-cancer-wisconsin-data
* https://www.bmj.com/content/353/bmj.i2314#:~:text=Principal%20findings,with%20a%20stable%20alcohol%20intake. 
* https://www.cancer.org/cancer/breast-cancer/about/how-common-is-breast-cancer.html#:~:text=Breast%20cancer%20mainly%20occurs%20in,cancer%20are%20younger%20than%2045. 
* https://www.cdc.gov/cancer/breast/young_women/bringyourbrave/breast_cancer_young_women/index.htm#:~:text=About%201%20in%208%20women,than%2045%20years%20of%20age.



