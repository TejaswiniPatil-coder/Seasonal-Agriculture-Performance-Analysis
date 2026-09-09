# Seasonal Agriculture Performance Analysis

## 📌 Project Overview

Seasonal Agriculture Performance Analysis is a data analytics and machine learning project developed as part of the VOIS Internship Major Project.

The project analyzes agricultural data to identify patterns and insights related to seasonal performance, crop production, yield, regional performance, profitability, water efficiency, and disease/pest risk.

The complete project was developed and executed using **Google Colab and Python**.

---

## 🎯 Objectives

- Analyze agricultural performance across different seasons
- Compare crop-wise production and yield
- Analyze state-wise agricultural performance
- Evaluate profitability and profit margins
- Analyze water-use efficiency
- Examine disease and pest risk
- Identify relationships between agricultural variables
- Develop a machine learning model for yield prediction
- Generate evidence-based agricultural insights

---

## 📊 Dataset

The dataset contains:

- **4,000 agricultural records**
- **28 original variables**
- Information related to crops, seasons, states, farm area, environmental conditions, production, yield, financial performance, water usage, and disease/pest risk.

After feature engineering, the final dataset contains **31 columns**.

---

## 🔄 Project Workflow

1. Data Loading
2. Data Cleaning
3. Missing Value Handling
4. Duplicate Detection
5. Feature Engineering
6. Exploratory Data Analysis
7. Seasonal Analysis
8. Crop-wise Analysis
9. State-wise Analysis
10. Crop × Season Analysis
11. Environmental Analysis
12. Profitability Analysis
13. Water Efficiency Analysis
14. Disease/Pest Risk Analysis
15. Correlation Analysis
16. Outlier Analysis
17. Predictive Modeling
18. Model Evaluation
19. Evidence-Based Recommendations

---

## 🔧 Feature Engineering

Three additional features were created:

- `Yield_Efficiency`
- `Profit_Margin_pct`
- `Profit_Status`

The final dataset contains **4,000 rows and 31 columns**.

---

## 📈 Key Findings

### Seasonal Performance

- **Kharif** was the highest-producing season with **82,387.61 tonnes**.
- Kharif contributed **47.63%** of total production.
- Rabi contributed **39.02%**.
- Zaid contributed **13.35%**.

### Regional Performance

- **Punjab** was the highest-producing state.
- Total production from Punjab was **25,280.82 tonnes**.

### Profitability

- Total Revenue: **₹2,551,440,192**
- Total Cost: **₹2,105,214,332**
- Total Profit/Loss: **₹446,225,860**
- Profitable Farms: **2,034**
- Loss-Making Farms: **1,966**

### Crop Profitability

- **Chilli** was the most profitable crop.
- Total Chilli profit: **₹309,361,877**
- Average Chilli profit margin: **33.78%**

### Water Efficiency

- **Sugarcane** was the most water-efficient crop.
- Average water efficiency: **30.48 tonnes per 1,000 m³**

---

## 🤖 Machine Learning Model

A **Random Forest Regressor** was developed to predict:

**Target:** `Yield_Tonnes_Ha`

### Model Configuration

- 18 input features
- 80/20 train-test split
- Random Forest Regressor
- 200 trees
- Random state: 42

Downstream variables such as production, revenue, profit, and water efficiency were excluded from the model to reduce target leakage.

### Test Set Performance

| Metric | Result |
|---|---:|
| MAE | 0.7412 tonnes/hectare |
| RMSE | 2.6168 tonnes/hectare |
| R² Score | 0.9645 |

### 5-Fold Cross-Validation

| Metric | Mean |
|---|---:|
| R² | 0.9632 |
| MAE | 0.7581 tonnes/hectare |

The model demonstrated strong predictive performance with consistent cross-validation results.

---

## 🛠️ Technologies Used

- Google Colab
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Random Forest Regressor

---

## 📁 Project Structure

```text
Seasonal-Agriculture-Performance-Analysis/
│
├── Seasonal_Agriculture_Performance_Analysis.ipynb
└── README.md
