# Water Pump Status Classification - Machine Learning Project

This project was developed for a continuous open data competition in which the goal was to predict the functional status of water pumps based on a rich dataset containing over 50 variables.

Participants were evaluated based on the performance of their predictive models in a real-world simulation. This project demonstrates a full end-to-end machine learning workflow, including preprocessing, model selection, and submission formatting.

## Problem Description

The dataset includes technical, geographical, and usage-related information about water pumps. The objective is to predict the **status** of each pump, which can be one of the following three categories:

- `functional`
- `non functional`
- `needs repair`

This is a **multi-class classification problem** with an **imbalanced dataset** and common data science challenges such as:
- Missing values
- High-cardinality categorical variables
- Need for robust preprocessing and feature engineering

## Technologies Used 

- `pandas`, `numpy`, `seaborn`, `matplotlib`
- `scikit-learn`, `imblearn`, `xgboost`
- `missingno`, `SMOTE`, `Pipeline`, `GridSearchCV`, etc.

## Project Steps

1. **Exploratory Data Analysis (EDA)**
   - Visualization of missing data
   - Analysis of class distribution and feature types

2. **Preprocessing & Feature Engineering**
   - Handling missing values with `SimpleImputer` and `KNNImputer`
   - Encoding categorical variables (`OneHotEncoder`, `LabelEncoder`)
   - Feature scaling with `StandardScaler`, `RobustScaler`, and `MinMaxScaler`
   - Feature reduction with `PCA` (optional)

3. **Handling Imbalanced Data**
   - Resampling using `SMOTE` and `SMOTENC` for categorical variables

4. **Model Training & Evaluation**
   - Trained models: `RandomForestClassifier`, `XGBoost`, `GradientBoosting`, `KNN`
   - Cross-validation using `RepeatedKFold`
   - Model comparison using accuracy and classification metrics

5. **Hyperparameter Tuning**
   - Used `GridSearchCV` and `RandomizedSearchCV` for model optimization

6. **Final Prediction & Submission**
   - Predictions generated on the test set
   - Submission file formatted with required ID and predicted labels

## Sample Visuals

![image](https://github.com/user-attachments/assets/c9b11b85-2727-435d-b356-f8908e3aeb9c)


![image](https://github.com/user-attachments/assets/aa8cadb5-8573-420d-b0a0-78da284423f3)


This project was submitted as part of the Machine Learning module in the Big Data & Data Science Master's program.
