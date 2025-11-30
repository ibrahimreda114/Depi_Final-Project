# 📦 End-to-End Supply Chain Analytics Project

## 📊 Project Overview
This project provides a comprehensive analysis of supply chain operations, tracking key performance indicators (KPIs) related to inventory management, shipping costs, supplier reliability, and product profitability. The primary goal is to establish a data-driven monitoring system to identify bottlenecks, optimize stock levels, and reduce operational costs and defect rates.

## 🎯 Business Objectives
* **Cost Reduction:** Analyze shipping and manufacturing costs to pinpoint areas for optimization and saving.
* **Supplier Evaluation:** Monitor defect rates and lead times to effectively assess supplier reliability and consistency.
* **Inventory Optimization:** Track stock levels per SKU to prevent both costly overstocking and disruptive stockouts.
* **Revenue Analysis:** Segment and understand revenue streams by product type and customer demographics for strategic growth.

## 🛠 Tools & Technology
* **Power BI Desktop:** Used for data visualization and the interactive dashboard creation.
* **Power Query (M Language):** Utilized for the ETL (Extract, Transform, Load) process, including data cleaning and normalization.
* **DAX (Data Analysis Expressions):** Used for creating complex, dynamic measures (e.g., Profit Margin, YoY Growth, Defect Rates).
* **Data Modeling:** Employed a **Star Schema** approach to transform the raw flat file into an efficient, relational model.

## 💾 Dataset Snapshot
The source data began as a single **Flat File** containing merged transactional and descriptive data. Key data points included:
* **Financial & Sales:** `Revenue generated`, `Total products sold`, `Costs`.
* **Product & Inventory:** `SKU`, `Product Type`, `Stock levels`, `Order quantities`, `Price`.
* **Logistics & Time:** `Shipping costs`, `Transportation Mode`, `Shipping carrier`, `Lead times`, `Manufacturing lead time`.
* **Quality & Suppliers:** `Supplier name`, `Defect rates`, `Inspection results` (Pass/Fail/Pending).
* **Customer:** `Customer demographics` (Female, Male, Non-binary, Unknown).

## 📈 Key Insights from Dashboard
* **Profitability:** Demonstrated Total Revenue of $577K with a strong Average Profit Margin of ~86%.
* **Quality Control:** Identified specific suppliers and product types contributing disproportionately to higher defect rates.
* **Logistics Efficiency:** Provided cost-vs-revenue analysis across different transportation modes (Air, Sea, Road, Rail) to optimize shipping strategy.

## 📂 Project Structure 🔗
Detailed documentation for this project is available in the following files:
* [⚙️ Data Preparation and Processing](Data_Preparation_and_Processing.md)
* [📊 Analytics and Dashboard Deep Dive](Analytics_and_Dashboard.md)
