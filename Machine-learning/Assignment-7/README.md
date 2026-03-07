# Food Delivery Time Prediction using CNN

## Project Overview
This project analyzes a food delivery dataset to predict whether an order will be delivered **Fast** or **Delayed** using machine learning and deep learning techniques. The project demonstrates a complete machine learning pipeline including data preprocessing, feature engineering, model training, evaluation, and validation.

The primary goal is to compare a traditional machine learning model (**Logistic Regression**) with a deep learning approach (**Convolutional Neural Network – CNN**) to understand how different models perform on delivery prediction tasks.

---

## Dataset
The dataset used in this project is:

**Food_Delivery_Time_Prediction.csv**

It contains various features related to food delivery such as:

- Customer location
- Restaurant location
- Distance
- Weather conditions
- Traffic conditions
- Delivery person experience
- Vehicle type
- Order priority
- Order time
- Delivery time
- Customer and restaurant ratings

---

## Project Phases

### Phase 1: Data Preprocessing
The dataset is cleaned and prepared for modeling.

Steps performed:
- Loading the dataset
- Handling missing values
- Encoding categorical variables
- Feature scaling
- Creating new engineered features

Key engineered features:
- **Distance_Category**
- **Weather_Traffic_Impact**

---

### Phase 2: CNN Model Development
A **Convolutional Neural Network (CNN)** model is implemented to classify deliveries as **Fast** or **Delayed**.

Model architecture includes:
- Conv1D layers
- MaxPooling layers
- Dense layers
- Sigmoid output layer for binary classification

---

### Phase 3: Model Evaluation and Validation

Multiple evaluation techniques are used to assess model performance:

- Logistic Regression baseline model
- Confusion Matrix
- ROC Curve and AUC
- K-Fold Cross Validation
- Training vs Validation Loss visualization

These methods help evaluate model accuracy, generalization capability, and classification performance.

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- TensorFlow / Keras
- Jupyter Notebook

---

## Results

The models were able to classify delivery outcomes using operational and environmental factors. The CNN model captures nonlinear relationships between features such as distance, traffic conditions, and weather conditions.

Cross-validation was used to ensure the model generalizes well to unseen data.

---

## Key Insights

- Delivery **distance** significantly affects delivery time.
- **Traffic and weather conditions** increase the probability of delayed deliveries.
- **Vehicle type and delivery experience** influence delivery efficiency.

These insights can help delivery platforms improve operational planning and logistics.

---

## Future Improvements

Possible improvements include:

- Using larger datasets
- Adding real-time traffic data
- Applying advanced deep learning models
- Hyperparameter tuning
- Feature importance analysis

---

## Author
Project developed as part of an academic machine learning assignment.
