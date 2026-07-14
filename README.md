# Auto Loan Securitisation & Credit Risk Analytics Dashboard

## 📊 Project Overview
This repository contains an institutional-grade Asset-Backed Securitisation (ABS) and Credit Risk Analytics platform built using Power BI, Advanced DAX, and automated data validation layers. The project implements structured finance principles to analyze a ₹517.76M retail auto loan portfolio, providing senior leadership and external investors with granular visibility into credit performance, cash flow distribution mechanisms, degradation curves, and macroeconomic stress resilience.

The technical architecture utilizes a highly optimized **Star Schema Relational Model** ensuring microsecond query performance across transaction histories, dynamic monthly tracking periods, and static vintage pools.

---

## 📂 Project Repository Structure
This private repository houses the complete submission package required by the securitisation performance evaluation guidelines:

1. **`Auto_Loan_Securitisation_Risk_Dashboard.pbix`**
   * The core Power BI dashboard containing the production data model, interactive visualizations, transition heatmaps, and custom 'What-If' parameter simulation slicers.
2. **`Auto_Loan_Securitisation_Executive_Presentation.pptx`**
   * A 10-slide, high-impact PowerPoint presentation designed for C-suite executive reporting. It features a consistent corporate carbon-fiber and corporate navy aesthetic, breaking down core KPIs, vintage curves, waterfall health, and data security controls.
3. **`Securitisation_Risk_Calculations_Crosscheck.xlsx`**
   * An Excel data dictionary and math verification ledger. It serves as the data truth crosscheck, documenting every custom DAX formula, syntax, and structural layer validation.
4. **`README.md`**
   * This technical documentation guide detailing setup, architecture, and submission metrics.

---

## 📈 Core Pool Performance Metrics (Baseline KPIs)
The analytical engine monitors and dynamically computes the following key credit metrics across the collateral pool:
* **Total Outstanding Portfolio Balance:** ₹517,763,704 (₹517.76M) — Represents the total absolute principal credit exposure across the live book.
* **Active Customer Base:** 485 Unique Account Profiles.
* **Weighted Average Coupon (WAC):** 11.45% — The true annualized interest yield of the asset pool, weighted against specific loan contract balance sizes rather than a simple arithmetic mean.
* **Weighted Average Maturity (WAM):** 43.5 Months — The true residual lifecycle duration of the portfolio prior to maturity principal collection.
* **Portfolio Delinquency Ratio (30+ DPD):** 2.45% — Highly stable credit quality comfortably below the corporate target risk threshold (< 3.00%).

---

## 🛠️ Advanced Analytics & Modeling Frameworks

### 1. Cash Flow Distribution Waterfall
Modeled a sequential structured finance cash flow distribution hierarchy to simulate monthly asset cash collections (amounting to ₹18.59M in the latest reporting tracking block):
* **Tranche A (Senior Notes):** Allots a 70% structural principal allocation paying a protected market coupon yield of 6.50% per annum (Fully Met).
* **Tranche B (Mezzanine Notes):** Allots a 20% structural principal allocation paying a higher-risk premium coupon yield of 8.50% per annum (Fully Met).
* **Excess Spread (Equity Layer):** The residual cash flow (₹15.90M) is funneled to the lowest equity tier, acting as a powerful first-loss credit enhancement buffer to safeguard external debt investors.
* **Loss Trigger Alarm:** A DAX-driven systemic switch returning a binary flag (`1` for Alert / `0` for Safe). It triggers automatically if the `MonthlyNetLossRate` spikes above 1.50%, isolating and altering cash flow routing to protect senior capital.

### 2. DPD Roll Rate Heatmap
Constructed a transition probability matrix tracking account movement month-over-month from `Current` status down to `90+ DPD Default`. This conditional heatmap calculates historical migration trends, giving risk teams early warnings to optimize collections allocation before accounts decay into deep defaults.

### 3. Static Pool Vintage Loss Curves
Plots cumulative net losses on the Y-axis against Months on Book (MOB) on the X-axis, categorized by quarterly loan origination cohorts (e.g., 2021-Q1 vs 2023-Q2). This tracking isolates credit policy drift over time, visually signaling if a newer underwriting generation decays faster than long-term historical baselines.

### 4. Interactive Macro Stress Parameters
Built real-time interactive parameters enabling dynamic scenario analysis:
* **Simulated Default Rates:** Configured from 0.00% up to an extreme 10.00% crisis boundary (moving in 0.5% increments).
* **Simulated Prepayment Rates (CPR):** Configured from 0.00% to 30.00% (moving in 1.0% increments).
* **Output Vector:** Dynamically computes `Stressed Expected Loss Amount` inside a dedicated KPI card visual, calculating portfolio loss impact instantaneously under varied economic shock matrices.

---

## 🔒 Security & Data Governance
Designed and embedded **Row-Level Security (RLS)** within the production data engine using optimized DAX expressions:
1. **`Western Region Manager` Role:** Limits data access using structural criteria (`[Region] = "West"`). Regional staff see only their local territory's assets, preserving client confidentiality.
2. **`Senior Executive` Role:** Strips away filter caps, allowing comprehensive portfolio aggregation for macro reporting and C-suite reporting.

---

## 🏛️ Real-World Credit Risk Context
The architecture addresses critical structural errors exposed by major financial crises:
* **The 2008 Global Financial Crisis (GFC):** Caused by subprime mortgage pools built with opaque slicing, faulty credit ratings, and a complete absence of transparent vintage curve metrics that masked systemic pool degradation.
* **The 2018 IL&FS Liquidity Crisis (India):** Triggered by extreme asset-liability mismatches when short-term institutional papers funded highly illiquid long-term underlying structures.
* **Systemic Resolution:** Implementing automated, transparent analytics dashboards with granular transaction tracking, interactive stress parameter validation, and visible roll-rate analysis directly prevents structural default traps and ensures strict operational solvency.

---

## 🎯 Submission Protocol
This project concludes the 15-day Securitisation Capstone framework. In accordance with strict transfer protocols, repository ownership is officially being transferred to the grading account: **`ZethetaIntern`** via the GitHub Danger Zone repository transfer utility.
