# PhonePe Transaction Analysis Dashboard

A Power BI dashboard analyzing PhonePe transaction data — tracking volume, value, user growth, and success rates across services and time.

## 📊 Overview

This single-page interactive dashboard provides a snapshot of PhonePe transaction activity, combining key performance indicators with trend and breakdown visuals for deeper analysis.

## 🔑 Key Metrics (KPI Cards)
- **Total Transactions** 
- **Total Transaction Value**
- **Total Users**
- **Success Rate**
- **Month-over-Month Transaction Growth (%)**

## 📈 Visuals
- **Column charts** — transaction breakdown by *Service* and *Payment Status*
- **Line chart** — transaction trends over time by *Month*
- **Slicer** — interactive filtering across the dashboard

## 🗂️ Data Model
- `All_Transactions` — core transaction-level fact table
- `Date_table` — date dimension table for time intelligence (MoM calculations, trend analysis)

## 🛠️ Tools Used
- Power BI Desktop (data modeling, DAX measures, visualization)

## 🚀 Screenshots
1. Dashboard<img width="1372" height="767" alt="Screenshot 2026-07-04 104235" src="https://github.com/user-attachments/assets/02ab77b0-be15-47a8-9c28-a09d33e1e452" />
2. Raw Data
<img width="1587" height="870" alt="Screenshot 2026-07-04 104307" src="https://github.com/user-attachments/assets/4741fad4-68ca-439d-8ce8-942164f54f9e" />
3. Data Modelings
<img width="1523" height="853" alt="Screenshot 2026-07-04 104350" src="https://github.com/user-attachments/assets/920a563c-9eb1-46db-bf30-cc25dc319840" />





## 📌 Key Insight(s)

Scale of the data: 300,000 transactions from 107,658 users, totaling ₹3.47 billion in transaction value across 2024.

1. Loans drive the value, Money Transfers drive the volume
Loans account for just 17% of transaction count (50,000) but 73% of total value (₹2.53B) — driven by high-ticket items like Bike Loans, Mutual Funds, and Gold Loans (each ~₹630M). Money Transfers are the opposite: 50% of all transactions (150,000) but only 11% of value — lots of small P2P transfers.

2. Success rate is strong but failures are concentrated
96% success rate overall (287,993 successful / 9,980 failed / 2,027 pending). Failures aren't random — "Server error" (41%) and "Wrong PIN" (33%) account for ~74% of all failures, suggesting a technical/UX fix (better PIN retry flow, backend stability) could meaningfully cut failed transactions.

4. Transaction activity is remarkably stable month-to-month
Monthly transaction count stays in a tight band (24,000–25,700) all year with no major seasonal spike or dip — this is a mature, steady-state usage pattern rather than growth or decline.

5. Gen X and Millennials are the core user base — but Gen Z is close behind
Gen X (40,268) and Millennials (40,161) dominate the user base, with Gen Z at 22,324 and Boomers a small tail (4,905). Interestingly, average transaction value is nearly identical across all age groups (~₹11,500–11,700) — spending behavior doesn't vary much by generation here.

6. User acquisition is steady, not viral
New user sign-ups run at a consistent ~4,300–4,700/month from Aug 2023 through mid-2025, with no acquisition spikes — again pointing to steady organic growth rather than a marketing-driven surge.
-
-

---
*Note: Sample/demo dataset used for analysis purposes.*
