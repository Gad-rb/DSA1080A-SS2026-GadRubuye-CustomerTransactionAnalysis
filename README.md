# Customer Transaction & Behavior Analysis

**DSA1080A – Programming for Data Science | Spring Semester 2026 | USIU-Africa**

---

## Project Overview

This project presents an end-to-end data analysis of customer transaction behavior using Python. The analysis focuses on understanding purchase frequency, revenue distribution, repeat vs. new customer patterns, and spending behavior across a real-world e-commerce dataset.

---

## Dataset

| Detail | Information |
|---|---|
| **Dataset Name** | E-Commerce Data (Online Retail Dataset) |
| **Source** | UCI Machine Learning Repository via Kaggle |
| **Link** | https://www.kaggle.com/datasets/carrie1/ecommerce-data |
| **Raw Rows** | 541,909 rows |
| **Cleaned Rows** | 392,692 rows |
| **Columns after Feature Engineering** | 34 columns |
| **Format** | CSV (Structured tabular data) |

### Variable Descriptions

| Variable | Description |
|---|---|
| `InvoiceNo` | Unique transaction identifier. Prefix 'C' indicates cancellation. |
| `StockCode` | Unique product/item code. |
| `Description` | Name/description of the product. |
| `Quantity` | Number of units purchased per transaction. |
| `InvoiceDate` | Date and time of the transaction. |
| `UnitPrice` | Price per unit of product in GBP (£). |
| `CustomerID` | Unique identifier for each customer. |
| `Country` | Country where the customer is based. |
| `Revenue` | Derived: Quantity × UnitPrice. Primary financial metric. |
| `Month` | Extracted from InvoiceDate for time-based analysis. |
| `DayOfWeek` | Extracted from InvoiceDate for activity pattern analysis. |
| `Hour` | Extracted from InvoiceDate for peak hour analysis. |

---

## Research Questions

1. What is the distribution of purchase frequency across customers, and what proportion are high-frequency buyers?
2. How does revenue per customer vary, and which customer segment contributes most to total revenue?
3. What is the ratio of repeat to new customers, and what is the probability of a second purchase?
4. How is spending distributed across the customer base, and what does the distribution shape reveal?
5. Which countries generate the highest revenue, and how does behavior differ across regions?

---

## Project Structure
```
DSA1080A-SS2026-GadRubuye-CustomerTransactionAnalysis/
│
├── data/
│   ├── raw_dataset.csv
│   └── cleaned_dataset.csv
│
├── visuals/
│   ├── top10_products_revenue.png
│   ├── monthly_revenue_trend.png
│   ├── customer_spending_distribution.png
│   ├── revenue_by_country_boxplot.png
│   └── activity_heatmap.png
│
├── notebook.ipynb
├── report.pdf
└── README.md
```

---

## Tools Used

- **Python 3** — primary programming language
- **Jupyter Notebook** — development environment
- **pandas** — data loading, cleaning, and manipulation
- **matplotlib & seaborn** — data visualization
- **numpy** — numerical operations
- **GitHub** — version control and project submission
- **Claude AI (Anthropic)** — AI assistance (declared per academic integrity policy)

---

## Key Findings

1. **Revenue is highly seasonal** — November 2011 was the peak month at £1,156,205, with Q4 (September–November) accounting for a disproportionate share of annual revenue, driven by pre-holiday wholesale purchasing activity.

2. **Customer spending is strongly right-skewed** — the median customer spends £658 in total while the mean is £1,406, confirming that a small high-value segment drives a disproportionate share of revenue. The top customer alone generated £280,206.

3. **The United Kingdom dominates total revenue at £7,285,024 (approximately 84% of all sales)**, but has the lowest median transaction value among the top 10 countries. The Netherlands and Australia place fewer but significantly larger orders, with median transaction values of approximately £90 and £65 respectively.

4. **A small set of products drives the majority of revenue** — PAPER CRAFT, LITTLE BIRDIE leads at approximately £165,000, followed by REGENCY CAKESTAND 3 TIER at £140,000. The top 3 products account for a substantial share of total product revenue.

5. **Purchase activity is concentrated in weekday business hours** — Tuesday to Thursday between 09:00 and 13:00 represent the highest-revenue windows, consistent with a B2B wholesale customer base operating on standard business schedules. Saturday is entirely inactive.

*Additional insights to be added upon Week 4 advanced analysis completion.*

---

## Methodology

Statistical methods from STA1020 — including distribution analysis, IQR-based outlier detection, and probability estimation — were applied throughout this analysis to ensure findings are statistically grounded.

Python concepts from DSA1060 were also applied throught the project

---
## Student Information

| Detail | Information |
|---|---|
| **Full Name** | Gad Rubuye |
| **Student ID** | 677569 |
| **Course** | DSA1080A – Programming for Data Science |
| **Institution** | USIU-Africa |
| **Semester** | Spring Semester 2026 |

---

## Academic Integrity Declaration

This project was completed individually with AI assistance from Claude (Anthropic). All analysis, code, and insights were built from scratch using the declared dataset. No Kaggle notebooks or external GitHub projects were copied. All sources are cited.

---

*Last updated: Week 3 — Exploratory Data Analysis complete*
