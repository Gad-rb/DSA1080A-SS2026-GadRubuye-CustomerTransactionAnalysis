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
| **Number of Rows** | 541,909 rows |
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

*To be completed upon project finalization in Week 4.*

---

## Methodology

Statistical methods from STA1020 — including distribution analysis, IQR-based outlier detection, and probability estimation — were applied throughout this analysis to ensure findings are statistically grounded.

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

*Last updated: Week 1 — Proposal & Setup*
