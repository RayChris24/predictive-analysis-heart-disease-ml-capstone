# Predictive Analysis of Heart Disease Using Machine Learning 🫀

## Project Overview
This capstone project involves building a machine learning classification pipeline to predict the risk of heart disease based on various health and lifestyle metrics. The goal is to identify key predictors and assist in early preventive healthcare using data-driven insights.

## Business Problem
Heart disease remains a leading cause of global mortality. Identifying high-risk individuals early can significantly improve preventative care and resource allocation in healthcare facilities. This project uses data science to analyze complex health-related data, identifying the most significant risk patterns to support early diagnosis.

## Dataset Details
* **Initial Size:** 319,795 observations and 18 features.
* **Post-Cleaning:** Reduced to 301,717 observations after identifying and removing 18,078 duplicate records.
* **Key Features Analyzed:** BMI, Smoking, AlcoholDrinking, Stroke, Physical/Mental Health, Age Category, Diabetic status, SleepTime, and GenHealth.

## Tech Stack & Methods Used
* **Language:** Python
* **Libraries:** Pandas, NumPy, Matplotlib, Seaborn, Scikit-Learn
* **Techniques:** Exploratory Data Analysis (EDA), Data Cleaning, Feature Engineering, Feature Scaling (StandardScaler), Hyperparameter Tuning (GridSearchCV).
* **Algorithms Evaluated:** Logistic Regression, Decision Tree, Random Forest, K-Nearest Neighbors (KNN), Support Vector Machine (SVM), Naive Bayes, and Gradient Boosting.

## Key Insights
* **Age & Disease Prevalence:** The likelihood of heart disease increases significantly with age, with higher prevalence observed in older age groups.
* **Class Imbalance:** EDA revealed a significant class imbalance, with individuals without heart disease drastically outnumbering those with the disease.
* **Top Predictors (Decision Tree):** Feature importance analysis indicated that **BMI** (35.1% importance) was the strongest predictor, followed by **SleepTime** (11.0%), **PhysicalHealth** (7.6%), and **MentalHealth** (6.5%).

## Model Performance
Multiple classification algorithms were rigorously evaluated. Because this is a medical dataset, models were assessed not just on baseline accuracy, but on their ability to reliably identify complex risk patterns. 

The top-performing models achieved the following accuracy scores:
* **Gradient Boosting (Best Model):** 91.16%
* **Support Vector Machine (SVM):** 91.16%
* **Logistic Regression (Baseline/Tuned):** 91.14%

**Other Models Evaluated:**
* **K-Nearest Neighbours (KNN):** 90.03%
* **Random Forest:** 89.80%
* **Decision Tree:** 85.57%
* **Naive Bayes:** 71.17%

*Note: Gradient Boosting and SVM provided the highest overall accuracy, making them the most robust choices for this specific classification task.The classification report for the best-performing model indicates strong precision (0.92) and recall (0.99) for negative cases, maintaining high overall accuracy while effectively analyzing complex lifestyle data*.

## How to Run This Project
1. Clone the repository to your local machine.
2. Ensure the `heart.csv` dataset is in the same directory as the notebook.
3. Run `capstone_heart_disease_prediction_ml.ipynb` using Jupyter Notebook or JupyterLab.
