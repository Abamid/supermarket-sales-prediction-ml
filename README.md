# 🛒 Supermarket Sales Prediction Using Machine Learning

## 📌 Project Overview
This project focuses on building a machine learning model to predict **total sales per transaction** in a supermarket. Accurate sales prediction supports better inventory management, staff scheduling, revenue forecasting, and strategic business planning.

---

## 🏢 Business Problem
Supermarkets handle thousands of transactions daily across multiple product categories and branches. Without reliable sales forecasts, businesses risk:
- Stock shortages or overstocking
- Inefficient staff allocation
- Poor revenue planning
- Suboptimal business decisions

### 🎯 Objective
Build and evaluate machine learning models that accurately predict **total sales per transaction**, and extract insights that support data-driven decision-making.

---

## 📊 Dataset Description
- **Source:** Kaggle – Supermarket Sales Dataset  
- **Link:** https://www.kaggle.com/datasets/faresashraf1001/supermarket-sales  
- **Records:** 1,000 transactions  
- **Target Variable:** `Sales` (continuous numeric)

### Key Features
- Product line
- Unit price
- Quantity
- Customer type
- Payment method
- Branch & city
- Tax, cost, and income-related variables

---

## 🔍 Exploratory Data Analysis (EDA)

### Key Observations
- No missing values detected
- Sales values are right-skewed
- Strong positive relationship between **quantity and sales**
- Balanced sales distribution across product lines

These insights informed feature selection and model choice.

---

## ⚙️ Data Preprocessing & Feature Engineering
- Dropped non-predictive identifiers (Invoice ID, Date, Time)
- One-hot encoded categorical variables
- Scaled numerical features to improve model performance
- Prevented data leakage by excluding cost-derived variables when necessary

---

## 🤖 Model Development
The following regression models were trained and evaluated:
- Linear Regression
- Random Forest Regressor
- Gradient Boosting Regressor

---

## 📈 Model Evaluation

| Model               | MAE | RMSE | R² Score |
|--------------------|-----|------|----------|
| Linear Regression  | ~0  | ~0   | 1.0000   |
| Random Forest      | 0.74| 1.31 | 0.99997  |
| Gradient Boosting  | 1.62| 2.18 | 0.99993  |

---

## 🏆 Best Model Selection
**Selected Model:** Random Forest Regressor

### Justification
Although Linear Regression achieved perfect scores, this was due to **data leakage from cost-derived variables**. Random Forest provides:
- Strong predictive performance
- Robust handling of non-linear relationships
- Better real-world reliability

---

## 🔑 Feature Importance & Business Insights

### Most Influential Features
- Gross income
- Tax (5%)
- Cost of goods sold (COGS)
- Unit price

### Business Insights
- Sales are primarily driven by pricing and cost-related variables
- Product categories contribute relatively evenly to revenue
- Quantity purchased strongly impacts total sales

---

## 💡 Actionable Recommendations
- Optimize pricing strategies to increase transaction value
- Use sales forecasts to align inventory and staffing levels
- Focus promotions on high-margin products
- Monitor tax and cost structures to maximize profitability

---

## 🛠️ Tools & Technologies
- Python
- Pandas, NumPy
- Scikit-learn
- Matplotlib, Seaborn
- Google Colab

---

## 🚀 Future Improvements
- Remove all cost-derived features for production use
- Incorporate time-series patterns
- Deploy model using an API or dashboard

---

## 📬 Author
**Abubakar Amidu**  
DeepTech & Machine Learning Projects
