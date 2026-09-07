# Employee Attrition Prediction with HR Analytics

A machine learning project that analyzes employee data and predicts employee attrition using classification algorithms.

##  Project Overview

Employee attrition can have a significant impact on an organization. Understanding the factors associated with employee turnover can help organizations identify potential attrition risks.

This project uses the IBM HR Employee Attrition dataset to explore employee-related factors and build machine learning models for predicting whether an employee is likely to leave the organization.

The project covers data preprocessing, exploratory data analysis, feature encoding, feature scaling, model training, evaluation, and feature importance analysis.

##  Objectives

- Analyze employee data and understand attrition patterns.
- Identify important factors associated with employee attrition.
- Preprocess and transform the dataset for machine learning.
- Train and compare multiple classification models.
- Evaluate model performance using different metrics.
- Analyze important features influencing the prediction.
- Perform a sample employee attrition prediction.

## 📊 Dataset

The project uses the **IBM HR Employee Attrition dataset**.

- **Total records:** 1,470
- **Original features:** 35
- **Target variable:** Attrition
- **Target classes:** Yes / No

The dataset contains employee information such as:

- Age
- Department
- Job Role
- Monthly Income
- Job Satisfaction
- Overtime
- Distance From Home
- Total Working Years
- Years at Company
- Business Travel
- Work-Life Balance
- And other employee-related attributes

##  Data Preprocessing

The following preprocessing steps were performed:

1. Removed unnecessary columns:
   - EmployeeCount
   - EmployeeNumber
   - Over18
   - StandardHours

2. Converted categorical variables into numerical features using **One-Hot Encoding**.

3. Applied **StandardScaler** for feature scaling.

4. Split the dataset into:
   - 80% Training data
   - 20% Testing data

##  Exploratory Data Analysis

The project includes:

- Employee attrition distribution analysis
- Correlation heatmap
- Decision tree visualization
- Model accuracy comparison
- Confusion matrix
- ROC curve
- Feature importance analysis

##  Machine Learning Models

Three classification algorithms were trained and compared:

1. Logistic Regression
2. Decision Tree Classifier
3. Random Forest Classifier

##  Model Performance

| Model | Test Accuracy |
----------------------------------
| Logistic Regression | 88.10% |
| Decision Tree | 86.73% |
| Random Forest | 87.76% |

Logistic Regression achieved the highest test accuracy among the three models at **88.10%**.

Random Forest was further analyzed using cross-validation, confusion matrix, ROC-AUC analysis, and feature importance.

##  Cross-Validation

A 5-fold cross-validation was performed for the Random Forest model.

**Average Cross-Validation Accuracy: 85.71%**

##  Random Forest Evaluation

The Random Forest model achieved:

- **Accuracy:** 87.76%
- **AUC:** 0.753

The classification report, confusion matrix, and ROC curve are included in the notebook.

## ⭐ Important Features

The Random Forest feature importance analysis identified several influential features, including:

1. Monthly Income
2. Overtime
3. Age
4. Daily Rate
5. Monthly Rate
6. Total Working Years
7. Distance From Home
8. Hourly Rate
9. Years at Company
10. Number of Companies Worked

##  Sample Prediction

The project also demonstrates a sample employee attrition prediction using the trained Random Forest model.

The model predicts whether an employee is likely to:

- **Stay**
- **Leave**

##  Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn
- Google Colab
- Jupyter Notebook

## 📁 Repository Contents

```
Employee-Attrition-Prediction/
│
├── EMPLOYEE_ATTRITION.ipynb
└── README.md
