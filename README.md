# End-Sem-Project
Udemy Course Popularity Prediction (XGBoost)
📌 Overview

This project focuses on predicting the popularity of Udemy courses using machine learning techniques. Popularity is measured by the number of ratings (rating_count), which reflects user engagement and enrolment.

The project applies data preprocessing, feature engineering, supervised learning models, and clustering techniques to analyze and predict course success.

🎯 Problem Statement
Goal: Predict course popularity (rating_count)
Type: Regression problem
Dataset Size: ~314K rows (~150MB)
Sampling: Reduced to 50K rows using stratified sampling (based on course level)
📊 Features Used

Key features used in the model include:

rating_average
duration_seconds
lectures_count
is_free
level
locale
practice_test_questions_count
Engineered features (text & date-based)
⚙️ Tech Stack
Language: Python
Libraries:
Pandas, NumPy
Scikit-learn
XGBoost
Matplotlib, Seaborn

🔄 Workflow
1. Data Loading & Inspection
Load dataset
Understand structure, missing values, and distributions
2. Data Preprocessing
Handle missing values
Encode categorical variables
Normalize/transform features
Log transformation of target (log1p)
3. Exploratory Data Analysis (EDA)
Distribution plots
Correlation analysis
Feature relationships
4. Feature Engineering
Extract meaningful insights from:
Text data
Dates
Create new predictive features
5. Train-Test Split
Split dataset into training and testing sets

🤖 Models Used
Model	Description
Ridge Regression	Linear baseline model
Random Forest	Ensemble bagging method
Gradient Boosting	Sequential boosting
XGBoost ⭐	Best performing model
Hyperparameter tuning done using RandomizedSearchCV

📈 Evaluation Metrics
RMSE (Root Mean Squared Error)
MAE (Mean Absolute Error)
MAPE (Mean Absolute Percentage Error)
R² Score

🧠 Unsupervised Learning
Applied clustering techniques to group similar courses
Helps identify patterns in course types and popularity

🏆 Key Insights
Course popularity is strongly influenced by:
Ratings (rating_average)
Content duration
Number of lectures
Paid vs free courses show different engagement trends
Feature engineering significantly improves performance
XGBoost outperforms other models due to better handling of non-linearity
