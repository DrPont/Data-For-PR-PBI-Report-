# 📊 Georgian Banking Market Intelligence Dashboard

An automated, end-to-end Business Intelligence report providing a comprehensive market overview and competitive analysis of the Georgian commercial banking sector. This report relies on regulatory data provided by the **National Bank of Georgia (NBG)** via "Data for PR," tracking sector dynamics from **January 2023 to May 2026**.

> 🔒 **Confidentiality Note:** To maintain data privacy, financial figures and amounts for **Liberty Bank** have been deliberately modified/masked. System-wide patterns and comparative metrics remain fully intact for evaluation.

---

## 🚀 Overview & Scope

This report serves as a centralized hub for tracking performance, growth trajectories, and financial health ratios across all operating commercial banks in Georgia. By integrating automated extraction pipelines with robust data modeling, the dashboard translates dense regulatory filings into dynamic, scannable market insights.

* **Reporting Period:** January 2023 – May 2026 (Present).
* **Update Frequency:** Fully automated pipeline for continuous data gathering and rendering.
* **Analysis Depth:** Covers systemic market shares, growth metrics (MoM, YoY, YTD), nominal vs. real changes, and currency-denominated fluctuations (GEL/FX).

---

## 🛠️ Technical Stack

The architecture leverages a robust mix of enterprise database tools, scripting languages, and advanced BI modeling:

* **Data Extraction & Scraping:** Python (BeautifulSoup/Requests) pipelines deployed via Jupyter Notebooks.
* **Database & Orchestration:** Oracle SQL (Stored Procedures, Scheduled Jobs, Complex Queries).
* **ETL & Data Transformation:** Power Query & M Language (for clearing and reshaping structural Excel files).
* **Data Modeling & Analytics:** DAX (Data Analysis Expressions) for complex time intelligence and financial ratios.
* **UI/Visual Framework:** JSON customization code for tailored report themes and layout optimizations.

---

## 🔄 Data Pipeline Architecture

1. **Extraction:** Python scripts automatically scrape the NBG website to gather the latest "Data for PR" files.
2. **Staging & Cleaning:** Raw files are routed through Python pipelines in Jupyter and Power Query to handle data type casting, null management, and structural formatting.
3. **Warehousing:** Cleaned components are indexed and maintained via Oracle SQL databases using optimized stored procedures and scheduled jobs.
4. **Modeling & Visualization:** Data is ingested into the BI engine, where a star-schema model utilizes dynamic DAX measures to output real-time calculations.

---

## 📈 Key Insights & Dashboard Pages

The report is divided into target views to serve both macro-level sector reviews and micro-level bank comparisons:

### 1. Market Categorization & Peer Tiers (Pages 1-2)
* **Tier-Based Grouping:** Banks are structurally organized into Tiers (Tier 1, Tier 2, Tier 3) to evaluate collective group performance against systemic metrics.
* **Deep-Dive Focus:** A dedicated page highlights **7 chosen commercial banks** (including BOG, TBC, Liberty, Basis, Credo, Tera, and Silk) for cross-sectional KPI benchmarking.

### 2. Comprehensive Financial Analysis
* **Balance Sheet Dynamics:** Tracks total assets, loan portfolios, loan loss reserves, and structured liability metrics.
* **Profit & Loss (P&L) Statements:** Granular breakdown of Net Interest Income, Net Fee & Commission (F&C), Foreign Exchange (FX) trading gains/losses, operating expenses, and provisioning.

### 3. Custom Financial Coefficients & Ratios
Dozens of advanced banking ratios are built into the report framework using core Balance Sheet (BS) and P&L indicators:
* **Profitability:** Return on Equity (ROE Cumulative) and Return on Assets (ROA).
* **Margins & Yields:** Net Interest Margin (NIM on Assets/Loans/Cash), Loan Yield, Cost of Deposits, and overall Cost of Funds.
* **Risk & Efficiency:** Efficiency Ratio (Cost to Income), Cost of Risk (Loans vs. Assets), and Expected Credit Loss (ECL) Rates.

### 4. Granular Segmentation Pages
* **Loan Portfolios:** Deep dive into loan allocations by distinct macroeconomic sectors (e.g., Real Estate, Construction, Energy, Trade) and micro-level retail product segments (e.g., Mortgages, Consumer Loans, Payrolls, Credit Cards).
* **Deposit Structures:** Micro-analysis split by deposit types (Client Deposits, Legal Entities, Individuals, and Non-Bank Financial Institutions).

---

## 📸 Sample Visual Matrix (Data Snippet)

Below is an indicative slice of the comparative performance metrics captured dynamically within the report engine:

| Financial Item / Coefficient | Bank of Georgia (BOG) | TBC Bank | Liberty Bank (Masked) | Basis Bank | Credo Bank |
| :--- | :---: | :---: | :---: | :---: | :---: |
| **Total Assets** | 43,243.59M | 39,790.78M | 6,335.59M | 6,216.65M | 4,047.93M |
| **Loan Portfolio** | 29,000.43M | 28,005.60M | 4,597.77M | 3,752.28M | 3,363.67M |
| **Total Deposits** | 29,544.54M | 26,780.72M | 4,820.17M | 4,143.44M | 1,962.01M |
| **Net Income** | 818.68M | 562.36M | 41.71M | 61.79M | 28.84M |
| **ROE** | 32.31% | 23.47% | 14.15% | 16.53% | 14.25% |
| **Cost to Income** | 27.32% | 33.89% | 70.32% | 40.43% | 52.27% |

---
_Note: This README serves as documentation for the static PDF snapshot version of the live, automated tracking report._
