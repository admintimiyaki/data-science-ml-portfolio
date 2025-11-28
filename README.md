# Data Science & Machine Learning Portfolio

- **Name:** Temur Rustamov
- **Student ID:** C00280204
- **Module:** Data Science & Machine Learning
- My LinkedIn: www.linkedin.com/in/rustamovt


## Portfolio Specification

### Overview

This portfolio demonstrates my project work for the Data Science & Machine Learning module, covering both **regression** and **classification** problems using real-world datasets.

The projects showcase skills in:

- data preprocessing and feature engineering,  
- exploratory data analysis and visualisation,  
- model building and evaluation,  

using **Python** with libraries such as **pandas**, **NumPy**, **matplotlib**, **seaborn**, and **scikit-learn**.

Each portfolio item represents a different prediction task:

| Project                            | Type           | Dataset                     | Main Algorithm      | Objective                                           |
| ---------------------------------- | -------------- | --------------------------- | ------------------- | --------------------------------------------------- |
| **Wine Quality pH Analysis**       | Regression     | Red Wine Quality Dataset    | Linear Regression   | Predict pH values from chemical attributes          |
| **SMS Spam Classification**        | Classification | SMS Spam Collection Dataset | Naive Bayes         | Classify text messages as spam or legitimate (ham)  |
| **Titanic Survival Prediction**    | Classification | Titanic Passenger Data      | Random Forest       | Predict passenger survival (0/1) on the Titanic     |

---

## Objectives

The goal of this portfolio is to:

1. Demonstrate the implementation of end-to-end machine learning models.
2. Apply **Linear Regression** for regression tasks and evaluate performance using metrics such as **R²**.
3. Apply **Naive Bayes** and **Random Forest** for classification tasks and evaluate performance using **accuracy**.
4. Interpret model performance, identify key factors influencing predictions, and present results in a clear, professional way.

---

## Project Descriptions

### **Wine Quality pH Analysis – Linear Regression**

This project analyses how the chemical composition of red wine affects its acidity (pH).  
Using simple and multiple **Linear Regression**, the model predicts the pH level based on several chemical features (e.g. fixed acidity, citric acid, density, sulphates, alcohol).

- **Key methods:**  
  - Correlation analysis and visualisation  
  - Feature selection and scaling  
  - Simple and multiple linear regression  
  - Residual and predicted vs actual plots

- **Outcome:**  
  - The final model achieved an R² of approximately **0.65**, indicating moderate to strong predictive performance for pH.

- **Interpretation:**  
  - **Fixed acidity** showed the strongest negative relationship with pH (higher fixed acidity → lower pH → more acidic wine).  
  - **Density** and **alcohol** also contributed to predicting pH, along with other chemical attributes.

---

### **SMS Spam Classification – Naive Bayes**

This project applies **Naive Bayes** classification to detect spam messages.  
Using the SMS Spam Collection dataset, the model learns to distinguish between spam and ham (legitimate) text messages.

- **Key methods:**  
  - Train–test split  
  - Text vectorisation using **CountVectorizer** (bag-of-words)  
  - Multinomial Naive Bayes classifier

- **Evaluation:**  
  - Model performance is evaluated using **accuracy** on a held-out test set.

- **Outcome:**  
  - The model achieved high accuracy on the test data and correctly classified typical spam phrases as spam, while recognising normal conversational messages as ham.

---

### **Titanic Survival Prediction – Random Forest**

This project uses a **Random Forest** classifier to predict whether a passenger on the Titanic survived (`Survived = 1`) or not (`Survived = 0`), based on features such as class, sex, age and embarkation port.

- **Key methods:**  
  - Data exploration and correlation analysis  
  - Stratified train–test split to preserve survival/class/sex distributions  
  - Custom preprocessing pipeline:
    - `AgeImputer` (impute missing Age values)
    - `FeatureEncoder` (one-hot encode categorical features such as Sex and Embarked)
    - `FeatureDropper` (remove unused text/high-cardinality columns)
  - Feature scaling with **StandardScaler**  
  - **RandomForestClassifier** with **GridSearchCV** for hyperparameter tuning  
  - Generating a prediction CSV (`PassengerId`, `Survived`) suitable for submission (e.g. Kaggle format)

- **Evaluation:**  
  - Model performance is evaluated using **accuracy** on an internal stratified test split.

- **Outcome:**  
  - The tuned Random Forest model achieved good accuracy, confirming that **Sex** and **Pclass** (and related features) are strong predictors of survival.  

