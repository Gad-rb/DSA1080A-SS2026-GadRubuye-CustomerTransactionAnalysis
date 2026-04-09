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

├── data/
│   ├── raw_dataset.csv
│   └── cleaned_dataset.csv
│
├── visuals/
│   ├── top10_products_revenue.png
│   ├── monthly_revenue_trend.png
│   ├── customer_spending_distribution.png
│   ├── revenue_by_country_boxplot.png
│   ├── activity_heatmap.png
│   ├── customer_segmentation.png
│   ├── repeat_vs_new_customers.png
│   ├── country_revenue_share.png
│   ├── peak_purchasing_periods.png
│   └── frequency_vs_spend_correlation.png
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

1. **Revenue is critically concentrated in a single market** — the United Kingdom accounts for 81.97% of total revenue. The next nine markets combined contribute less than 18%, creating structural geographic risk.

2. **Customer spending is strongly right-skewed** — the median customer spends £658 while the mean is £1,406. The top customer alone generated £280,206. A small high-value segment drives a disproportionate share of total revenue.

3. **65.6% repeat purchase rate confirms strong customer loyalty** — 2,845 of 4,338 customers returned for a second order, with an average of 4.27 orders per customer. The 1,493 one-time customers represent an untapped retention opportunity.

4. **Revenue is highly seasonal** — November 2011 peaked at £1,156,205, with Q4 accounting for over 40% of annual revenue. February and April are the weakest months at £446,085 and £468,374 respectively.

5. **International markets are underleveraged** — the Netherlands and Australia show median transaction values of approximately £90 and £65 per transaction respectively, significantly above the UK median of under £20, indicating high-value wholesale buying behavior.

6. **Thursday midday is the highest-value purchasing window** — Thursday generates £1,973,016 in total revenue, the highest of any day. Peak hour is 12:00 at £1,373,695. Saturday recorded zero transactions, confirming a B2B wholesale customer base.

7. **Purchase frequency and total spend are moderately correlated (r = 0.55)** — more frequent buyers tend to spend more, but order size plays an independent role, suggesting loyalty programs should reward both frequency and order value.

8. **A small set of products drives the majority of revenue** — PAPER CRAFT, LITTLE BIRDIE leads at approximately £165,000, followed by REGENCY CAKESTAND 3 TIER at £140,000. Non-product entries (POSTAGE, Manual) appear in the top 10 and must be excluded from product recommendations.

---

## Recommendations

1. **Launch a high-value customer retention program** — identify top RFM-scoring customers and assign dedicated account management with volume-based pricing incentives.

2. **Invest in international market development** — target the Netherlands and Australia with localized account managers and country-specific promotions to capitalize on their demonstrated high transaction values.

3. **Implement an H1 revenue activation campaign** — introduce early-year loyalty discounts, new product launches in January/February, and spring bundles to reduce Q4 dependency and improve cash flow stability.

---

## Methodology

Statistical methods from STA1020 including distribution analysis, IQR-based outlier detection, percentile-based segmentation, correlation analysis, and probability estimation were applied throughout this analysis to ensure findings are statistically grounded.

Programming concepts from DSA1060 — including data structures, control flow, and object-oriented principles — informed the code architecture and implementation approach used across all analytical sections.

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

*Final submission: complete project — Gad Rubuye 677569, DSA1080A SS2026*
