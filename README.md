# Bank-Loan-Analytics-Dashboard-End-to-End-Power-BI-Project
End-to-End Bank Loan Analytics Dashboard built in Power BI — analyzing 38K+ loan records to track KPIs, Good vs Bad loan performance, borrower risk profiles, and monthly lending trends across the US.

# 🏦 Bank Loan Analytics Dashboard — End-to-End Power BI Project

![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![Excel](https://img.shields.io/badge/Microsoft%20Excel-217346?style=for-the-badge&logo=microsoft-excel&logoColor=white)
![DAX](https://img.shields.io/badge/DAX-Measures-blue?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen?style=for-the-badge)

---

> 💡 **Transforming 38,000+ raw US loan records into actionable banking intelligence — built end-to-end in Power BI.**

---

## 📌 Overview

In the banking sector, managing a loan portfolio without real-time visibility is a serious operational risk. Analysts need instant answers — *How much capital is deployed? How much is being recovered? Which borrower segments are defaulting?*

This project delivers exactly that. A **professional, 2-page interactive Power BI dashboard** that gives stakeholders a complete picture of the loan portfolio — from executive-level KPIs down to deep visual analysis — all built from scratch on a dataset of **38,576 real-world style US loan entries**.

---

## 🎯 Business Objectives

| # | Objective | How It's Solved |
|---|---|---|
| 1 | Monitor lending activity month over month | MTD & MoM KPI cards with % change indicators |
| 2 | Separate healthy vs risky loan portfolio | Good Loan vs Bad Loan segmentation panel |
| 3 | Identify high-risk borrower segments | Grade, Sub-Grade, DTI & Employment analysis |
| 4 | Track repayment vs disbursement performance | Funded Amount vs Amount Received KPIs |
| 5 | Geo-analysis of loan distribution | US State filled map visual |

---

## 📊 Dashboard Pages

### 📋 Page 1 — Summary

The command center for decision-makers. Tracks the most critical portfolio metrics at a glance with **Month-to-Date (MTD)** values and **Month-over-Month (MoM) % change** indicators — all powered by DAX time intelligence.

| KPI Metric | Description |
|---|---|
| Total Loan Applications | Total volume of loan requests received |
| Total Funded Amount | Total principal capital disbursed to borrowers |
| Total Amount Received | Total repayments collected from borrowers |
| Average Interest Rate | Mean cost of lending across the entire portfolio |
| Average DTI | Mean borrower Debt-to-Income ratio |

Also features the most important risk panel in the dashboard — **Good Loan vs Bad Loan** — showing percentage split, application count, funded amount, and amount received for each segment.

---

### 📈 Page 2 — Overview

Six powerful visual breakdowns for deep portfolio understanding:

- 📅 **Monthly Trend** — loan application volume tracked across all 12 months of 2021
- 🗺️ **US State Map** — geographic concentration of lending activity across all US states
- ⏱️ **Loan Term Analysis** — 36-month vs 60-month loan distribution and comparison
- 💼 **Employment Length** — borrower job stability vs loan volume correlation
- 🎯 **Loan Purpose** — why borrowers are taking loans (debt consolidation, home improvement, car, etc.)
- 🏠 **Home Ownership** — RENT vs MORTGAGE vs OWN impact on lending behavior

---

## 🗃️ Dataset

| Property | Details |
|---|---|
| File | `Financial_loan_data.xlsx` |
| Total Records | **38,576 loan entries** |
| Total Columns | **23 attributes** |
| Time Period | January 2021 — December 2021 |
| Geography | United States (all states) |

**Key Columns:**

| Column | Description |
|---|---|
| `LOAN_AMOUNT` | Principal amount approved |
| `LOAN_STATUS` | Fully Paid / Current / Charged Off |
| `INT_RATE` | Interest rate (stored as decimal) |
| `DTI` | Debt-to-Income ratio |
| `GRADE / SUB_GRADE` | Risk classification — A1 through G5 |
| `PURPOSE` | Reason for loan application |
| `ANNUAL_INCOME` | Borrower's yearly income |
| `TOTAL_PAYMENT` | Total amount repaid by borrower |
| `TERM` | Loan duration — 36 or 60 months |
| `ADDRESS_STATE` | US state of the borrower |
| `HOME_OWNERSHIP` | RENT / MORTGAGE / OWN |
| `EMP_LENGTH` | Borrower employment duration |

---

## 🛠️ Tech Stack

| Tool | Purpose |
|---|---|
| **Power BI Desktop** | Dashboard design, visuals, slicers, interactivity |
| **Power Query (M Language)** | Data ingestion, cleaning and transformation |
| **DAX** | Custom KPI measures — MTD, MoM%, ratios, conditionals |
| **Microsoft Excel (.xlsx)** | Raw data source |

---

## 📐 DAX Measures Written

- `Total Loan Applications` — COUNT with dynamic slicer context
- `MTD Loan Applications` — DATESMTD time intelligence function
- `MoM% Applications` — DIVIDE + PARALLELPERIOD for period-over-period comparison
- `Total Funded Amount` — SUM with filter context
- `Total Amount Received` — SUM with repayment filter
- `Good Loan %` — CALCULATE + DIVIDE with Fully Paid / Current filter
- `Bad Loan Funded Amount` — CALCULATE with Charged Off status filter
- `Avg Interest Rate` — AVERAGE with dynamic filter context
- `Avg DTI` — AVERAGE with conditional formatting threshold logic

---

## 💡 Key Business Insights Uncovered

- ✅ **83.4% Good Loan Rate** — majority of the portfolio is healthy (Fully Paid + Current)
- ⚠️ **16.6% Bad Loans** — Charged Off loans represent significant capital loss, heavily concentrated in Grade D–G borrowers
- 📌 **Debt Consolidation is #1 purpose** — nearly 47% of all applications cite this as their reason
- 📉 **60-month borrowers pay more** — average interest rate is 2–3% higher than 36-month loan holders
- 🏙️ **CA, NY & TX lead in volume** — these 3 states account for the highest loan application counts nationally
- 💼 **10+ year employees dominate** — the most stable and largest borrower segment by employment length

---

## 📁 Repository Structure

```
📦 Bank-Loan-Analytics-Dashboard/
│
├── 📊  Bank Loan Analytics Dashboard.pbix     ← Open in Power BI Desktop
├── 📂  Financial_loan_data.xlsx               ← Source dataset (38,576 rows × 23 cols)
├── 📑  Problem Statement.pptx                 ← KPI requirements & dashboard specs
└── 📖  README.md                              ← You are here
```

---

## ▶️ How to Run This Project

```
Step 1 — Clone this repository
git clone https://github.com/YOUR-USERNAME/Bank-Loan-Analytics-Dashboard.git

Step 2 — Download Power BI Desktop (free)
https://powerbi.microsoft.com/desktop/

Step 3 — Open the dashboard file
File → Open → Select Bank Loan Analytics Dashboard.pbix

Step 4 — Reconnect data source if prompted
Home → Transform Data → Data Source Settings
→ Update path to your local Financial_loan_data.xlsx

Step 5 — Click Refresh and explore both pages!
```

---

## 📸 Dashboard Preview

| Summary Page | Overview Page |
|---|---|
| ![Summary](IMAGES/HI_page-0001.jpg) | ![Overview](IMAGES/HI_page-0002.jpg) |

---

## 🧩 Skills Demonstrated

`Power BI` &nbsp;|&nbsp; `DAX` &nbsp;|&nbsp; `Power Query` &nbsp;|&nbsp; `Data Modeling` &nbsp;|&nbsp; `Time Intelligence` &nbsp;|&nbsp; `KPI Dashboard Design` &nbsp;|&nbsp; `Financial Analytics` &nbsp;|&nbsp; `Data Cleaning` &nbsp;|&nbsp; `Storytelling with Data`

---

## 📬 Connect With Me

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/YOUR-PROFILE)
[![GitHub](https://img.shields.io/badge/GitHub-Follow-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/YOUR-USERNAME)

---

<p align="center">⭐ If you found this useful, please star the repo — it helps others discover this project!</p>
