# Taiwanese Bankruptcy Prediction Case Study

## Overview

This case study aims to predict the risk of bankruptcy for companies using the Taiwanese Bankruptcy Prediction dataset. The dataset contains financial attributes collected from the Taiwan Economic Journal for the years 1999 to 2009. The classification task involves building Bagging and Boosting Classifier models to predict bankruptcy risk based on the dataset features.

## Dataset

### Origin and Objective
The data were collected from the Taiwan Economic Journal, defining bankruptcy based on the business regulations of the Taiwan Stock Exchange. The dataset consists of 96 columns, with the first attribute (Y) being the class label indicating bankruptcy.

### Features
- X1 to X95 represent various financial attributes, including Cost of Interest-bearing Debt, Cash Reinvestment Ratio, Current Ratio, and more.

## Data Preprocessing

### Exploratory Data Analysis
- Checking for missing values and duplicates.
- Renaming columns to lowercase and removing spaces.
- Exploring the distribution of the target variable 'bankrupt?'.

### Feature Engineering
- Handling features related to net income and outliers.

### Data Scaling and Splitting
- Scaling features using RobustScaler.
- Splitting the data into training and testing sets.

## Model Training - Bagging Classifiers

### SVM with Bagging
- Utilizing a Support Vector Machine (SVM) as the base estimator for Bagging.
- Training a BaggingClassifier and evaluating performance.

### Random Forest with Bagging
- Training a RandomForestClassifier with Bagging.
- Evaluating the performance of the ensemble model.

### NearMiss Undersampling
- Employing NearMiss undersampling technique.
- Training a RandomForestClassifier with Bagging using the undersampled data.

## Model Training - Boosting Classifiers

### Gradient Boosting
- Training a GradientBoostingClassifier using undersampled data.
- Evaluating the model's performance.

### XGBoost
- Training an XGBClassifier using undersampled data.
- Evaluating the performance of the XGBoost model.

## Model Training - Oversampling

### Random OverSampling
- Performing Random OverSampling.
- Training a BaggingClassifier with SVM using oversampled data.
- Evaluating the performance of the oversampled model.

### Gradient Boosting with Oversampling
- Training a GradientBoostingClassifier with oversampled data.
- Evaluating the model's performance.

### XGBoost with Oversampling
- Training an XGBClassifier with oversampled data.
- Evaluating the performance of the XGBoost model.

## Results

- Presenting the results of each model's classification report.

## Additional Libraries

- imbalanced-learn for sampling techniques.
- xgboost for XGBoost Classifier.

## Conclusion

This case study demonstrates the application of Bagging and Boosting Classifier models in predicting the risk of bankruptcy for Taiwanese companies. The choice of undersampling and oversampling techniques is explored to address class imbalance.

## Author

Ilaha Musayeva
09/17/23

**Disclaimer:** The dataset used for this analysis is from the Taiwan Economic Journal, and bankruptcy is defined based on the Taiwan Stock Exchange business regulations. Interpretation should be cautious.
