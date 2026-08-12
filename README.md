
# Customer Churn Prediction – Case Study

## Project Overview

**Customer Churn Prediction** is a Machine Learning case study focused on identifying customers who are likely to leave a banking service. The project analyzes customer demographics, transaction behavior, credit card usage, and financial attributes to understand the key factors associated with customer attrition and develop a predictive model for proactive customer retention.

The dataset contains customer information such as **Gender, Marital Status, Card Category, Transaction Count, Transaction Amount, Revolving Balance, and Attrition Flag**. The target variable, **Attrition_Flag**, is used to classify customers into existing and attrited customer groups.

## Objective

The primary objective of this project is to build an effective classification model capable of identifying customers who are at risk of churn. Since failing to identify an actual churner can result in customer and revenue loss, **Recall** is considered an important evaluation metric. The project focuses on maximizing recall while maintaining a good balance between **Accuracy, Precision, Recall, and F1-Score**.

## Methodology

The project follows a complete Machine Learning workflow, beginning with data exploration, data cleaning, preprocessing, and feature analysis. Categorical variables such as **Marital Status** and **Card Category** are transformed using n-1 dummy encoding, while the **Gender** variable is encoded using Label Encoding.

The dataset is divided into **70% training data and 30% testing data**, while maintaining the same proportion of the target classes in both datasets.

Three classification algorithms are developed and evaluated:

* **Decision Tree Classifier**
* **Random Forest Classifier**
* **Gradient Boosting Classifier**

Each model is evaluated using **Accuracy, Precision, Recall, and F1-Score** on both training and testing datasets.

## Model Selection

The Decision Tree model achieved high training performance but showed signs of overfitting, with lower precision and recall on unseen test data. Random Forest improved generalization and achieved strong test performance.

The **Gradient Boosting Classifier** provided the best overall balance between training and testing performance, achieving **0.96 test accuracy, 0.93 precision, 0.81 recall, and 0.86 F1-score**. It also demonstrated less overfitting compared with the Decision Tree and Random Forest models.

Therefore, **Gradient Boosting was selected as the final model** for customer churn prediction.

## Feature Importance

Feature importance analysis identified the following as the **top three factors influencing customer churn**:

1. **Total Transaction Count**
2. **Total Transaction Amount**
3. **Total Revolving Balance**

These findings indicate that customer engagement, spending behavior, and revolving balance are important indicators of potential attrition.

## Hyperparameter Tuning

The Gradient Boosting model was further optimized using **GridSearchCV** with recall as the scoring metric. The tuned model uses parameters including **125 estimators, a learning rate of 0.01, maximum tree depth of 4, and a subsample ratio of 0.5**. Fine-tuning improved the model's test recall, making it better suited for identifying customers who are likely to churn.

## Business Recommendations

The analysis provides actionable strategies for customer retention:

* Increase engagement among customers with low transaction activity through targeted rewards and marketing campaigns.
* Encourage higher spending through personalized cashback, promotions, and loyalty programs.
* Provide financial support and flexible repayment options for customers with high revolving balances.
* Use churn predictions to identify at-risk customers early and implement targeted retention strategies.

## Project Outcome

This case study demonstrates the practical application of **Exploratory Data Analysis, Feature Engineering, Classification Algorithms, Model Evaluation, Hyperparameter Tuning, Feature Importance, and Business Decision-Making** to a real-world customer retention problem.

The final solution can help financial institutions identify high-risk customers, understand the major drivers of churn, and implement **data-driven customer retention strategies** to reduce attrition and improve customer relationships.

## Technologies Used

**Python | Pandas | NumPy | Matplotlib | Seaborn | Scikit-learn | Jupyter Notebook**

**Project Focus:** Customer Churn Prediction | Classification | Customer Retention | Machine Learning | Business Analytics
