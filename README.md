# Executive Sales Dashboard 📊

An interactive Tableau dashboard designed to track, analyze, and present key sales performance indicators, profitability metrics, and regional distributions.

---

## 🖼️ Dashboard Preview
![Executive Sales Dashboard Preview](dashboard_preview.png)

---

## 📈 Dashboard Overview
This executive-facing dashboard provides an end-to-end breakdown of sales figures, production costs, and overall profit margins. It enables stakeholders to quickly monitor fiscal performance across different periods, products, and geographical regions.

### Key Metrics Tracked:
*   **Sum of Sales:** \$29,358,677
*   **Sum of Production Cost:** \$17,277,794
*   **Sum of Profit:** \$12,080,884

---

## 🔍 Visual Components & Insights

### 1. High-Level KPI Cards
*   Provides immediate visibility into total Sales, Production Costs, and Net Profit.

### 2. Performance Breakdown
*   **Top Products & Customers:** Identifies high-value inventory items and driving customer accounts ranked by calculated sales amounts.
*   **Top Regions in Sales:** A geographic map tracking global distribution, highlighting the highest-performing markets (e.g., North America leading with \$9.38M).

### 3. Time-Series Trends
*   **Year-wise Sales Performance:** Side-by-side annual sales comparisons highlighting growth trajectories.
*   **Monthly Sales Trends:** A seasonal line chart illustrating performance fluctuations across monthly cycles.
*   **Quarterly Sales Share:** A clean breakdown showing proportional distribution across fiscal quarters (Q1–Q4).

---

## 🛠️ Tools & Technologies Used
*   **Tableau Public / Desktop:** Dashboard design, calculated fields, and interactive visualization.
*   **Data Source:** Integrated transactional sales tables (`Fact_InternetSales`).


---

### 💛 Power BI Executive Dashboard

![Power BI Dashboard Preview](Power%20BI%20Executive%20Dashboard.png)







---

## 📂 Project Structure
*   📁 `Executive_Sales_Dashboard.twbx` — The complete Tableau packaged workbook file containing worksheets and data extracts.
*   📁 `dashboard_preview.png` — Visual screenshot preview of the active dashboard layout.

---

### 🟢 Microsoft Excel Data Pipeline & Analysis
* **Data Prep Asset:** `[View Excel Binary Dataset](./Executive_Sales_Data.xlsb)`
* **Key Focus:** Data warehousing prep, business logic modeling, KPI baseline definitions, and source data cleaning.

![Excel Dashboard Preview](Excel_Executive_Sales_Dashboard.png)

---

## 🗄️ MySQL Database Analysis & Business Intelligence
* **Source Script File:** `[View Full Analytics Script](./AdventureWorks_Sales_Analysis.sql)`
* **Database System:** MySQL Workbench
* **Key Skills Demonstrated:** Data formatting (`CONCAT`, `ROUND`), margin analysis, corporate data metrics calculations.

### 🔍 Featured Business Query: Bottom-Line Profitability
> This query calculates absolute values for Total Revenue, Total Product Cost, and Net Profit Margin, converting large numbers dynamically into localized formatting (Lakhs) for executive financial tracking.

```sql
-- Section: Bottom-Line Profitability & Margin Realization
SELECT
    CONCAT(ROUND(SUM(SalesAmount) / 100000, 2), ' Lakhs') AS Total_Revenue,
    CONCAT(ROUND(SUM(TotalProductCost) / 100000, 2), ' Lakhs') AS Total_Cost,
    CONCAT(ROUND((SUM(SalesAmount) - SUM(TotalProductCost)) / 100000, 2), ' Lakhs') AS Total_Profit
FROM fact_sales_combined;
```

---
---

---

## 💼 Executive Slide Deck Presentation

* **Direct Presentation Link:** [Open Executive Presentation PDF](./Executive_Sales_Presentation.pdf)
* **Key Insights Delivered:** Strategic regional expansion plans, margin optimization recommendations, and operational bottleneck tracking delivered directly to stakeholders.


