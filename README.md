# employee-churn-analysis-prediction:Project Overview

Understanding why and what kind of  employees are most likely to leave can lead to actions to improve employee retention as well as possibly planning new hiring in advance.Goal of this project:Utilizing both descriptive and inferential statistical approach to understand the key drivers of churn happening within the company and build a model that can predict employee churn.
<li>Created a tool that predicts the likelihood of employee churn (accuracy:86%) and identified key features of churn to help management in  making strategic changes to improve retention .</li>
<li>Engineered and analysed dataset feature columns and applied transformation to categorical fields</li>
<li>Optimized Logistic and Random Forest Regressors using GridsearchCV to reach the best model.</li>
<li>Utilized Random Forest's Feature Importance to identify key feature for the prediction model </li>

This is the repo for my second capstone project and it falls under "HR Analytics".From Sep 2019 to April 2020 I completed a number of projects as part of the Springboard Data Analytics Track.


# Code and Resources Used
<li>Python Version: 3.7</li>
<li>Packages: pandas, numpy, sklearn, matplotlib, seaborn</li>
<li>kaggle article: https://www.kaggle.com/hamzaben/employee-churn-model-w-strategic-retention-plan</li>

**Dataset:**
In this case study, a  fictional HR dataset was sourced from **IBM HR Analytics Employee Attrition & Performance** which contains various numerical and categorical features of employee data . I will use this dataset **Capstone2_HR** to predict core key drivers of employee churn.

But for practical purpose :I have named the company "**Star line Co.**" and have created Problem Statement and Issue trees around a fictitious context.

# EDA
I looked at the distributions of the data and the value counts for the various categorical variables. Below are a few highlights from the countplot .

![alt text](https://github.com/waibazen/employee-churn-analysis-prediction/blob/master/eda.png "Logo Title Text 1")

# Model Building
First, I transformed the categorical variables into dummy variables. I also split the data into train and tests sets with a test size of 30%.

I tried two different models and evaluated them using confusion matrix. I chose Precision and accuracy because data set is fairly imbalanced and company prioritizes to optimize its model on predicting less false positive i.e. employee who left but were labelled as active employee.

I tried two different models:

A)Logistic Regression – Baseline for the model
B)Random Forest – without feature engineering the data, I thought that this would be a good fit.

# Model performance
The Random Forest model r outperformed the logistic regression on the test and validation sets based on our business rule:

1. Random Forest :
Accuracy = 0.86,Precision =0.80, Recall=0.17
2. Logistic Regression:
Accuracy = 0.75,Precision =0.36, Recall=0.73



