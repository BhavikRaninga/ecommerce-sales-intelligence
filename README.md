[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)]https://colab.research.google.com/drive/1KKJrJvbV27ceDo0M2rIM_cqtvhFGrdwL#scrollTo=YMPfq4BlYFTc
https://colab.research.google.com/github/BhavikRaninga/ecommerce-sales-intelligence/blob/main/notebooks/ecommerce_sales_analysis.ipynb
# 📊 E-Commerce Profitability & Sales Intelligence System

## 🚀 Project Overview

This project presents an end-to-end **data science solution** for analyzing and optimizing e-commerce business performance. It combines **data cleaning, business analytics, machine learning, and visualization** to uncover revenue drivers, operational inefficiencies, and growth opportunities.

---

## 🎯 Objectives

* Analyze multi-channel e-commerce sales data
* Identify key revenue drivers and loss factors
* Segment products based on performance
* Build a machine learning model to predict revenue

---

## 📂 Dataset

* Source: Kaggle (E-Commerce Sales Dataset)
* Contains:

  * Transaction-level sales data
  * Product details (SKU, category, size)
  * Order status (shipped, returned, cancelled)
  * Channel and fulfillment information

---

## 🧹 Data Cleaning & Preprocessing

* Removed irrelevant columns (`index`, unnamed fields)
* Standardized column names
* Converted `Date` to datetime format
* Filtered valid transactions (Shipped/Delivered only)
* Removed invalid entries (`Qty > 0`, `Amount > 0`)
* Created **Revenue** feature

---

## 📊 Exploratory Data Analysis (EDA)

### Key Insights:

* **Revenue Concentration:**
  The *Set* category dominates overall revenue, contributing as much as the next four categories combined.

* **Revenue Leakage (~5%):**
  Returns, cancellations, and lost shipments significantly impact profitability.

* **Sales Trend:**
  Monthly analysis shows variation in revenue, with potential seasonality or incomplete data in certain months.

* **B2C Dominance:**
  Majority of revenue comes from direct customers, indicating stronger margins compared to B2B.

---

## 🤖 Machine Learning

### 1. Product Segmentation (K-Means Clustering)

* Features used: `Revenue`, `Quantity`
* Identified 3 clusters:

  * **High Performers:** Key revenue-driving SKUs
  * **Mid Performers:** Growth opportunity products
  * **Low Performers:** Underperforming SKUs

📌 Insight:

> A small subset of SKUs contributes disproportionately high revenue, highlighting strong product-level concentration.

---

### 2. Sales Prediction Model (Regression)

#### Models Used:

* Linear Regression
* Random Forest Regressor

#### Features:

* Quantity
* Category
* B2B
* Time-based features (Month, Day)
* Fulfillment & location (enhanced model)

#### Performance:

* **R² Score ≈ 0.41**

📌 Interpretation:

> The model demonstrates moderate predictive power, capturing key revenue drivers. However, performance is limited due to missing features such as pricing variations, discounts, and customer behavior.

---

## 🧠 Key Learnings

* Real-world datasets are messy and require **business-driven cleaning decisions**
* **Feature quality matters more than model complexity**
* Combining **analytics + ML + insights** creates maximum impact
* Data science is as much about **interpretation** as it is about modeling

---

## 🛠️ Tech Stack

* Python
* pandas, numpy
* matplotlib, seaborn
* scikit-learn
* Jupyter Notebook

---

## 📈 Future Improvements

* Incorporate pricing and discount features
* Add customer-level segmentation
* Deploy as an interactive dashboard (Streamlit)
* Integrate real-time prediction API

---

## 📌 Conclusion

This project demonstrates a complete workflow from **raw data to actionable insights and predictive modeling**. It highlights how data can be leveraged to improve decision-making in e-commerce businesses.

---
## 💡 Business Impact

- Identified revenue concentration risk in top category  
- Detected ~5% revenue loss due to returns and cancellations  
- Segmented products to optimize inventory and marketing strategy  
- Built predictive model to support sales forecasting  

👉 This project demonstrates how data-driven insights can improve profitability and decision-making in e-commerce businesses.

## 🔗 Author

**Bhavik Raninga**
Aspiring Data Scientist | Applied AI Enthusiast
