# Global Pollution Severity Classification

## Project Overview
This project classifies countries into **Low, Medium, and High pollution severity levels** using environmental and socio-economic indicators from the Global Pollution dataset.

The objective is to apply multi-class classification techniques to analyze pollution patterns and evaluate model performance using standard machine learning metrics.

---

## Dataset
The dataset includes environmental indicators such as:

- Air Pollution Index  
- Water Pollution Index  
- Soil Pollution Index  
- CO₂ Emissions  
- Industrial Waste  
- Renewable Energy Usage  
- Energy Consumption Per Capita  
- GDP Per Capita  
- Population  

A combined **Total Pollution index** was created to categorize countries into three balanced severity groups.

---

## Methodology

### Data Preprocessing
- Handled missing values using median imputation  
- Engineered Total Pollution index  
- Created multi-class target variable (Low, Medium, High)  
- Encoded categorical features (Country, Year)  
- Applied feature scaling (StandardScaler and MinMaxScaler for Naive Bayes)  
- Performed train-test split to avoid data leakage  

### Models Implemented
- Multinomial Naive Bayes  
- K-Nearest Neighbors (with hyperparameter tuning)  
- Decision Tree (with pruning)

---

## Evaluation Metrics
Models were evaluated using:

- Accuracy  
- Precision  
- Recall  
- F1-score  
- Confusion Matrix  

---

## Results
KNN and Decision Tree outperformed Naive Bayes, indicating that nonlinear models better capture relationships among pollution indicators.

---

## Conclusion
Machine learning classification models can effectively categorize countries by pollution severity. The best-performing model provides a structured approach for environmental risk assessment and policy planning.

---

## Files Included
- `Global_Pollution_Classification.ipynb` – Complete analysis and modeling  
- `Global_Pollution_Analysis.csv` – Dataset  
