# Food Delivery Time Prediction

## Project Overview
This project predicts whether a food delivery will be **Fast (0)** or **Delayed (1)** using machine learning classification models. The prediction is based on operational and environmental factors such as distance, weather conditions, traffic conditions, vehicle type, and delivery personnel experience.

The target variable was created using the median delivery time to ensure balanced class distribution.

---

## Technologies Used
- Python  
- Pandas  
- NumPy  
- Scikit-learn  
- Matplotlib  
- Seaborn  

---

## Methodology

### Data Preprocessing
- Extracted latitude and longitude from location fields  
- Calculated geographic distance using the Haversine formula  
- Encoded categorical variables using LabelEncoder  
- Standardized numerical features  
- Created binary delivery status (Fast / Delayed)  

### Models Implemented
- Gaussian Naive Bayes  
- K-Nearest Neighbors (with hyperparameter tuning)  
- Decision Tree (with pruning using max_depth and min_samples_split)  

### Evaluation Metrics
- Accuracy  
- Precision  
- Recall  
- F1-score  
- Confusion Matrix  
- ROC Curve  

---

## Key Insights
- Distance and traffic conditions significantly impact delivery delays.  
- Weather conditions influence delivery performance.  
- Delivery personnel experience improves delivery efficiency.  
- Tree-based models effectively capture nonlinear relationships.  

---

## Conclusion
The analysis demonstrates that delivery delays can be predicted using machine learning techniques. The best-performing model can support operational decision-making, route optimization, and service performance improvement.

---

## Files Included
- `Food_Delivery_Time_Prediction.ipynb` – Complete analysis and modeling  
- `Food_Delivery_Time_Prediction.csv` – Dataset  
