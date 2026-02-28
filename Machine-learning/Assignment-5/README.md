# Food Delivery Time Prediction  
## Neural Networks and Clustering Assignment

---

## Assignment Objective

This assignment applies both **unsupervised learning** and **supervised learning** techniques to analyze and predict food delivery delays.

The main objectives were:

- Perform clustering analysis to identify delivery patterns
- Build and tune a Neural Network classifier
- Compare Neural Network performance with Logistic Regression
- Evaluate models using multiple performance metrics
- Interpret results and justify the best-performing model

---

## Problem Statement

The goal of this project is to classify food deliveries as:

- Fast (0)
- Delayed (1)

The target variable `Delivery_Status` was created using the median delivery time as the classification threshold.

---

## Dataset Overview

The dataset includes operational and environmental features such as:

- Customer and restaurant locations
- Traffic conditions
- Weather conditions
- Delivery personnel experience
- Order priority
- Delivery time

---

## Feature Engineering

The following preprocessing steps were performed:

- Extracted latitude and longitude from location columns
- Computed Haversine distance between customer and restaurant
- Created a Rush Hour indicator feature
- Encoded categorical variables using LabelEncoder
- Standardized numerical features using StandardScaler

---

# Part 1: Clustering Analysis

## K-Means Clustering

- The Elbow Method was used to determine the optimal number of clusters.
- Three clusters were selected based on inertia reduction.
- Cluster analysis showed that traffic conditions strongly influence delivery delays.

## Hierarchical Clustering

- Agglomerative clustering was implemented.
- A dendrogram was generated to visualize hierarchical grouping.
- Results supported similar segmentation patterns observed in K-Means.

### Clustering Insight

Traffic congestion was found to be a stronger driver of delivery delays than delivery distance alone.

---

# Part 2: Supervised Learning

## Neural Network (MLPClassifier)

A feedforward neural network was implemented and tuned using GridSearchCV.

### Best Hyperparameters

- Hidden layers: (32, 16)
- Activation function: ReLU
- Regularization (alpha): 0.0001
- Early stopping enabled
- Maximum iterations: 2000

### Evaluation Metrics

The model was evaluated using:

- Accuracy
- Precision
- Recall
- F1-score
- ROC-AUC

The Neural Network achieved strong recall but lower AUC.

---

## Logistic Regression

Logistic Regression was implemented as a baseline linear classifier.

It achieved higher overall accuracy compared to the Neural Network.

---

# Model Comparison

| Model | Accuracy |
|--------|----------|
| Neural Network | 55% |
| Logistic Regression | 57.5% |

Although the Neural Network achieved higher recall and F1-score, Logistic Regression achieved higher overall accuracy and demonstrated more stable discrimination performance.

---

# Final Model Selection

Logistic Regression was selected as the better-performing model for this dataset.

The results suggest that the dataset may not contain strong nonlinear patterns, and simpler linear models may generalize more effectively.

---

# Key Takeaways

- Traffic conditions significantly influence delivery delays.
- Clustering helps identify meaningful delivery segments.
- Neural Networks can model complex patterns but may not always outperform simpler models.
- Proper evaluation using multiple metrics is essential for fair model comparison.

---

# Conclusion

This assignment demonstrates the integration of clustering and classification techniques for operational data analysis.

While Neural Networks offer nonlinear modeling capabilities, Logistic Regression provided better generalization performance for this dataset and is recommended as the final predictive model.
