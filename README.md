# **Customer Behavior Data Analysis Project**

## **Overview**
This project demonstrates an **end-to-end data analytics workflow** using **Python, MySQL, and Power BI**. The main goal of the project is to analyze customer purchase data, clean and prepare the dataset, perform SQL analysis, and create an interactive dashboard to visualize key insights.

The project highlights important data analytics skills such as **data cleaning, database querying, and data visualization**.

---

## **Dataset**
The dataset used in this project contains information related to **customer shopping behavior and product purchases**.

**Main Data Fields**
- Customer information
- Product categories
- Purchase details
- Discount applied
- Sales data

The dataset is first processed and cleaned using **Python**, and then stored in a **MySQL database** for analysis.

---

## **Tools & Technologies**
The following tools and technologies were used in this project:

- **Python**
- **Pandas**
- **NumPy**
- **MySQL**
- **Power BI**
- **Jupyter Notebook**

These tools were used for **data processing, analysis, and visualization**.

---

## **Project Steps**

### **1. Data Loading**
The dataset was imported into Python using **Pandas** to explore and understand the data structure.

### **2. Data Cleaning**
Data cleaning was performed to ensure the dataset is accurate and ready for analysis.

Tasks included:
- Handling missing values
- Removing duplicate records
- Correcting inconsistent values
- Formatting data types

### **3. SQL Analysis (MySQL)**

The cleaned dataset was imported into **MySQL** for analysis.

SQL queries were written to answer important business questions such as:

- Which products are purchased the most?
- What are the customer purchasing patterns?
- How frequently are discounts used?
- What are the sales trends?

Example SQL Query:

```sql
SELECT item_purchased,
ROUND(100 * SUM(CASE WHEN discount_applied = 'Yes' THEN 1 ELSE 0 END)/COUNT(*),2) AS discount_rate
FROM customer
GROUP BY item_purchased
ORDER BY discount_rate DESC
LIMIT 5;
```

### **4. Power BI Dashboard**
An **interactive Power BI dashboard** was created to visualize insights from the dataset.

Dashboard Highlights:
- Sales overview
- Product performance
- Customer purchase trends
- Discount analysis

## **Dashboard Preview**

```
![Dashboard Screenshot](dashboard.png)
```
---

## **Results**
The analysis revealed several important insights:

- Identification of **top-performing products**
- Understanding of **customer purchase patterns**
- Analysis of **discount usage trends**
- Insights into **sales performance**

These insights demonstrate how data analytics helps businesses make **data-driven decisions**.

---

## **Skills Demonstrated**

This project demonstrates the following **data analytics skills**:

- Data Cleaning
- Exploratory Data Analysis
- SQL Query Writing
- Data Visualization
- Dashboard Development
- Business Insight Generation

---

## **Conclusion**
This project demonstrates a complete **data analytics workflow**, from raw data processing to insight generation and visualization. It showcases practical skills in **Python, MySQL, and Power BI**, which are essential tools for data analysts.
