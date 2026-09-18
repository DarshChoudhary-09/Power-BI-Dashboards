# Mobile Sales Performance Dashboard — Power BI
An interactive Power BI dashboard built to analyze mobile phone sales transactions, track key revenue and volume KPIs, and surface brand, city, and payment-method trends for stakeholders.

## Project Objective
Retail and sales teams often rely on scattered spreadsheets to track performance, making it hard to spot trends quickly. This project turns raw, transaction-level mobile sales data into a self-service, interactive dashboard that lets stakeholders:

- Track headline sales KPIs (revenue, units, transactions, order value) at a glance
- Filter performance by month to spot seasonal trends
- Identify top-performing brands, models, cities, and payment methods
- Replace static, manual reporting with an on-demand, drillable view of the business.

## Dataset Used
- <a href=  "https://github.com/DarshChoudhary-09/Power-BI-Dashboards/blob/main/Day%20-%2030%20-%20Mobile%20Sales%20Data.xlsx"> Dataset </a>

## Business Questions (KPIs)
The dashboard is built to answer:

1. What is the total revenue and total units sold?
2. How many transactions were processed, and what's the average order value?
3. How does revenue trend month over month?
4. Which brand and mobile model generate the most revenue?
5. Which cities contribute the most sales?
6. Which payment method do customers prefer?
7. How does customer satisfaction (ratings) vary by brand?
8. Which day of the week sees the highest sales?

- Dashboard Interaction <a href="https://github.com/DarshChoudhary-09/Power-BI-Dashboards/blob/main/Project.pbix">View dashboard</a>


## Process
1. Data Preparation (Power Query) — Loaded the raw Excel file, checked for nulls/duplicates, and standardized inconsistent Day Name entries (e.g. "Sat" vs "Saturday").
2. Data Modeling — Structured the data into a single Sales_Data table with a Date hierarchy (Year → Month → Day) to enable time-based filtering.
3. DAX Measures — Built core measures for:
- Total Sales = SUMX(Sales_Data, Units Sold * Price Per Unit)
- Total Quantity = SUM(Units Sold)
- Transaction Count = DISTINCTCOUNT(Transaction ID)
- Average Order Value = Total Sales / Transaction Count
4. Dashboard Design — Designed a single-page report with KPI cards, a month-level slicer, and custom card-based visuals for a clean, branded look.

## Dashboard
<img width="887" height="499" alt="Screenshot 2026-09-18 211742" src="https://github.com/user-attachments/assets/6626576d-935f-4542-a228-e9cb979d21b9" />

## Project Insights
- Overall performance: The dataset covers ₹76.92 Cr in total revenue across 3,835 transactions and 19,150 units sold, at an average order value of ~₹2.01 Lakh per transaction.
- Brand performance is tightly contested: Apple leads revenue (₹16.16 Cr), closely followed by Samsung (₹16.00 Cr), OnePlus (₹15.37 Cr), -Vivo (₹15.01 Cr), and Xiaomi (₹14.38 Cr) — no single brand dominates, with each holding roughly 18–21% of total revenue.
- Top model: The iPhone SE is the single highest-revenue model (₹5.96 Cr), followed by the OnePlus Nord and Galaxy Note 20.
- City concentration: Delhi (₹20.39 Cr) and Mumbai (₹12.72 Cr) together account for over 40% of total revenue — far ahead of the next tier of cities (Ranchi, Chennai, Rajkot), each contributing ₹2.5–3.1 Cr.
- Payment preference: UPI is the most-used payment method, both by transaction count (1,011) and revenue (₹20.17 Cr), narrowly ahead of Debit Card, Credit Card, and Cash.
- Seasonality: July, March, and January are the strongest months by revenue, while September and February are comparatively weaker.
- Day-of-week trend: Saturday generates the highest revenue, with weekday sales (Wednesday, Thursday) trailing slightly behind weekend performance.
- Customer satisfaction: Average rating across all brands is 3.69/5, with Xiaomi customers reporting the highest average satisfaction (3.72/5).

## Tools Used
Power BI Desktop · DAX · Power Query · Excel.

## Author
Darsh Choudhary - https://www.linkedin.com/in/darsh-choudhary-4a7563238/




