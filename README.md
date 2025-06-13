
# 🛒 Walmart Sales Forecasting

Forecast weekly sales at Walmart stores using machine learning.

---

## 🎯 Project Objective

This project aims to build a machine learning model to forecast **weekly sales** at Walmart stores using historical data. The goal is to support better planning, inventory management, and strategic decision-making.

---

## 📊 Dataset Overview

- **Source**: Kaggle (Walmart Sales Forecasting)
- **Target Variable**: `Weekly_Sales`
- **Features Used**:
  - `Store`, `Date`, `Holiday_Flag`, `Temperature`, `Fuel_Price`, `CPI`, `Unemployment`
  - `Year`, `Month`, `Week`, `Day`, `DayOfWeek`, `Is_Weekend`, `PreHoliday_Week`
  - `Temp_Range_Cold`, `Temp_Range_Mild`, `Temp_Range_Hot`
  - `Fuel_Level_Medium`, `Fuel_Level_High`
  - `Holiday_Label_Non-Holiday`

---

## 🤖 Modeling Approach

- **Models Used**:
  - Linear Regression
  - Decision Tree
  - Random Forest
  - XGBoost Regressor

---

## 🛠️ Tools & Libraries

- **Programming Language**: Python
- **Libraries**:
  - `pandas`, `numpy`
  - `matplotlib`, `seaborn` for EDA
  - `scikit-learn` for modeling and evaluation
  - `xgboost` for gradient boosting
  - `joblib` for model serialization

---

## 🧱 Feature Engineering

- Extracted `Year`, `Month`, `Week` from `Date`
- Converted `IsHoliday` to binary
- Labeled `Temperature` and `Fuel Price` into categories
- Removed irrelevant or redundant columns

---

## 🔍 Exploratory Data Analysis (EDA)

- Analyzed trends across time, stores, and holidays
- One-hot encoded categorical variables
- Visualized distributions and outliers
- Created:
  - Correlation heatmaps
  - Boxplots of `Weekly_Sales`
  - Sales comparison: Holiday vs Non-Holiday
  - Analysis of `Temp_Range` and `Fuel_Level`

---

## 💡 Key Insights

- Holidays lead to significantly higher weekly sales.
- Temperature and fuel price influence consumer behavior.
- Outliers are common due to holiday spikes and store-level promotions.

---

## 🧪 Model Building

- **Algorithms**: Linear Regression, Decision Tree, Random Forest, XGBoost
- **Train-Test Split**: 80:20
- **Hyperparameter Tuning**:
  - Grid Search CV
  - Randomized Search CV
- **Evaluation Metrics**:
  - RMSE (Root Mean Squared Error)
  - MAE (Mean Absolute Error)
  - R² Score

### ✅ Best Model: XGBoost Regressor

- **RMSE**: `76,214.40`
- **R² Score**: `0.981`

---

## 📁 Project Structure

```
walmart_sales_forecasting/
├── Walmart_Sales.csv
├── Walmart_Sales.ipynb
├── requirements.txt
├── xgboost_walmart_model.ipynb
├── xgboost_walmart_model.pkl
├── Training_data.csv 
└── README.md
```

---

## 💼 Business Impact

- Enables Walmart to forecast upcoming weekly sales
- Aids stock and workforce management
- Highlights key seasonal and holiday trends for decision-making

---

## ✅ Conclusion

- **XGBoost** performed best among tested models
- Effective **feature engineering** and **tuning** boosted performance
- Model explains **98.1%** of the variance in weekly sales

---

## 🔭 Future Work

- Integrate real-time or recent data
- Build an interactive dashboard for live predictions

---

## 👨‍💻 Author

**Mihir Patil**  
Data Science Capstone Project | MIT World Peace University
