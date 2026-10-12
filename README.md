# 💊 Pharmaceutical Sales & Demand Control Tower (Power BI)

## 📌 Project Overview
An end-to-end business intelligence solution designed to analyze daily pharmaceutical sales, therapeutic categories, and long-term demand trends. This project provides deep insights into pharmacy operations, top-performing drug classifications, and year-over-year (YOY) growth metrics to support data-driven decision-making in healthcare retail.

---

## 🚀 Key Performance Indicators (KPIs) & Metrics
The dashboard tracks core commercial and operational metrics:
* **Total Quantity Sold:** Aggregate volume of pharmaceutical products dispensed.
* **Daily Average Quantity:** Average daily sales turnover.
* **Prior Year Quantity (PY):** Baseline metrics for historical comparison.
* **YOY Growth %:** Annual growth rate tracking performance across periods.

---

## 🗄️ Data Architecture & Modeling (Star Schema)
The data model was structured using a robust **Star Schema** to ensure high performance and accurate filtering:
* **`salesdaily` (Fact Table):** Contains transactional daily sales data linked by date and drug classification code.
* **`Dim_ATC` (Dimension Table):** Standardized drug classification based on ATC codes (Anatomical Therapeutic Chemical Classification System) mapped with descriptions.
* **`Dim_Date` (Dimension Table):** A dedicated calendar table enabling advanced **Time Intelligence** DAX calculations.

---

## 🛠️ DAX Measures Used
Core metrics were engineered using professional DAX calculations:
```dax
Total Quantity Sold = SUM(salesdaily[Quantity_Sold])
PY Quantity Sold = CALCULATE([Total Quantity Sold], SAMEPERIODLASTYEAR(Dim_Date[Date]))

---

📊 Dashboard Preview & Layout
​Executive Summary: High-level KPI cards tracking volume, growth, and trends.
​Category Performance: Clustered bar charts breaking down sales by therapeutic categories (e.g., Analgesics, Anti-inflammatories, Respiratory).
​Time Series Trend: Continuous temporal analysis tracking seasonal fluctuations over multi-year data.


---

​⚙️ Tools & Technologies
​Power BI Desktop: Data modeling, Power Query transformations, DAX modeling, and visualization design.
​GitHub & Git: Version control and professional portfolio documentation.

---

## 🛡️ License

This project is licensed under the MIT License. You are free to use, modify, and share this project with proper attribution.

## 🌟 About Me

Hi there! I'm Ahmed Alnaggar. I'm a data analyst.



