# 📊 US Macroeconomic & Index-Based Trend Forecasting

This repository contains a pipeline for financial trend prediction using US macroeconomic indicators and major market indices. The project includes data extraction, feature engineering, and model building using both oversampling and undersampling techniques to tackle class imbalance.

## 🧠 Project Overview

**Goal**: Predict market trend direction using historical macroeconomic data and financial indices through a robust data science pipeline.

The project consists of:
1. **Data Extraction** – Collect and clean macroeconomic and index data.
2. **Feature Engineering** – Generate weekly aggregated features.
3. **Model Building** – Build classification models to predict market direction using various sampling strategies.

---
## 📂 Data Sources

- Macroeconomic data from public databases (e.g., FRED)
- Market index data (S&P 500, Nasdaq, etc.)
- Aggregated weekly to create a consistent time series format

---

## ⚙️ Notebooks Overview

### 1. `1. Data Extractor - US Macro and Indices.ipynb`
- Extracts macroeconomic and index data
- Cleans and formats into a time-series structure

### 2. `2_Feature_Creation.ipynb`
- Resamples data weekly
- Generates relevant trend and lag features
- Outputs: `final_df.csv`

### 3. `3_Model_Building.ipynb`
- Builds base machine learning models
- Evaluates without addressing class imbalance

### 4. `3_Model_Building_Oversampled.ipynb`
- Applies **oversampling (SMOTE)** to balance classes
- Trains models and compares performance

### 5. `3_Model_Building_Undersampled.ipynb`
- Applies **undersampling** for class balance
- Evaluates model impact with reduced data

---

## 📈 Models & Techniques

- **Logistic Regression**
- **Random Forest**
- **XGBoost**

With performance evaluated using:
- Precision, Recall, F1-score
- Confusion Matrix
- ROC-AUC (if applicable)

---

## 🧪 Sampling Strategies

To deal with class imbalance in trend labels:
- **Oversampling** (SMOTE)
- **Undersampling** (Random undersampling)

---
