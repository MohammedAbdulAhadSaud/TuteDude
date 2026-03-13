# Deforestation Issue Analysis Using Support Vector Machine (SVM)

## Overview

This project analyzes global deforestation patterns using machine learning techniques. The objective is to explore how environmental, economic, and policy-related factors influence deforestation levels and to build a predictive model using Support Vector Machine (SVM).

The dataset contains multiple indicators such as population, GDP, rainfall, CO₂ emissions, agricultural land percentage, corruption index, and environmental policy measures. These variables are used to predict the percentage of tree cover loss.

---

## Dataset

The dataset includes the following key attributes:

- Country
- Year
- Forest Loss Area (km²)
- Tree Cover Loss (%)
- CO₂ Emissions
- Rainfall
- Population
- GDP (Billion USD)
- Agriculture Land Percent
- Deforestation Policy Strictness
- Corruption Index
- International Aid
- Illegal Lumbering Incidents
- Protected Areas Percent

These variables provide environmental, economic, and governance indicators related to deforestation.

---

## Methodology

The analysis follows several steps:

### 1. Data Preprocessing

- Handling missing values using mean imputation
- Encoding categorical variables
- Removing non-numeric features not required for modeling
- Scaling features using StandardScaler

### 2. Model Development

A Support Vector Regression (SVR) model was used to predict tree cover loss percentage. The model was trained using a training dataset and evaluated on a testing dataset.

### 3. Hyperparameter Tuning

GridSearchCV was applied to optimize the SVM model parameters including:

- Kernel type
- Regularization parameter (C)
- Gamma
- Epsilon

This process improves the model's predictive performance.

---

## Model Evaluation

The model performance was evaluated using the following metrics:

- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)
- R² Score

These metrics measure how closely the predicted deforestation values match the actual values.

---

## Visualization

Several visualizations were generated to better understand the data and validate the model:

- Feature correlation heatmap
- Population vs deforestation scatter plot
- GDP vs deforestation scatter plot
- Actual vs predicted deforestation comparison plot

These visualizations help analyze relationships between variables and assess model prediction quality.

---

## Key Insights

- Most variables show relatively weak correlations with deforestation levels.
- Population and GDP do not demonstrate strong direct relationships with tree cover loss.
- Environmental policies and land use variables may have a stronger influence on deforestation patterns.
- The SVM model can generate predictions but is limited by the complexity and variability of environmental data.

---

## Conclusion

This project demonstrates how machine learning techniques such as Support Vector Machines can be applied to analyze environmental datasets. Although the predictive accuracy is limited due to weak feature relationships, the analysis provides insights into potential factors associated with deforestation.

Further improvements could include incorporating additional environmental variables, satellite data, and larger datasets to improve predictive performance.

---

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn
- Jupyter Notebook
