# IND-ENG 242A: Machine Learning - HW2

Assignment for UC Berkeley's IND-ENG 242A course on machine learning.

## Overview

This homework assignment involves building a machine learning classification model to predict 10-year coronary heart disease (CHD) risk using the Framingham Heart Study dataset.

## Dataset

The project uses the Framingham Heart Study dataset with the following features:
- **Demographics**: `male`, `age`, `education`
- **Health Behaviors**: `currentSmoker`, `cigsPerDay`, `BPMeds`
- **Medical History**: `prevalentStroke`, `prevalentHyp`, `diabetes`
- **Vital Signs & Labs**: `totChol`, `sysBP`, `diaBP`, `BMI`, `heartRate`, `glucose`
- **Target Variable**: `TenYearCHD` (binary: 0 = no CHD, 1 = CHD within 10 years)

Data split: Training and test sets are provided separately.

## Methodology

The analysis includes:

1. **Data Preprocessing**
   - Categorical encoding (education level converted to dummy variables)
   - Exploratory data analysis with multicollinearity checks

2. **Model Development**
   - Support Vector Machine (SVM) classifier with GridSearchCV
   - Feature scaling using StandardScaler
   - Hyperparameter tuning

3. **Evaluation**
   - Confusion matrix
   - ROC curve and AUC
   - Classification report
   - Accuracy metrics

## Files

- `main.ipynb` - Jupyter notebook with complete analysis and model development
- `main.html` - HTML export of the notebook
- `data/framingham_train.csv` - Training dataset
- `data/framingham_test.csv` - Test dataset

## Requirements

Key dependencies:
- pandas
- numpy
- scikit-learn
- statsmodels
- matplotlib
- seaborn
