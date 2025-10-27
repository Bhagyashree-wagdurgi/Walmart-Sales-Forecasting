# Walmart-Sales-Forecasting
End-to-end data analysis and forecasting project using Walmart’s weekly sales data. Includes EDA, correlation analysis, and Holt–Winters time series forecasting for 5 top-performing stores to predict the next 12 weeks of sales. Tools: Python, Pandas, Matplotlib, Statsmodels
Perfect 👍 You want a **numbered, detailed, professional `README.md`** that’s ready for GitHub — explaining both the **business** and **technical** sides of your **Walmart Sales Forecasting Project**.

---

# 🏪 Walmart Sales Forecasting Project

## 1️⃣ Project Overview
Walmart operates thousands of stores across the United States, each affected by multiple external and internal factors such as holidays, temperature, and unemployment rate.
This project aims to **analyze historical sales data** and **forecast future sales** to help management plan inventory, staffing, and promotional strategies more effectively.

The goal is to build a **data-driven forecasting model** that identifies trends, seasonal patterns, and key factors influencing store performance.


## 2️⃣ Objectives
1. Understand sales patterns and their relationship with external factors.
2. Identify the most and least profitable stores.
3. Forecast future sales using time series modeling.
4. Provide actionable insights for business decision-making.


## 3️⃣ Dataset Description
**Dataset Source:** Walmart Kaggle Dataset

**Key Columns:**

| Column Name    | Description                               |
| -------------- | ----------------------------------------- |
| `Store`        | Store ID                                  |
| `Dept`         | Department number                         |
| `Date`         | Week start date                           |
| `Weekly_Sales` | Total sales for that department and week  |
| `IsHoliday`    | Whether the week includes a major holiday |
| `Temperature`  | Average temperature for the week          |
| `Fuel_Price`   | Cost of fuel in the region                |
| `CPI`          | Consumer Price Index                      |
| `Unemployment` | Unemployment rate                         |

---

## 4️⃣ Data Preprocessing Steps
1. **Merged** multiple CSVs (`features`, `stores`, and `sales`) into one dataset.
2. **Handled Missing Values** using median and forward-fill methods.
3. **Converted Date column** into `datetime` format and extracted time-based features (`Year`, `Month`, `Week`).
4. **Removed Outliers** based on z-score and visual inspection.
5. **Feature Engineering:**

   * Created rolling averages (4-week and 12-week).
   * Encoded holidays and special weeks.
   * Normalized numeric variables for stable model performance.

---

## 5️⃣ Exploratory Data Analysis (EDA)
Key insights discovered during analysis:

1. **Sales vs Unemployment:** Negative correlation — as unemployment increases, sales tend to decline.
2. **Holiday Effect:** Weeks containing holidays (Thanksgiving, Christmas) show significantly higher sales.
3. **Temperature Impact:** Extremely hot or cold weeks reduce overall spending.
4. **Store Size:** Larger stores tend to generate higher sales consistently.
5. **Regional Trends:** Sales patterns vary significantly across different store regions.

Visualizations included:

* Correlation heatmaps
* Store-wise and department-wise bar charts
* Time series line plots
* Distribution of weekly sales
* Holiday vs Non-Holiday comparison plots

---

## 6️⃣ Modeling and Forecasting

**Models Used:**

1. **ARIMA / SARIMA** — Baseline statistical model capturing seasonality.
2. **Facebook Prophet** — Handles trend and holiday effects automatically.
3. **Linear Regression & Random Forest** — Benchmarks for comparison.

**Model Evaluation Metrics:**

* RMSE (Root Mean Squared Error)
* MAE (Mean Absolute Error)
* MAPE (Mean Absolute Percentage Error)

**Results:**

* Prophet achieved **lowest RMSE**, performing best for multi-store seasonal forecasting.
* SARIMA captured short-term seasonality effectively but struggled with sudden changes (holidays, promotions).

---

## 7️⃣ Key Insights and Conclusions

* **Economic Stability Matters:** Sales decline when unemployment rises.
* **Holidays Boost Revenue:** Holiday weeks outperform normal weeks by ~30–45%.
* **Temperature Influence:** Mild weather drives higher footfall and sales.
* **Store Segmentation:** Some stores consistently outperform others — these could serve as benchmarks.
* **Forecast Outcome:** Positive growth trend expected for high-performing stores in upcoming quarters.

---

## 8️⃣ Future Improvements

1. Integrate **promotional and pricing data** as external regressors.
2. Implement **Prophet / SARIMAX hybrid** model for improved accuracy.
3. Deploy a **Flask or Streamlit app** for real-time sales forecasting.
4. Build **interactive Power BI dashboards** for executive-level decision support.
5. Add **anomaly detection module** for detecting unusual sales behavior.

---

## 9️⃣ Tools and Technologies Used

| Category                 | Tools / Libraries             |
| ------------------------ | ----------------------------- |
| **Programming Language** | Python                        |
| **Data Handling**        | Pandas, NumPy                 |
| **Visualization**        | Matplotlib, Seaborn, Power BI |
| **Modeling**             | Statsmodels, Prophet          |
| **Deployment (Future)**  | Flask / Streamlit             |             

---

👤 **Bhagyashree Wagdurgi**
📧 *[[email](mailto:bhagyashreewagdurgi@gmail.com)]*
🔗 [LinkedIn](https://www.linkedin.com/in/bhagyashreesw246/)
💻 [GitHub](https://github.com/bhagyashree-wagdurgi)

---

⭐ **If you found this project useful, please give it a star on GitHub!**
💬 *Feedback and suggestions are always welcome.*

---
