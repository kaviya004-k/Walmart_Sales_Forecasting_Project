# Walmart Sales Forecasting Project

---

### **Overview**

**Problem Statement:**\
Walmart, the world's largest company by revenue, generates vast consumer data. This project aimed to analyze historical sales data from 45 Walmart stores to predict weekly sales, uncover patterns, and assess the impact of factors such as holidays, temperature, unemployment, and fuel prices.

**Objective:**\
Develop a statistical model to:

- Predict weekly sales.
- Identify top- and worst-performing stores.
- Analyze the impact of external factors (e.g., unemployment, CPI) on sales.
- Provide actionable insights to optimize operations and profitability.

---

### **Approach**

**1. Data Preprocessing:**

- Dataset: 6435 rows and 8 features (Store, Date, Weekly Sales, Holiday Flag, Temperature, Fuel Price, CPI, Unemployment).
- **Cleaning:** No missing or duplicate values.
- **Transformation:** Converted dates into usable formats for time-series analysis. Detected and handled outliers in `Weekly_Sales`, `Temperature`, and `Unemployment`.

**2. Exploratory Data Analysis:**

- **Sales Trends:** December observed the highest sales due to holidays like Christmas.
- **Store Insights:** Store 20 had the highest sales, while Store 33 performed the worst.
- **Correlation Analysis:**
  - Higher unemployment correlated with lower sales (negative correlation).
  - CPI and temperature showed weak or no significant impact on weekly sales.

**3. Predictive Modeling:**

- Implemented **Facebook Prophet** to forecast weekly sales for the next 12 weeks. Prophet was selected for its ability to model seasonal patterns effectively.

---

### **Key Insights**

**1. Top-Performing Stores:**

- Store 20 leads with maximum sales.

**2. Seasonal Trends:**

- Sales peak in December (holiday season) and slightly increase mid-year (summer/back-to-school shopping).
- Sales dip around August and September due to lack of major holidays.

**3. External Factors:**

- Unemployment significantly impacts sales negatively in some regions.
- CPI and temperature had minimal influence.

**4. Performance Gaps:**

- The difference between the best (Store 20) and worst (Store 33) performing stores was \$275,428,478.

---

### **Predictive Modeling Results**

**Forecast for Next 12 Weeks:**
Using the Prophet model, the weekly sales for Store 1 showed strong seasonal trends and aligned with historical data, providing reliable forecasts for resource planning.

---

### **Conclusion**

This project provided actionable insights into Walmart’s sales patterns, allowing better resource allocation, promotional planning, and strategic decision-making. The predictive model ensures accurate forecasting, enabling Walmart to stay ahead in a competitive market.

**Key Takeaways:**

- Tailored promotional offers during peak seasons can boost sales further.
- Focus on improving the performance of underperforming stores with targeted strategies.
- Maintain a watch on unemployment trends to mitigate sales impact in affected regions.

