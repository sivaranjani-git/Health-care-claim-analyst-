# 🏥 Healthcare Claims Analytics Dashboard

**End-to-end revenue cycle analytics solution built with SQL, Python, and Power BI to analyze healthcare claims, uncover denial patterns, and improve reimbursement performance.**

![Status](https://img.shields.io/badge/status-active-brightgreen)
![Tools](https://img.shields.io/badge/tools-SQL%20%7C%20Python%20%7C%20Power%20BI-blue)
![Domain](https://img.shields.io/badge/domain-Healthcare%20RCM-orange)

---

## 📌 Overview

Healthcare providers lose significant revenue every year due to claim denials, payment delays, and inefficient AR management. This project simulates a real-world **Revenue Cycle Management (RCM)** workflow — from raw claims data to an interactive executive dashboard — to help stakeholders identify **why claims are denied, where payments are delayed, and how collection performance can be improved.**

The project mirrors the day-to-day analysis performed by **Healthcare Claims Analysts, Revenue Cycle Analysts, and Healthcare Data Analysts**, combining hands-on **AR/Medical Billing domain knowledge** with **data analytics and BI tooling**.

---

## 🎯 Objective

Analyze healthcare claims data to:
- Identify denial patterns and root causes
- Track payment delays and AR aging
- Measure reimbursement and collection trends
- Build KPI-driven dashboards to support faster, data-backed revenue cycle decisions

---

## 🛠️ Tools & Technologies

| Category | Tools |
|---|---|
| Database / Querying | SQL (SQL Server / PostgreSQL / MySQL) |
| Data Wrangling & Analysis | Python (Pandas, NumPy, Matplotlib/Seaborn) |
| Visualization / BI | Power BI |
| Supporting Tools | Excel, Jupyter Notebook |

---

## 🗃️ Dataset

Simulated healthcare claims dataset containing:

`Claim ID` · `Patient ID` · `Provider` · `Insurance Payer` · `CPT Code` · `ICD-10 Code` · `Date of Service` · `Billed Amount` · `Allowed Amount` · `Paid Amount` · `Adjustment Amount` · `Denial Code` · `Denial Reason` · `Claim Status` · `Days in AR` · `Place of Service` · `State`

> Note: Data is synthetically generated / anonymized for demonstration purposes and does not represent real patient or provider information (HIPAA-safe).

---

## 📁 Repository Structure

```
healthcare-claims-analytics-dashboard/
│
├── data/
│   ├── claims_data.csv              # raw synthetic dataset (5,015 rows)
│   ├── claims_data_cleaned.csv      # cleaned dataset (output of notebook)
│   └── claims_kpi_summary.xlsx      # exported KPI tables for reporting
│
├── sql/
│   ├── 00_create_table.sql
│   ├── 01_claims_by_payer.sql
│   ├── 02_denials_by_reason.sql
│   ├── 03_monthly_payment_trend.sql
│   ├── 04_avg_days_in_ar.sql
│   ├── 05_top_denied_cpt_codes.sql
│   └── 06_provider_wise_collections.sql
│
├── python/
│   └── healthcare_claims_analysis.ipynb   # cleaning, KPIs, trends, visualizations (pre-executed)
│
├── powerbi/
│   ├── POWER_BI_SETUP_GUIDE.md      # DAX measures + page-by-page build guide
│   └── Healthcare_Claims_Dashboard.pbix   # (build in Power BI Desktop using the guide)
│
├── images/
│   ├── monthly_trend.png
│   ├── top_denial_reasons.png
│   ├── collection_rate_by_payer.png
│   ├── ar_aging.png
│   └── claim_status_breakdown.png
│
└── README.md
```

---

## 📊 Key Performance Indicators (KPIs)

- Total Claims Processed
- Total Billed Amount vs Total Paid Amount
- **Collection Rate** = Total Paid / Total Billed
- **Denial Rate** = Denied Claims / Total Claims
- **First-Pass Resolution Rate** = Claims paid without resubmission
- Average Days in AR
- Top Denial Reasons
- Claims Volume & Value by Payer
- Claims Volume & Value by Provider

---

## 🧮 SQL Analysis

- Total claims and billed/paid amounts by payer
- Denial breakdown by reason and denial code
- Monthly payment and collections trend
- Average Days in AR by payer/provider
- Top denied CPT codes
- Provider-wise collection performance

---

## 🐍 Python Analysis

- Data cleaning and missing value handling
- Standardizing payer names, CPT/ICD-10 codes, and date formats
- KPI calculation (collection rate, denial rate, AR aging buckets)
- Trend analysis across time, payer, and provider
- Exploratory visualizations (denial trends, payment trends, AR aging distribution)

---

## 📈 Power BI Dashboard

**7 Dashboard Pages:**
1. **Executive Summary** — high-level KPIs and financial snapshot
2. **Claims Overview** — claim volume, status breakdown, trends
3. **Denial Analysis** — denial rate, top denial reasons, denied CPT codes
4. **Payer Performance** — collection rate and turnaround by payer
5. **Provider Performance** — billed vs collected by provider
6. **AR Aging Analysis** — days-in-AR buckets and aging trends
7. **Financial Summary** — billed, allowed, paid, and adjustment analysis

**Visuals used:** KPI Cards, Bar Charts, Line Charts, Pie Charts, Heat Map, Treemap
**Interactivity:** Slicers for Payer, Provider, State, and Month

---

## 🔍 Key Insights (Sample)

- Identified the top 5 denial reasons contributing to ~60% of all denials
- Flagged payers with the longest average AR turnaround
- Highlighted providers with below-average first-pass resolution rates
- Surfaced monthly collection trends to support cash-flow forecasting

*(Replace with your actual findings once analysis is complete.)*

---

## 🚀 How to Run This Project

1. Clone the repository
   ```bash
   git clone https://github.com/<your-username>/healthcare-claims-analytics-dashboard.git
   ```
2. Load `data/claims_data.csv` into your SQL database and run scripts in `/sql`
3. Open notebooks in `/python` using Jupyter Notebook to reproduce cleaning and KPI analysis
4. Open `Healthcare_Claims_Dashboard.pbix` in Power BI Desktop to explore the interactive dashboard

---

## 👤 About This Project

This project was built to demonstrate practical, job-ready skills at the intersection of **medical billing/AR operations** and **data analytics**, applying real revenue cycle concepts (denials, AR aging, payer performance) using an industry-standard analytics stack.

**Skills demonstrated:** SQL querying, Python data wrangling, Power BI dashboard design, healthcare RCM domain knowledge, KPI design, and business storytelling with data.

---

## 📬 Connect

Feel free to reach out if you'd like to discuss this project, healthcare revenue cycle analytics, or potential collaboration opportunities.
