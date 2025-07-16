 Proactive Insights for Employee Well-being: Predicting Burnout with Machine Learning
 Capstone Project | NeuroWell Analytics
 Project Overview
Employee burnout is a growing global concern, affecting productivity, engagement, and mental health in the workplace. This project, built for NeuroWell Analytics, applies machine learning techniques to predict employee burnout using historical workplace and well-being data. The goal is to help organizations take proactive action based on data-driven insights.

 Objectives
Understand burnout trends using Exploratory Data Analysis (EDA)
Preprocess and engineer features to improve model performance
Build regression models to predict employee Burn Rate
Identify key burnout drivers using model interpretation
Recommend interventions to reduce burnout and improve workplace wellness

 Dataset
Train set: train.csv
Test set: test.csv

Each record includes:
Feature	                  Description
Employee ID	              Unique identifier
Date of Joining	          Start date at the company
Gender	                  Male / Female
Company Type	            Service or Product company
WFH Setup Available	      Whether proper remote setup exists
Designation	              Seniority level
Resource Allocation	      Hours assigned per day
Mental Fatigue Score	    Self-reported fatigue
Burn Rate	                Target variable (rate of burnout)

Exploratory Data Analysis
Burn Rate distribution shows moderate right skew
High burnout is linked to high mental fatigue and high workload
WFH setup appears to slightly reduce burnout rates
Designation correlates moderately with burnout (junior staff are more affected)

Data Preprocessing & Feature Engineering
Missing values imputed (median/mode)
Binary encoding for categorical variables
Extracted Tenure in years from Date of Joining
Removed Employee ID as it’s not predictive

Model Development
Tested models:
Linear Regression
Random Forest Regressor
Gradient Boosting Regressor

Best model: Tuned Gradient Boosting Regressor
R²: 0.9044 | RMSE: 0.0603 | MAE: 0.0474

Key Features Driving Burnout
Top predictive features:
Mental Fatigue Score
Resource Allocation
Tenure
Designation

InsightsHigh fatigue and workload are clear drivers of burnout. Newer employees and junior roles are especially vulnerable. WFH availability has modest impact.

Sample Prediction Output
Employee ID	Predicted Burn Rate
fffe31003300390039003000	0.6170
fffe33003400380035003900	0.3670
...	...

Recommendations
Implement fatigue tracking and wellness check-ins
Rebalance workload for high-risk employees
Promote flexibility (WFH and hybrid options)
Onboard new staff with support programs

Tools & Libraries
Python, Pandas, NumPy
Seaborn & Matplotlib (EDA)
Scikit-learn (modeling, tuning)
Jupyter Notebook

Author
Keho Olamide Stella 
Aspiring Data Scientist | Economics Graduate  
[GitHub](https://github.com/Stellabigeal)  
[LinkedIn](https://www.linkedin.com/in/olamide-keho-47a865244)

Status
✅ Completed
Future Work: Streamlit deployment or SHAP explanations
