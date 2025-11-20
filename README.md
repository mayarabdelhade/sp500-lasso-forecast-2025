# sp500-lasso-forecast-2025
FinTech project predicting S&amp;P500 returns using macro indicators and Lasso Regression.
# 📈 S&P 500 Return Forecasting (2025) Using Lasso Regression  
*A FinTech & Quantitative Modeling Project by Mayar Abdelhade*

---

![Python](https://img.shields.io/badge/Python-3.10-blue)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange)
![Model](https://img.shields.io/badge/Model-Lasso%20Regression-yellowgreen)
![Status](https://img.shields.io/badge/Project-Completed-brightgreen)

---

## 📑 Table of Contents
1. [Project Overview](#project-overview)
2. [Dataset](#dataset)
3. [Modeling Approach](#modeling-approach)
4. [Exploratory Data Analysis](#exploratory-data-analysis)
5. [Model Diagnostics](#model-diagnostics)
6. [2025 Forecast](#2025-forecast)
7. [Visualizations](#visualizations)
8. [Files in Repository](#files-in-repository)
9. [How to Run](#how-to-run)
10. [Author](#author)

---

## 🧠 Project Overview
This project forecasts the **S&P 500 annual return for 2025** using macroeconomic indicators and **Lasso Regression**, a regularized linear model that handles multicollinearity and feature selection.

The model was trained using 20+ years of macroeconomic + market data including:
- Interest Rate  
- Inflation (CPI)  
- GDP Growth  
- Unemployment Rate  
- EPS Growth  
- CAPE Ratio  
- 10Y Yield  
- VIX Index  
- Tariff Dummy (Trade War Indicator)

---

## 📊 Dataset
The dataset contains yearly S&P500 returns and macro indicators.

📄 **File:** `Data S&P500.csv`  
📌 Years covered: **2005–2024**

---

## 🤖 Modeling Approach
Models trained:
- **OLS Regression**  
- **Ridge Regression**  
- **Lasso Regression (Final Model)**  

Lasso was selected because:
- Best generalization (lowest Test MSE)
- Handles noisy features
- Automatically shrinks insignificant coefficients to zero

---

## 🔍 Exploratory Data Analysis

### ✔️ Correlation Heatmap  
Shows relationships between variables and highlights multicollinearity.

📎 `correlation_Heatmap.png`

---

## 🧪 Model Diagnostics

| Metric | Value |
|-------|--------|
| **Train MSE** | 0.0095 |
| **Test MSE** | 0.0223 |
| **Conclusion** | Slight generalization gap → **Good fit**, not overfitting |

### 📊 Train vs Test MSE Plot
📎 `train_vs_test_mse.png`

---

## 🔮 2025 Forecast

### **Predicted S&P500 Return for 2025:**  
### ⭐ **+21.94%**

### **Implied S&P500 Index Level:**  
If 2024 closes at **5538**:  
➡️ **2025 Forecast = 6743**

📎 `sp500_forecast_2025.png`

---

## 📈 Visualizations

- **Actual vs Predicted Returns (Lasso)**  
  📎 `Actual_vs_predicted Lasso Model.png`

- **Train vs Test MSE Comparison**  
  📎 `train_vs_test_mse.png`

- **S&P500 2024 vs Forecast 2025 Line Graph**  
  📎 `sp500_forecast_2025.png`

---

## 📁 Files in Repository

| File | Description |
|------|-------------|
| `S&P500_Returnipynb.ipynb` | Full notebook with modeling + code |
| `Data S&P500.csv` | Dataset used |
| `correlation_Heatmap.png` | EDA heatmap |
| `train_vs_test_mse.png` | Diagnostics |
| `Actual_vs_predicted Lasso Model.png` | Predicted vs actual |
| `sp500_forecast_2025.png` | 2025 forecast plot |
| `README.md` | This documentation |

---

## ▶️ How to Run

1. Clone the repo:
```bash
git clone https://github.com/mayarabdelhade/sp500-lasso-forecast-2025.git
