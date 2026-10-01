# Insurance Payout & Premium Dashboard — Power BI

![Power BI](https://img.shields.io/badge/Power%20BI-Dashboard-F2C811?logo=powerbi&logoColor=black)
![Data Analytics](https://img.shields.io/badge/Analytics-Insurance%20Portfolio-blue)
![Status](https://img.shields.io/badge/Project-Completed-success)

## 📊 Project Overview

The **Insurance Payout & Premium Dashboard** is an interactive Power BI analytics project designed to analyze insurance policies from a **premium, protection, investment, maturity, payout, customer, and sales-performance perspective**.

The dashboard converts policy-level insurance data into an interactive reporting solution that can help users understand:

- Premium collection and payment behavior
- Policy protection/coverage values
- Investment value versus maturity value
- Annual premium versus protection value
- Premium payment progress and outstanding payable amounts
- Policy tenure and payment-duration patterns
- Customer distribution by state and occupation
- Performance across policy types and protection plans
- Sales-agent and management-hierarchy performance

The project demonstrates practical skills in **Power BI, data modeling, DAX, interactive visualization, KPI design, filtering, drill-down analysis, and business storytelling**.

---

## 🎯 Business Objective

The primary objective of this dashboard is to provide a single analytical view of an insurance portfolio and answer questions such as:

1. How much premium has been generated and paid?
2. What is the total premium payable across policies?
3. How does the investment value compare with the maturity value?
4. How does annual premium compare with the protection/coverage amount?
5. Which policy types and protection plans contribute most to the portfolio?
6. How are customers distributed geographically and by occupation?
7. What is the premium-payment completion level?
8. Which sales agents and management structures are associated with higher premium or policy performance?
9. How do policy tenure and payment duration affect the portfolio?
10. Which areas may require deeper investigation from a business or portfolio-management perspective?

---

## 🖥️ Dashboard Pages

The Power BI report contains **six analytical pages**.

### 1. Summary

Provides a high-level snapshot of the insurance portfolio.

Key metrics and dimensions include:

- Total Premium Amount
- Total Annual Premium
- Total Premium Paid
- Total Premium Payable
- Customer/Policy counts
- Policy start-date trends
- Policy type
- Protection plan
- Sales agent
- Customer state
- Customer occupation

The Summary page is intended to provide a quick executive-level understanding before moving into detailed analysis.

---

### 2. Insurance Overview

Focuses on the overall insurance portfolio and premium performance.

The page supports analysis across:

- Policy Type
- Protection Plan
- Sales Agent
- Start Date
- State
- Occupation
- Annual Premium
- Premium Amount
- Underwriting Expense

Interactive filtering allows users to investigate the portfolio from different business dimensions.

---

### 3. Investment Value vs Maturity Value

This page analyzes the relationship between the amount invested/premium paid and the eventual maturity value.

Important analytical fields include:

- Total Premium Amount
- Total Premium Paid
- Maturity Amount
- Annualized ROI (%)
- Start Date
- Policy tenure

This view helps identify how policy investment characteristics translate into maturity outcomes.

---

### 4. Annual Premium vs Protection Value

This page compares the recurring annual premium against the protection/coverage amount associated with policies.

Key fields include:

- Total Annual Premium
- Sum Assured / Coverage Amount
- Annualized ROI (%)
- Tenure
- Policy Type
- Protection Plan
- Customer and agent dimensions

This comparison helps understand the relationship between the premium paid by customers and the insurance protection provided.

---

### 5. Premium Analysis — 5–20 Years

This page focuses on premium payment behavior over different policy-tenure ranges.

The analysis includes:

- Total Premium Paid
- Total Premium Payable
- Total Annual Premium
- Premium Payment Duration
- Payment Bucket
- Premium Paid %
- Premium Payable %
- Maturity Amount
- Annualized ROI
- Tenure

The page is designed to support deeper analysis of payment completion and long-duration insurance policies.

---

### 6. Sales Hierarchy

The Sales Hierarchy page analyzes performance across the insurance distribution structure.

The report includes dimensions such as:

- Sales Agent
- Zonal Manager
- Regional Manager
- State
- Policy Type
- Protection Plan
- Policy Holder
- Total Premium Amount
- Total Premium Paid
- Total Premium Payable
- Profit/Gain
- Underwriting Expense

A parameter is also used to dynamically select rows/dimensions for analysis, making the page more interactive.

---

## 🧩 Data Model

The report uses a dimensional-model approach with a central insurance policy fact table and supporting dimension tables.

### Fact Table

**`FCT Insurance_Policy_Table`**

Contains policy-level transactional and financial information such as:

- Customer ID
- Start Date
- Policy Status
- Premium Amount
- Total Annual Premium
- Total Premium Amount
- Total Premium Paid
- Total Premium Payable
- Maturity Amount
- Coverage / Sum Assured
- Tenure
- Payment Frequency
- Payment Duration
- Underwriting Expense
- Profit/Gain
- Annualized ROI
- Premium-payment metrics

### Dimension Tables

**`DM Customer_Detail_Table`**

Customer-related attributes such as:

- Customer ID
- Policy Holder Name
- State
- Occupation

**`DM Policy_Type`**

Contains policy-type classification.

**`DM Policy_Protection_Plan`**

Contains protection-plan/policy-name information.

**`DM Insurance_Agent_Table`**

Contains sales-agent information.

**`DM Regional_Manager`**

Contains regional-management information.

**`DM Zonal_Manager`**

Contains zonal-management information.

### Supporting Parameters

The report also uses Power BI parameter tables for dynamic visual analysis, including:

- `Visual- Parameter`
- `Parameter - Selecting Rows`

These parameters allow users to change analytical dimensions without creating separate visuals for every possible breakdown.

---

## 🔢 Key Metrics / Measures

The dashboard uses financial and operational measures around the following concepts:

| Metric | Purpose |
|---|---|
| Total Premium Amount | Measures the overall premium value represented in the portfolio |
| Total Annual Premium | Measures annualized premium contribution |
| Total Premium Paid | Measures premium already paid |
| Total Premium Payable | Measures premium still payable/contractually due |
| Maturity Amount | Measures expected/value-at-maturity amount represented in the data |
| Coverage / Sum Assured | Measures insurance protection value |
| Premium Paid % | Measures the proportion of payable premium that has been paid |
| Premium Payable % | Measures the proportion of premium that remains payable |
| Annualized ROI (%) | Evaluates annualized investment return represented by the policy data |
| Profit/Gain | Measures the gain/profit field available in the policy data |
| Underwriting Expense | Tracks underwriting-related expense |

> **Note:** The exact calculation logic for each measure is defined inside the PBIX model. The dashboard should be interpreted according to the source data definitions and business rules used in the report.

---

## 🔍 Interactive Features

The dashboard includes interactive filtering and analysis capabilities.

### Common Filters / Slicers

Users can analyze the portfolio by:

- Policy Type
- Policy Name / Protection Plan
- Sales Agent
- Start Date
- State
- Occupation
- Policy Status
- Tenure
- Payment-related categories

### Dynamic Analysis

The report includes parameter-driven visuals that allow users to dynamically change analytical dimensions.

This makes the dashboard useful for exploratory analysis instead of relying only on fixed charts.

### Policy Status

The report has a report-level filter configured for:

**Policy Status = Active**

This means the default report context focuses on active policies unless the filter configuration is changed.

---

## 💡 Example Business Insights

The dashboard can be used to identify insights such as:

### Premium Performance

- Compare total premium generated with total premium paid.
- Identify the outstanding premium payable.
- Analyze premium contribution by policy type and protection plan.
- Examine premium trends by policy start date.

### Customer Analysis

- Identify states with higher policy activity.
- Compare portfolio distribution across occupations.
- Analyze customer concentration by geography.

### Investment & Maturity

- Compare premium/investment value with maturity value.
- Analyze annualized ROI across policy characteristics.
- Examine how tenure affects maturity outcomes.

### Protection Analysis

- Compare annual premium with coverage/sum assured.
- Identify policy categories with relatively high protection values.
- Analyze protection characteristics by policy type and plan.

### Payment Analysis

- Identify policies with higher or lower premium-payment completion.
- Compare paid versus payable premium.
- Analyze payment behavior across different tenure buckets.

### Sales Analysis

- Compare premium performance across sales agents.
- Analyze performance by regional and zonal hierarchy.
- Drill from management levels into individual agents and policy/customer dimensions.

> These are analytical use cases supported by the dashboard; actual findings should be taken from the current data and filter context rather than assumed from the dashboard structure alone.

---

## 🛠️ Tools & Technologies

| Tool | Purpose |
|---|---|
| **Power BI Desktop** | Dashboard development and visualization |
| **Power Query** | Data preparation and transformation |
| **DAX** | Measures, calculated logic and KPIs |
| **Data Modeling** | Fact/dimension relationships and analytical structure |
| **Power BI Parameters** | Dynamic visual and row-selection analysis |
| **Excel / Source Data** | Source data preparation, where applicable |

---

## 📌 Project Workflow

```text
Raw Insurance Data
        ↓
Data Cleaning & Transformation
        ↓
Data Modeling
        ↓
Relationships & Dimensions
        ↓
DAX Measures / KPIs
        ↓
Interactive Visualizations
        ↓
Dashboard Design
        ↓
Business Insights
```

---

## 📈 Skills Demonstrated

This project demonstrates practical experience in:

- Power BI Dashboard Development
- Data Cleaning
- Power Query
- Data Modeling
- Star-schema concepts
- DAX Measures
- KPI Development
- Financial Analytics
- Insurance Analytics
- Premium & Payout Analysis
- Customer Segmentation
- Sales Performance Analysis
- Interactive Slicers
- Dynamic Parameters
- Drill-down Analysis
- Business Intelligence
- Data Storytelling

---

## 👨‍💻 Author

**Gaurav Singh**

**Skills:** Power BI • DAX • Power Query • SQL • Excel • Tableau • Python

---

## ⭐ Project Highlights

- 6 analytical Power BI pages
- Insurance portfolio KPI analysis
- Premium and payment analysis
- Investment vs maturity analysis
- Premium vs protection analysis
- 5–20 year premium analysis
- Customer and geographic analysis
- Sales-agent hierarchy analysis
- Dynamic Power BI parameters
- DAX-driven business metrics
- Interactive filtering and cross-analysis

---
