# Assignment 2 - Global Pollution Analysis and Energy Recovery

## Overview

This project analyzes global pollution data and its relationship with energy recovery. The objective is to perform exploratory data analysis, build predictive models, and evaluate their performance using regression and classification techniques.

The project is completed as part of the Machine Learning assessment.

---

## Dataset Description

The dataset contains information related to:

- Country
- Year
- Air Pollution Index
- Water Pollution Index
- Soil Pollution Index
- Industrial Waste (in tons)
- Energy Recovered (in GWh)
- CO2 Emissions (in MT)
- Renewable Energy (%)
- Plastic Waste Produced (in tons)
- Energy Consumption Per Capita (in MWh)
- Population (in millions)
- GDP Per Capita (in USD)

---

## Project Workflow

### 1. Data Preprocessing
- Checked and handled missing values
- Cleaned column names
- Encoded categorical variable (Country)
- Created Pollution Severity target
- Applied feature scaling after train-test split

### 2. Exploratory Data Analysis (EDA)
- Descriptive statistics
- Correlation heatmap
- Trend visualization
- Distribution analysis

### 3. Regression Modeling
Target: Energy_Recovered (in GWh)

Models used:
- Linear Regression
- Random Forest Regressor

Evaluation Metrics:
- Mean Squared Error (MSE)
- Mean Absolute Error (MAE)
- R-squared (R²)

### 4. Classification Modeling
Target: Pollution_Severity

Models used:
- Logistic Regression
- Random Forest Classifier

Evaluation Metrics:
- Accuracy
- Precision
- Recall
- F1 Score
- Confusion Matrix
- ROC Curve

---

## Model Comparison

Regression models were compared using R² and error metrics.

Classification models were compared using Accuracy and ROC-AUC score.

---

## Conclusion

The analysis explores the relationship between pollution indicators and energy recovery. Regression models evaluate how well pollution factors predict energy recovery levels. Classification models identify pollution severity categories.

Model performance indicates the complexity of environmental data and highlights the need for advanced modeling techniques in real-world pollution analysis.

---

## Files Included

- Global_Pollution_Analysis.ipynb
- Global_Pollution_Analysis.csv
- README.md

---

## Submission

This repository contains the complete notebook with preprocessing, modeling, evaluation, visualizations, and conclusions as required by the assessment guidelines.
