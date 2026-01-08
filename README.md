# Proactive Insights for Employee Well-being: Predicting Burnout with Machine Learning

## Capstone Project | NeuroWell Analytics

## Project Overview
Employee burnout is a growing global concern, affecting productivity, engagement, and mental health in the workplace. This project, built for NeuroWell Analytics, applies machine learning techniques to predict employee burnout using historical workplace and well-being data.
The goal is to help organizations take proactive action based on data-driven insights.

Objectives
- Understand burnout trends using Exploratory Data Analysis (EDA)
- Preprocess and engineer features to improve model performance
- Build regression models to predict employee Burn Rate
- Identify key burnout drivers using model interpretation
- Recommend interventions to reduce burnout and improve workplace wellness

Dataset
Files:
- train.csv — training dataset
- test.csv — testing dataset

Features:

Feature              	          Description
- Employee ID           -      Unique identifier
- Date of Joining	      -      Start date at the company
- Gender	              -      Male / Female
- Company               -      Type	Service or Product company
- WFH Setup Available	  -      Whether proper remote setup exists
- Designation	          -      Seniority level
- Resource Allocation	  -      Hours assigned per day
- Mental Fatigue        -      Score	Self-reported fatigue level
- Burn Rate	            -      Target variable (rate of burnout)

Exploratory Data Analysis
- Burn Rate distribution shows moderate right skew
- High burnout is associated with higher mental fatigue and workload
- WFH setup appears to slightly reduce burnout rates
- Junior staff show higher burnout risk

Data Preprocessing and Feature Engineering
- Imputed missing values using median and mode
- Applied binary encoding to categorical variables (Gender, Company Type, WFH Setup)
- Extracted employee Tenure (in years) from Date of Joining
- Removed Employee ID as it is not predictive

Model Development
Models Tested:
- Linear Regression
- Random Forest Regressor
- Gradient Boosting Regressor

Best Model: Tuned Gradient Boosting Regressor
- Metric	Value
- R²	0.9044
- RMSE	0.0603
- MAE	0.0474

Key Features Driving Burnout
Top predictors identified:
- Mental Fatigue Score
- Resource Allocation
- Tenure
- Designation

Insight
High fatigue and workload are strong indicators of burnout. Newer employees and those in junior roles are more vulnerable. WFH setup has modest influence.

Sample Prediction Output
- Employee ID	Predicted Burn Rate
- fffe31003300390039003000	0.6170
- fffe33003400380035003900	0.3670
- ...	...

Recommendations
- Introduce fatigue tracking and wellness check-ins
- Rebalance workload for high-risk employees
- Promote flexible work options (e.g., WFH or hybrid)
- Strengthen onboarding and support for new employees

Tools and Libraries
- Python
- Pandas, NumPy
- Seaborn, Matplotlib (for visualization)
- Scikit-learn (for modeling and tuning)
- Jupyter Notebook

Author
- Keho Olamide Stella
- Aspiring Data Scientist | Economics Graduate  
- [GitHub](https://github.com/Stellabigeal)  
- [LinkedIn](https://www.linkedin.com/in/olamide-keho-47a865244)

Project Status
- Completed




