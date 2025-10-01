# Heart Disease Detection Using Machine Learning

## Overview
This project aims to predict the risk of heart disease in individuals using machine learning algorithms. Early detection of heart disease is crucial for timely intervention and better healthcare outcomes. Using a combination of **data preprocessing, visualization, and classification models**, this project identifies patterns in patient data and predicts the presence of heart disease.

---

## Project Workflow

### 1. Dataset
- The project uses the **Cleveland Heart Disease dataset** from the UCI Machine Learning Repository.  
- Focused on 13 key features like:
  - `age`, `sex`, `chest pain type (cp)`, `resting blood pressure (trestbps)`, `cholesterol (chol)`, `fasting blood sugar (fbs)`, `max heart rate (thalach)`, `exercise-induced angina (exang)`, `ST depression (oldpeak)`, `slope of peak exercise (slope)`, `number of major vessels (ca)`, `thal`.  
- The target variable is `disease_present` (0 = No, 1 = Yes).

---

### 2. Data Preprocessing
- Handled missing values and cleaned the dataset.  
- Converted categorical features to numeric using **Label Encoding**.  
- Split data into **training** and **testing** sets.  
- Applied **feature scaling** to standardize numeric variables.

---

### 3. Exploratory Data Analysis (EDA)
- Visualized data patterns using **bar plots, box plots, violin plots, and pair plots**.  
- Explored relationships between features and target variable.  
- Identified trends and correlations to guide model selection.

---

### 4. Classification Models
Three machine learning models were trained and evaluated:

| Model                  | Accuracy | Precision | Recall | F1 Score |
|------------------------|----------|-----------|--------|----------|
| Logistic Regression    | 77%      | 84%       | 78%    | 81%      |
| XGBoost                | 78%      | 84%       | 78%    | 81%      |
| Support Vector Machine (SVM) | 80% | 84%       | 83%    | 84%      |

- **SVM** performed best in terms of accuracy and recall, indicating it can reliably detect individuals with heart disease.  
- Logistic Regression and XGBoost also gave competitive results.
