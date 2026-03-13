# Global Pollution Analysis and Energy Recovery using Apriori Association Rule Mining

## Overview

This project analyzes global environmental pollution data to identify hidden relationships between pollution indicators and energy recovery patterns. The study applies the Apriori association rule mining algorithm to discover meaningful patterns between air pollution, water pollution, carbon emissions, and energy recovery levels.

The objective of the analysis is to understand how environmental pollution factors are associated with energy recovery activities. The results help reveal patterns that may support environmental policy planning and sustainable energy strategies.

---

## Dataset Description

The dataset used in this project is **Global Pollution Analysis**, which contains environmental and energy-related indicators for different countries and years.

Key attributes in the dataset include:

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

These variables provide insights into pollution levels, environmental impact, and energy recovery practices across regions.

---

## Project Workflow

The project follows a structured data mining workflow consisting of the following stages:

1. Data loading and preprocessing  
2. Exploratory data analysis  
3. Feature engineering and categorization  
4. Transaction creation for association rule mining  
5. Frequent itemset generation using the Apriori algorithm  
6. Association rule generation and evaluation  
7. Interpretation of discovered patterns  

---

## Data Preprocessing

Several preprocessing steps were applied to prepare the dataset for analysis:

- Cleaning column names by removing spaces and special characters
- Handling missing values using mean imputation
- Encoding categorical variables such as country and year
- Standardizing pollution indicators using StandardScaler
- Converting numerical environmental indicators into categorical levels for rule mining

The pollution indicators were categorized into levels such as:

- Low  
- Medium  
- High  

This categorization allowed the dataset to be transformed into transactional data suitable for the Apriori algorithm.

---

## Exploratory Data Analysis

Exploratory data analysis was performed to understand relationships between environmental variables.

The following visualizations were used:

- Scatter plot showing the relationship between **air pollution index and energy recovery**
- Line plot illustrating **air pollution trends over time**
- Correlation heatmap displaying relationships between numerical environmental indicators

These visualizations help identify patterns and dependencies between pollution indicators and energy recovery variables.

---

## Feature Engineering

To apply association rule mining, continuous variables were transformed into categorical levels.

The following features were created:

- **Air_Level** based on Air Pollution Index  
- **Water_Level** based on Water Pollution Index  
- **Energy_Level** based on Energy Recovered  
- **CO2_Level** based on CO2 Emissions  

Each feature represents pollution intensity or energy recovery level categorized into low, medium, and high groups.

---

## Apriori Association Rule Mining

The Apriori algorithm was used to discover frequent patterns within the dataset.

The process involved:

1. Converting categorized variables into transaction format
2. Applying **TransactionEncoder** to transform transactions into a binary matrix
3. Generating frequent itemsets using the **Apriori algorithm**
4. Extracting association rules using support, confidence, and lift metrics

Minimum thresholds were applied to filter meaningful rules.

---

## Evaluation Metrics

The association rules were evaluated using three key metrics.

### Support

Support measures how frequently a rule appears in the dataset. A higher support value indicates that the rule occurs more frequently across the transactions.

### Confidence

Confidence measures the reliability of the rule. It indicates the probability that the consequent occurs when the antecedent is present.

### Lift

Lift measures the strength of the relationship between the antecedent and the consequent. A lift value greater than 1 indicates a strong positive association between the variables.

---

## Visualization of Association Rules

Several visualizations were used to evaluate the quality of the generated rules:

- Distribution plots of **support**
- Distribution plots of **confidence**
- Distribution plots of **lift**
- Scatter plots showing relationships between support, confidence, and lift

These visualizations help identify strong and meaningful association rules.

---

## Key Findings

The analysis revealed several important patterns in the dataset.

- High air pollution levels frequently appear together with high energy recovery levels.
- Moderate water pollution levels often correspond with moderate energy recovery patterns.
- Carbon emission levels show associations with energy recovery activities.
- Certain pollution indicators tend to co-occur, suggesting underlying environmental patterns.

These findings indicate that environmental pollution conditions may influence energy recovery initiatives and sustainability strategies.

---

## Conclusion

This project demonstrates how association rule mining can be applied to environmental datasets to uncover hidden patterns between pollution indicators and energy recovery practices.

By using the Apriori algorithm and evaluating rules through support, confidence, and lift metrics, meaningful relationships were discovered within the dataset.

The analysis highlights the potential of data mining techniques to support environmental monitoring, sustainable resource management, and energy policy development.

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Mlxtend

---

## Author

This project was developed as part of a data mining and machine learning assignment focusing on association rule mining and environmental data analysis.
