# 🌍 Regional Order & Payment Analysis Dashboard

## 📌 Problem Statement

Businesses operating at a global scale often face challenges in understanding **customer behavior, payment preferences, and transaction success rates**.

This project analyzes regional order and payment data to uncover insights that improve **revenue generation, payment efficiency, and customer experience**.

---

## 🎯 Objectives

* Analyze customer distribution and order volume
* Understand payment trends over time
* Evaluate payment methods usage
* Identify inefficiencies in payment processing
* Provide actionable recommendations for business improvement

---

## 📊 Dashboard Overview


<img width="1258" height="496" alt="Dashboard (2)" src="https://github.com/user-attachments/assets/dacd02e1-8a3f-49c9-9f71-7f137092592b" />

<img width="1364" height="545" alt="Data modelling" src="https://github.com/user-attachments/assets/1d95328c-f58a-4d60-aa13-4088c99fffb0" />

-----


## 📈 Key Metrics

| Metric               | Value   |
| -------------------- | ------- |
| Total Customers      | 63M     |
| Total Payment Amount | ~$15.5M |
| Total Orders         | 10K     |

---

# 🔍 Exploratory Data Analysis (EDA)

### 📊 Payment Trends Over Time

* Payment amount and customer count follow similar patterns
* Monthly fluctuations show aligned peaks and dips

👉 **Insight:**
Revenue is highly correlated with customer activity, indicating stable demand patterns.

---

### 🌍 Geographic Distribution

* Customers and payments span across:

  * North America
  * Europe
  * Asia

👉 **Insight:**

* Business operates on a **global scale**
* Revenue streams are diversified across regions

---

### 💳 Payment Method Analysis

| Payment Method | Insight           |
| -------------- | ----------------- |
| Bank Transfer  | Highest usage     |
| Credit Card    | Widely used       |
| PayPal         | Moderate usage    |
| Cryptocurrency | Emerging adoption |
| Cash           | Lowest usage      |

👉 **Insight:**

* Digital payments dominate the ecosystem
* Bank transfers are preferred for high-value transactions
* Cryptocurrency indicates a modern and evolving customer base

---

### 📌 Payment Status Analysis

Payment distribution includes:

* Completed
* Pending
* Failed
* Refunded

👉 **Observations:**

* Completed transactions form the majority
* Noticeable share of **failed and pending payments**

👉 **Insight:**
Indicates inefficiencies in payment processing and potential revenue leakage.

---

# 🔍 Key Insights Summary

* Large customer base (63M) with relatively fewer orders
* Strong correlation between customers and revenue
* Digital payment methods dominate (low cash usage)
* Bank transfer is the most preferred method
* Presence of failed, pending, and refunded transactions indicates operational gaps

---

# 💡 Business Recommendations

### 1. Payment Process Optimization

* Improve payment gateway performance
* Reduce failed and pending transactions
* Implement retry and fallback mechanisms

---

### 2. Customer Experience Enhancement

* Simplify checkout process
* Reduce friction during transactions

---

### 3. Refund Reduction Strategy

* Analyze root causes of refunds
* Improve product/service quality
* Enhance order tracking and transparency

---

### 4. Payment Strategy

* Promote high-success payment methods
* Optimize bank transfer workflows
* Monitor cryptocurrency adoption trends

---

### 5. Regional Strategy

* Identify top-performing countries
* Customize payment options by region
* Localize user experience

---

# ⚠️ Limitations

* No customer segmentation data
* No product-level analysis
* No cost or profit metrics
* Limited insight into causes of payment failures
* No funnel analysis (order → payment → completion)

---

# 🧠 Business Case

### Objective

Enhance payment efficiency and customer experience while reducing revenue leakage.

### Key Questions

* Which payment methods are most effective?
* Where are transaction failures occurring?
* How can payment success rates be improved?
* Which regions contribute most to revenue?

### Stakeholders

* Finance Team
* Product Team
* Operations Team
* Payment Gateway Providers

### Expected Outcomes

* Increased successful transactions
* Reduced payment failures
* Improved customer satisfaction
* Better regional strategy

---

# 🛠 Tools & Technologies

* **Power BI** – Dashboard development
* **DAX** – Data modeling and calculations
* **Excel / CSV** – Data preprocessing

---

# 🧱 Data Modeling

* Star schema approach

**Fact Table:**

* Payments / Orders

**Dimension Tables:**

* Date
* Customer
* Region
* Payment Method

---

# 📊 Key DAX Measures

```DAX id="q8y2pl"
Total Customers = DISTINCTCOUNT(Customers[Customer_ID])

Total Payment Amount = SUM(Payments[Amount])

Total Orders = COUNT(Orders[Order_ID])
```

---

# 📘 Data Dictionary

| Column Name    | Description                          |
| -------------- | ------------------------------------ |
| Customer ID    | Unique customer identifier           |
| Order ID       | Unique order identifier              |
| Payment Amount | Transaction value                    |
| Payment Method | Mode of payment                      |
| Payment Status | Completed, Failed, Pending, Refunded |
| Order Date     | Date of transaction                  |
| Region         | Customer location                    |

---

# 📂 Project Structure

```id="d8x4kp"
regional-order-analysis/
│
├── data/
│   ├── raw_data.csv
│   └── cleaned_data.csv
│
├── dashboard/
│   └── Regional_Order_Dashboard.pbix
│
├── images/
│   └── dashboard.png
│
├── docs/
│   ├── business_case.md
│   ├── data_dictionary.md
│   └── dax_measures.md
│
├── notebooks/
│   └── exploratory_analysis.ipynb
│
├── README.md
└── requirements.txt
```

---

# 🚀 How to Use

1. Download the `.pbix` file from the dashboard folder
2. Open using Power BI Desktop
3. Use filters (date, region, payment method) to explore

---

# 🔮 Future Improvements

* Build payment success prediction models
* Perform customer segmentation (RFM analysis)
* Add funnel analysis (conversion tracking)
* Integrate real-time data pipelines
* Include profitability metrics

---

# 👤 Author

**Salami Emmanuel Hammed**


---
