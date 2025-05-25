
# 📊 Credit Risk Analysis Project

## 🔍 Overview

This project aims to build a data-driven system for **credit risk analysis and prediction**, using loan, debt, credit behavior, and inquiry data. The goal is to help financial institutions assess customer risk and make better lending decisions.

---

## 📁 Dataset

- **Main data file:** `01_dataset (1).csv`
  - Includes **20,000 customers** and **124 features**
  - Target variable: `label` (0 = non-default, 1 = default)

- **Variable description:** `02_data_description.xlsx`
  - Details grouped variables such as:
    - Loan history: `SHORT_TERM_COUNT`, `LONG_TERM_COUNT`, ...
    - Outstanding balances: `OUTSTANDING_BAL_*`
    - Credit inquiries: `ENQUIRIES_*`
    - Late payment history: `CREDIT_CARD_MONTH_SINCE_*`

---

## 🧪 Methodology

### 1. Preprocessing
- Handle missing values and data types
- Normalize and encode variables where needed

### 2. Exploratory Data Analysis (EDA)
- Distribution of target variable
- Correlation and feature importance
- Risk segmentation and visualizations

### 3. Feature Selection
- PCA
- Filter method: Information Gain
- Wrapper method: Recursive Feature Elimination (RFE)

### 4. Model Training
- Models: `Logistic Regression`, `Random Forest`, `XGBoost`

### 5. Visualization
- Feature importance plots
- Risk scoring distribution
- Threshold-based segmentation (Very Poor → Excellent)

---

## ⚙️ Requirements

```bash
Python >= 3.8

# Required libraries
pandas
numpy
matplotlib
seaborn
scikit-learn
xgboost
```

To install:
```bash
pip install -r requirements.txt
```

---

## 📂 Project Structure

```
├── vda-final.ipynb                 # Main notebook
├── 01_dataset (1).csv              # Input dataset
├── 02_data_description.xlsx        # Variable documentation
├── README.md                       # Project documentation (this file)
```

---

## 📈 Key Results

- **XGBoost** performed best in Gini-score.
- Top contributing risk factors:
  - **Recent increases in outstanding balances**
  - **Low credit activity** (few loans or credit cards)**
  - **Stable or increasing debt levels over time**
  - **Lack of financial inquiries (low engagement)**
  - **Dependency on non-bank financial institutions**
  - **Poor credit relationships with banks**
  - **Inability to reduce outstanding balances**
  - **Consistent borrowing without repayment progress**
  - **Inquiry count in recent months**
  - **Number of credit cards (bank vs non-bank)**

---

## 🧑‍💻 Author

Project by: *TEAM 10*  
Course: Visual Data Analytics

---

