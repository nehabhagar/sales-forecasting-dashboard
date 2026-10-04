# Executive Sales Performance & Demand Forecasting Dashboard

An end-to-end commercial business intelligence project built with **Power BI**, **DAX**, and **Advanced Excel** to model sales velocity, profit margins, and seasonal demand trends across product lines and geographic markets.

![Executive Sales Dashboard Overview](dashboard_overview.png)

---

## 📌 Business Problem & Overview
Sales and operations teams require real-time visibility into revenue run-rates, category profitability, and regional shipment demand to optimize inventory staging and dispatch workflows. 

This project delivers an executive-level performance tracking and forecasting dashboard that replaces static spreadsheets with dynamic time-intelligence modeling.

---

## 🎯 Key Findings & Strategic Impact
- **Regional Sales Skew:** Isolated key regional clusters contributing to over 60% of total revenue, guiding targeted warehouse staging and regional fulfillment priority.
- **Margin-Eroding Product Lines:** Identified low-margin, high-discount subcategories where promotional spend failed to generate positive margin lift.
- **Seasonal Demand Peaks:** Mapped cyclical quarterly spikes to assist operations in buffer planning and fulfillment staffing ahead of high-volume periods.

---

## 📈 Time-Series Demand Forecasting Analysis

![Demand Forecasting View](demand_forecasting.png)

- Modeled cyclical sales peaks across quarterly cycles to project fulfillment staffing and buffer inventory requirements.
- Highlighted variance between projected demand versus actual monthly order velocity.

---

## 🛠️ Technical Stack & Modeling
- **Business Intelligence:** Microsoft Power BI Desktop
- **Data Modeling:** Normalized Star Schema (Fact Sales linked with Dim Date, Dim Product, Dim Customer, Dim Region)
- **Calculations & DAX:** Custom time-intelligence and margin measures:
  - `Sales YTD` = `TOTALYTD(SUM(Sales[Revenue]), 'DimDate'[Date])`
  - `YoY Sales Growth %` = `DIVIDE([Sales YTD] - [Sales Prior Year], [Sales Prior Year], 0)`
  - `Gross Margin %` = `DIVIDE([Total Profit], [Total Revenue], 0)`
  - `Rolling 3-Month Sales Average`
- **Data Preparation:** Power Query for ETL, schema standardization, and data type validation.

---

## 🚀 How to Run & Explore
1. Clone or download this repository.
2. Open the `.pbix` file in **Power BI Desktop**.
3. Use the dynamic slicers (Year, Quarter, Category, Region) to test scenario filters and drill down into sub-tier metrics.
## 🚀 How to Run & Explore
1. Clone or download this repository.
2. Open the `.pbix` file in **Power BI Desktop**.
3. Use the dynamic slicers (Year, Quarter, Category, Region) to test scenario filters and drill down into sub-tier metrics.
