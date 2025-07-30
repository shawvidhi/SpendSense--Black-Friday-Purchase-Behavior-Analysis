# 🛍️ SpendSense: Black Friday Purchase Behavior Analysis

Welcome to **SpendSense**, an in-depth exploratory data analysis (EDA) and feature engineering project built on the **Black Friday** dataset provided by a major retail company. This analysis uncovers hidden patterns in customer demographics and product categories to understand **purchase behavior** and support **personalized marketing strategies**.

---

## 📌 Problem Statement

A retail company, **ABC Pvt. Ltd.**, aims to:
- Understand how different **customer segments** purchase products.
- Analyze **demographic and product-based features** that influence spending.
- **Predict the purchase amount** for personalized offers and targeted promotions.

---

## 📊 Dataset Overview

- **Size**: ~550,000 rows
- **Features**:
  - `User_ID`, `Product_ID`
  - Demographics: `Gender`, `Age`, `Occupation`, `City_Category`, `Stay_In_Current_City_Years`, `Marital_Status`
  - Product categories: `Product_Category_1`, `Product_Category_2`, `Product_Category_3`
  - Target: `Purchase`

---

## 🔍 Exploratory Data Analysis (EDA)

Key insights from EDA:

### 👥 Customer Demographics
- **Male customers** form the majority of the buyers.
- Age group **26–35** has the highest purchase frequency.
- **Married individuals** show a slightly higher purchase tendency.
- Most customers belong to **City_Category B** and have lived there for **1 or more years**.

### 🛒 Product Categories
- **Product_Category_1** is mandatory and most active in the range `1–20`.
- **Category 2 & 3** contain many missing values — handled through imputation.

### 💵 Purchase Trends
- **Occupation** shows varying spending patterns — higher spending in occupations 4, 10, and 17.
- Customers staying longer in one city tend to **spend more**.
- Product combos and frequent buyers identified through pivot and heatmaps.

---

## 🧠 Feature Engineering

- **Missing Value Imputation**: Replaced `NaN` in `Product_Category_2/3` with `0` or statistical methods.
- **Label Encoding**: For `Gender`, `City_Category`, `Stay_In_Current_City_Years`, etc.
- **Binning**: Age grouped into numerical buckets for modeling.
- **Interaction Features**: Combined user-product behavior for personalized modeling.

---

## 📈 Next Steps (Modeling Ready)

This dataset is now ready for machine learning modeling (e.g., Linear Regression, XGBoost, LightGBM) to **predict purchase amounts** using engineered features.

---

## 🛠️ Tools & Libraries

- **Python**
- **Pandas, NumPy**
- **Matplotlib, Seaborn, Plotly**
- **scikit-learn** (for preprocessing)

---
