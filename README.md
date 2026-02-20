# 📈 Retail Demand Forecasting & Business Intelligence  
**Datathon Submission – High-Precision Inventory Prediction**

---

## 🚀 Executive Summary  
This project develops a high-accuracy demand forecasting model to optimize retail inventory planning. Using 8,910 rows of historical sales data, the model predicts daily unit sales based on pricing, promotions, seasonality, and competitive positioning.

The objective was to improve ordering decisions, reduce stockouts, and minimize overstock costs through data-driven forecasting.

---

## 📊 Key Performance Metrics  

| Metric | Value | Business Interpretation |
|--------|--------|------------------------|
| R² Score | 0.9848 | Model explains 98.5% of variance in sales patterns |
| Mean Absolute Error (MAE) | 6.31 units | Average prediction error is ~6 units |
| Accuracy | 97.83% | Reliable forecasting for operational planning |

---

## 💡 Business Problem Solutions  

### 1️⃣ Category Revenue Distribution  
Identified high-performing categories contributing the majority of total revenue.  

**Business Impact:**  
- Prioritized inventory allocation  
- Focused marketing investments  
- Strategic supplier negotiations  

---

### 2️⃣ Seasonal Sales Patterns  
Discovered a 100.3% variation between peak (December) and lowest (February) sales months.  

**Business Impact:**  
- Proactive workforce planning  
- Smarter warehouse allocation  
- Seasonal procurement optimization  

---

### 3️⃣ Review Rating Impact  
Identified a demand inflection point around a 4.0 rating threshold.  
Products above this rating showed significantly stronger sales performance.

**Insight:**  
Improving product quality and customer satisfaction directly drives revenue growth.

---

### 4️⃣ Promotion Effectiveness  
Measured the average uplift from promotional campaigns and identified the most promotion-sensitive categories.

**Business Application:**  
- Targeted promotional spending  
- Improved ROI tracking  
- Data-driven marketing strategy  

---

## 🎯 Feature Engineering Strategy  

To improve predictive performance, advanced feature engineering techniques were applied:

- **Lag Feature (Previous Day Sales):** Captures short-term demand momentum  
- **Competitor Price Gap:** Relative pricing metric vs. market average  
- **Rolling 3-Day Average:** Smooths short-term volatility and captures trend signals  
- **Seasonal Indicators:** Month-based encoding  

---

## 🛠 Modeling Approach  

### Data Preprocessing  
- Chronological sorting  
- Missing value handling (forward fill)  
- Feature scaling (where required)  

### Leakage Prevention  
- Removed revenue-related variables from training features  

### Model Selection  
- Random Forest Regressor (200 estimators)  
- Handles non-linear demand behavior effectively  

### Validation Strategy  
- 80/20 time-series split  
- Tested strictly on unseen future data  

---

## 📂 Project Files  

- `Demand_Forecasting.ipynb` – Complete documented code  
- `submission_predictions.csv` – Final predicted unit sales  
- `submission_metrics.csv` – Model evaluation metrics (R², MAE, RMSE)  
- `Presentation.pdf` – Business insights and strategic recommendations  

---

## 🧰 Tools & Technologies  

- Python  
- Pandas  
- Scikit-learn  
- Matplotlib  
- Seaborn  

---

## 📌 Key Takeaway  

This project demonstrates the ability to combine exploratory data analysis, feature engineering, and machine learning to deliver actionable business insights and high-precision retail demand forecasting.
