# Graduate Prediction Model
Project Overview
This project implements a machine learning model designed to predict whether a student will graduate or drop out based on key academic and financial factors. The purpose is to identify strong indicators of student success and help educational institutions proactively support at-risk students, ultimately improving retention rates.

By analyzing historical data related to students' academic performance, tuition fee status, and other factors, the model offers valuable insights to assist institutions in creating targeted interventions and support mechanisms.

# Problem Statement
Student retention is a crucial challenge for educational institutions. By identifying students who are at risk of dropping out, schools and universities can intervene and provide additional support to help these students succeed. This project builds a predictive model to forecast whether a student will graduate or drop out based on the following features:

# Academic performance in the first and second semesters
Financial status, such as tuition fee payments and scholarship eligibility
Dataset & Features
The dataset used for training the model contains information about various student attributes. The selected features used to predict whether a student will graduate or drop out include:

Curricular units 2nd sem (approved): Whether the student passed their 2nd-semester courses.
Curricular units 2nd sem (grade): The grade received in the 2nd-semester courses.
Curricular units 1st sem (approved): Whether the student passed their 1st-semester courses.
Curricular units 1st sem (grade): The grade received in the 1st-semester courses.
Tuition fees up to date: Whether the student’s tuition fees are paid up to date.
Scholarship holder: Whether the student holds a scholarship.
The target variable, Target, is binary:

1: Graduate
0: Dropout

# Approach
Data Cleaning: Clean the dataset to remove missing values, inconsistencies, and outliers.
Feature Selection: Choose relevant features that are believed to influence student graduation.
Model Training: Train a machine learning model to predict student outcomes based on selected features.
Prediction: Use the trained model to predict if a student will graduate or drop out, based on input features.

# Selecting relevant features
selected_Features = [
    "Curricular units 2nd sem (approved)",
    "Curricular units 2nd sem (grade)",
    "Curricular units 1st sem (approved)",
    "Curricular units 1st sem (grade)",
    "Tuition fees up to date",
    "Scholarship holder"
]

# Preparing input data
X = df[selected_Features] 
y = df["Target"]  # Target variable (Graduate or Dropout)

# Results
After running the model, it will output predictions on whether a student will graduate or drop out. This can help institutions identify at-risk students and provide additional resources or support to improve retention.

# Conclusion
This project demonstrates how machine learning can be applied to educational data to predict student success and help improve retention rates. By identifying students who are at risk of dropping out, institutions can intervene early and provide the support needed to help these students graduate successfully.
