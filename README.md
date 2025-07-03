# NHANES Age Group Classification

This project was built for a hackathon challenge focused on public health analytics. Using data from the National Health and Nutrition Examination Survey (NHANES), the objective is to predict whether an individual belongs to the *Senior (65+)* age group.

---

## Problem Statement

Given physical, lifestyle, and lab test features from NHANES, the goal is to develop a machine learning model that accurately classifies individuals as either *Adult* or *Senior (65+).*

---

## Tech Stack Used

- Python  
- Pandas  
- Scikit-learn (for preprocessing and modeling)  
- Jupyter Notebook  

---

## Architecture Flow

### Data Preprocessing
- Dropped unique identifier (SEQN)
- Handled missing values using mean imputation
- Encoded target variable: Adult → 0, Senior → 1
- Scaled numerical features using StandardScaler

### Model Training
- Used a RandomForestClassifier
- Split data into training and validation sets
- Evaluated model using accuracy and classification report

### Prediction
- Applied the same preprocessing to test data
- Predicted age group
- Exported predictions to submission.csv
