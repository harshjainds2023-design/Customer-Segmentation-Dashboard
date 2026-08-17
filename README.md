# 📊 Customer Segmentation & RFM Analysis

An end-to-end customer analytics project that uses Python, RFM Analysis, and Power BI to understand customer behavior, identify valuable customer segments, and generate actionable business insights.

## 📌 Project Overview

Customer segmentation helps businesses understand their customers and develop targeted marketing, retention, and engagement strategies.

In this project, customer transaction data is cleaned and analyzed using Python. RFM (Recency, Frequency, Monetary) Analysis is then performed to evaluate customer purchasing behavior and segment customers into meaningful groups.

The final insights are presented through an interactive Power BI dashboard.

## 🎯 Objectives

- Clean and prepare raw customer transaction data
- Analyze customer purchasing behavior
- Calculate Recency, Frequency, and Monetary metrics
- Assign RFM scores to customers
- Segment customers based on their RFM scores
- Identify high-value and at-risk customers
- Analyze revenue contribution by customer segment
- Build an interactive Power BI dashboard
- Generate actionable business recommendations

## 🛠️ Tools & Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Jupyter Notebook
- Power BI
- Excel / CSV

## 🧹 Data Cleaning & Preparation

The raw transaction dataset was processed using Python.

The following data preparation steps were performed:

- Checked dataset structure and data types
- Identified missing values
- Removed duplicate records
- Removed cancelled transactions
- Removed invalid transaction values
- Removed records with invalid unit prices
- Created a new `TotalAmount` column

### Total Amount Calculation

`TotalAmount = Quantity × UnitPrice`

## 📈 RFM Analysis

RFM Analysis was used to evaluate customer behavior using three key metrics:

### Recency (R)

Measures how recently a customer made a purchase.

Lower Recency indicates a more recent purchase and is considered better.

### Frequency (F)

Measures how frequently a customer made purchases.

Higher Frequency indicates more frequent purchasing behavior.

### Monetary (M)

Measures how much money a customer spent.

Higher Monetary value indicates a more valuable customer.

Each RFM metric was converted into a score from 1 to 5. These scores were then combined to create an overall RFM Score.

`RFM Score = R Score + F Score + M Score`

The final RFM Score ranges from 3 to 15.

## 👥 Customer Segmentation

Customers were segmented based on their overall RFM Score.

| Segment | RFM Score | Description |
|---|---:|---|
| 🏆 Champions | 14–15 | Highly valuable and engaged customers |
| 💎 Loyal Customers | 12–13 | Strong and regularly purchasing customers |
| 🌱 Potential Loyalists | 9–11 | Customers with potential to become loyal |
| ⚠️ At Risk | 6–8 | Customers showing weaker engagement |
| 😴 Lost Customers | 3–5 | Low-engagement or inactive customers |

### Customer Distribution

- At Risk: 1,188 customers
- Potential Loyalists: 1,022 customers
- Lost Customers: 885 customers
- Champions: 642 customers
- Loyal Customers: 601 customers

## 📊 Power BI Dashboard

The interactive Power BI dashboard provides a consolidated view of customer behavior and segment performance.

### Dashboard Features

- Total Customers KPI
- Total Revenue KPI
- Total Orders KPI
- Average RFM Score KPI
- Customer Segment Distribution
- Customers by Segment
- Revenue by Customer Segment
- Average Spending by Segment
- Recency vs Customer Spending
- Frequency vs Customer Spending
- Interactive Customer Segment filter
- Interactive RFM Score filter
- Interactive Recency filter

## 💡 Key Business Insights

- At Risk is the largest customer segment, indicating a significant customer retention opportunity.
- Champions represent highly valuable customers who should be retained through loyalty programs and personalized offers.
- Loyal Customers can be targeted with exclusive benefits and cross-selling opportunities.
- Potential Loyalists represent an opportunity to increase customer engagement and convert them into loyal customers.
- At Risk and Lost Customers can be targeted through re-engagement and win-back campaigns.
- Revenue and average spending analysis helps identify the segments contributing most to overall business value.

## 📁 Project Structure

```text
Customer-Segmentation-RFM-Analysis/
│
├── Dashboard/
│   ├── Customer Segmentation Dashboard.pbix
│   └── Dashboard Screenshot.png
│
├── Dataset/
│   └── Customer_RFM_Segmentation.csv
│
├── Notebook/
│   └── Customer Segmentation & RFM Analysis.ipynb
│
├── SQL Queries/
│   └── Customer Segmentation Analysis.sql
│
└── README.md

## 📌 Project Flow

Raw Transaction Data
        ↓
Data Cleaning & Preparation
        ↓
Customer-Level RFM Calculation
        ↓
RFM Scoring
        ↓
Customer Segmentation
        ↓
Business Analysis
        ↓
Power BI Dashboard
        ↓
Business Insights & Recommendations

📌 Business Recommendations
1. Retain Champions
Provide loyalty rewards and exclusive offers.
Encourage repeat purchases.
Build long-term customer relationships.
2. Strengthen Loyal Customers
Use personalized product recommendations.
Introduce loyalty benefits.
Encourage cross-selling and upselling.
3. Convert Potential Loyalists
   Provide targeted promotions.
   Encourage more frequent purchases.
   Offer personalized recommendations.
4. Re-engage At Risk Customers
   Launch personalized win-back campaigns.
   Offer limited-time discounts.
   Identify reasons for declining engagement.
5. Recover Lost Customers
   Run targeted reactivation campaigns.
   Provide relevant offers.
   Analyze previous purchasing behavior to improve re-engagement.
👨‍💻 Author

Harsh Jain

B.Tech CSE | Data Analytics Enthusiast

⭐ Conclusion

This project demonstrates an end-to-end customer analytics workflow, starting from raw transaction data cleaning and RFM analysis to customer segmentation and interactive business intelligence reporting.

The combination of Python, RFM Analysis, and Power BI transforms raw transaction data into meaningful customer insights that can support better marketing, customer retention, and revenue strategies.
