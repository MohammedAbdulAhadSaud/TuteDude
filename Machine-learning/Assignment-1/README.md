# Assignment 1 – Food Delivery Time Prediction

This project is part of my Machine Learning course Assignment ment in Tutedude.

The goal of this project is to predict food delivery time and analyze the factors that affect delivery performance.

---


## 📌 Project Objective

The objective of this project is to analyze the factors affecting food delivery time and build predictive models to:

1. Predict delivery time using regression models.
2. Classify deliveries as Fast or Delayed using classification models.

The project compares baseline linear models with ensemble methods and provides analytical insights based on model performance.

---

## 📊 Dataset Description

The dataset contains information about:

- Customer and restaurant locations
- Distance between locations
- Weather and traffic conditions
- Delivery personnel experience
- Order cost and tip amount
- Delivery time (target variable)

Both regression and classification modeling techniques were applied.

---

## 🔎 Exploratory Data Analysis (EDA)

- Checked missing values
- Generated descriptive statistics
- Created correlation heatmap
- Used pair plots for feature relationships
- Detected outliers using boxplots

Key finding:
Distance and traffic conditions influence delivery time.

---

## 🛠 Feature Engineering

- Implemented Haversine formula to calculate geographical distance using latitude and longitude.
- Created a `Rush_Hour` feature to capture peak delivery time effects.
- Applied one-hot encoding for categorical variables.
- Standardized numerical features.

---

## 📈 Models Implemented

### 1️⃣ Linear Regression (Baseline)

- Evaluated using MSE, MAE, and R².
- Observed weak performance (negative R²).
- Concluded that linear assumptions may not capture complex delivery patterns.

---

### 2️⃣ Logistic Regression (Baseline Classification)

- Classified deliveries as Fast or Delayed.
- Evaluated using Accuracy, Precision, Recall, F1-score, and ROC-AUC.
- Performance was limited, indicating weak separability of classes.

---

### 3️⃣ Random Forest (Improved Model)

- Applied Random Forest Regressor and Classifier.
- Compared performance against baseline models.
- Demonstrated improved handling of non-linear relationships.

---

## 📊 Model Comparison

- Linear models showed limited predictive power.
- Ensemble method (Random Forest) improved performance.
- Delivery prediction appears to involve complex, non-linear patterns.

---

## 💡 Key Insights

1. Distance plays a major role in delivery time.
2. Rush hour increases delay probability.
3. Simple linear models are insufficient for this dataset.
4. Ensemble methods better capture delivery dynamics.

---

## 📁 Files Included

- `Food_Delivery_Time_Prediction.ipynb` – Complete notebook
- Dataset file
- README.md

---

## 🏁 Conclusion

The project demonstrates that traditional linear models may struggle with real-world delivery prediction tasks. More advanced ensemble models provide better performance and deeper analytical insights.

This assessment focuses on model comparison, performance evaluation, and honest interpretation of results.
