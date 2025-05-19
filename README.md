# students performance Prediction Project

# Introduction

* Student performance prediction is a critical area of educational research. Understanding the factors that influence student success can help educators 
  design better curricula and interventions. This project aims to analyze students' academic data and develop a predictive model to estimate their 
  performance index based on various input features.

# Dataset Overview
  The dataset consists of 10,000 entries with six features:
* Hours Studied (Numerical)
* Previous Scores (Numerical)
* Extracurricular Activities (Categorical)
* Sleep Hours (Numerical)
* Sample Question Papers Practiced (Numerical)
* Performance Index (Target Variable - Numerical)

# Data Source
* https://github.com/TheMLengineer07/students__performance-model/blob/main/Student_Performance.csv

# Exploratory Data Analysis(EDA)

  Key Finding From EDA:
* Most students study 1 hour, but performance increases with more study hours.
* 50% of students scored above 65 in previous exams.
* Most students do not participate in extracurricular activities.
* The more students sleep, the higher their Performance Index.
* A strong positive correlation exists between Performance Index and features like Hours Studied, Previous Scores, and Sample Question Papers Practiced.
# Data Preprocessing
* Categorical Encoding: Extracurricular Activities were encoded using LabelEncoder().
* Splitting Data: The dataset was split into training (80%) and testing (20%) datasets.
* Feature Scaling: MinMaxScaler could be applied to normalize the numerical data.

# Model Developement
* A Linear Regression Model was built using sklearn

# Model Performance
* Training Score (R²): 0.9886
* Testing Score (R²): 0.9889
* Mean Absolute Error: 1.612
Coefficients:
* Hours Studied: 2.85
* Previous Scores: 1.01
* Extracurricular Activities: 0.60
* Sleep Hours: 0.47
* Sample Question Papers Practiced: 0.19
* Intercept: -33.92

# Model Deployment
* The trained model was saved using pickle for future predictions.
* The model is highly accurate, showing strong predictive capability for student performance.

# Conclusion

* The analysis confirms that studying hours, previous scores, and question paper practice significantly impact student performance. Sleep hours and 
  extracurricular activities show a lesser effect, but maintaining a balance in both areas is advisable for better performance.
