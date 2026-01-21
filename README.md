# 📊 Customer Churn & Retention Analysis | Power BI

![Power BI](https://img.shields.io/badge/Tool-Power%20BI-yellow)
![Domain](https://img.shields.io/badge/Domain-Data%20Science%20%26%20Analytics-blue)
![Status](https://img.shields.io/badge/Project-Completed-success)
![Internship](https://img.shields.io/badge/Internship-Future%20Interns-purple)

---

## 🚀 Project Overview

This project was developed as part of my **Data Science & Analytics Internship at Future Interns**.  
The objective of this project is to analyze **customer churn behavior** and identify **key retention drivers** for a subscription-based business using an **interactive Power BI dashboard**.

The dashboard focuses on **customer behavior analysis and business storytelling**, helping stakeholders understand *why customers churn* and *what factors improve retention*, enabling **data-driven retention strategies**.

---

## 🛠️ Tools & Technologies

- **Power BI Desktop** – Dashboard design & visualization  
- **DAX (Data Analysis Expressions)** – KPI and churn calculations  
- **Microsoft Excel** – Dataset handling  
- **Data Modeling** – Relationships & measures  

---

## 🎯 Business Objectives

This dashboard answers key business questions such as:

- What is the overall **customer churn rate**?  
- How many customers are **retained vs churned**?  
- Which **contract types** have the highest churn?  
- How does **customer tenure** impact churn behavior?  
- What is the impact of **pricing (monthly charges)** on churn?  
- How do **support and security services** influence customer retention?  
- Which **payment methods** show higher churn risk?  

---

## 🖼️ Dashboard Pages Overview

### 🔹 Page 1: Customer Churn & Retention Overview

![Churn Overview](Screenshots/page1_overview.png)

**Purpose:**  
Provides management with a high-level snapshot of customer churn and retention performance.

**Key KPIs & Visuals:**
- Total Customers  
- Churned Customers  
- Churn Rate (%)  
- Average Customer Tenure  
- Overall Churn Distribution  
- Churn by Contract Type  
- Churn by Internet Service  
- Churn Rate by Payment Method  

---

### 🔹 Page 2: Customer Churn Patterns & Retention Drivers

![Churn Drivers](Screenshots/page2_patterns_drivers.png)

**Purpose:**  
Designed to uncover **churn patterns and key drivers** influencing customer retention.

**Key Visuals:**
- Churn Across Customer Tenure Groups  
- Impact of Tech Support on Churn (Heatmap)  
- Pricing Impact (Average Monthly Charges vs Churn)  
- Churn Pattern by Online Security Usage  

---

## 📐 Key DAX Measures Used

```DAX
Total Customers = COUNT(customer_churn[customerID])

Churned Customers =
CALCULATE(
    COUNT(customer_churn[customerID]),
    customer_churn[Churn] = "Yes"
)

Churn Rate % =
DIVIDE(
    [Churned Customers],
    [Total Customers],
    0
)

Average Tenure = AVERAGE(customer_churn[tenure])


## 📌 Conclusion

This analysis highlights critical factors influencing customer churn and provides actionable insights that can help businesses improve customer retention strategies.

---

## 👤 Author

**Omkar Udawant**  
Data Science & Analytics Intern  
📍 Pune, India  

---

## 📜 Note

This project was created for learning and internship purposes.
