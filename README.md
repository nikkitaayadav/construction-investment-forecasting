# Construction Investment Forecasting

This repository contains a complete workflow for forecasting construction investment trends in Japan from 2023 to 2030 using historical investment data (1960–2023). The objective is to help planners, policymakers, and industry stakeholders anticipate sectoral growth, optimize budgets, and align infrastructure development with projected demand.

## Project Overview

- **Domain:** Construction and Infrastructure Investment Analytics
- **Dataset Size:** 378 rows × 28 columns, spanning 1960–2023
- **Sectors Covered:** Architecture, Civil Engineering, Residential, Non-Residential, and Public Sector projects
- **Approach:** Data cleaning → EDA → Model training → Hyperparameter tuning → Ensemble modeling
- **Outcome:** Gradient Boosting selected as the top model, with ensemble methods improving prediction stability
- **Ownership:** End-to-end design, implementation, and documentation completed as a solo project

## Methodology

### 1. Data Preprocessing
- Removed columns with excessive missing data
- Imputed remaining missing values using column means
- Applied Min-Max Scaling and Standard Scaling for feature normalization

### 2. Exploratory Data Analysis (EDA)
- Time-series trends of sectoral investments
- Year-on-year growth rates
- Comparative analysis across public vs. private investments
- Sectoral contribution to total construction expenditure

### 3. Model Development
Implemented and evaluated the following regression algorithms:
- Decision Tree Regressor
- Random Forest Regressor
- Gradient Boosting Regressor
- K-Nearest Neighbors (KNN) Regressor
- Linear Regression

### 4. Model Evaluation
- Metrics: **Mean Squared Error (MSE)**, **Mean Absolute Error (MAE)**, **R² Score**
- Gradient Boosting produced the most reliable performance
- Ensemble techniques (bagging & stacking) further enhanced robustness

### 5. Insights
- Architecture and Civil Engineering investments showed stable growth trends
- Public sector projects experienced more volatility compared to private investments
- Predictive modeling indicated steady growth across most sectors for the 2023–2030 horizon

## Files Included

- `notebook.ipynb`: Complete workflow from preprocessing to model evaluation
- `dataset.csv`: Historical investment dataset
- `report.pdf`: Detailed technical report with methodology, analysis, and conclusions
- `presentation.pptx`: Final presentation summarizing findings and recommendations

## Tech Stack

- **Programming:** Python (Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn)
- **Modeling:** Decision Tree, Random Forest, Gradient Boosting, KNN, Linear Regression
- **Tools:** Jupyter Notebook
- **Techniques:** EDA, Feature Scaling, Hyperparameter Tuning, Ensemble Learning

## Acknowledgments

- Dataset: [Construction Investment Amount in Japan – Kaggle](https://www.kaggle.com/datasets/yutodennou/construction-investment-amount-in-japan)

---

