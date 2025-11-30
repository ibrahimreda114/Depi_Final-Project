# 📦 Supply Chain Analytics Project

## 📊 Project Overview
This project involves analyzing supply chain data to track key performance indicators (KPIs) related to inventory management, shipping costs, supplier performance, and product profitability. The goal هو تحديد اختناقات سلسلة الإمداد (Supply Chain bottlenecks)، وتحسين مستويات المخزون، وتقليل معدلات العيوب.

## 🎯 Objectives
* **Cost Reduction:** Analyze shipping and manufacturing costs to identify saving opportunities.
* **Supplier Evaluation:** Monitor defect rates and lead times to assess supplier reliability.
* **Inventory Optimization:** Track stock levels per SKU to prevent overstocking or stockouts.
* **Revenue Analysis:** Understand revenue streams by product type and customer demographics.

## 🛠 Tools Used
* **Power BI Desktop:** For data visualization and dashboard creation.
* **Power Query:** For ETL (Extract, Transform, Load) processes and data cleaning.
* **DAX (Data Analysis Expressions):** For calculating measures (e.g., Profit Margin, Defect Rates).
* **Star Schema Modeling:** Transformed a single flat file into a structured Data Model.

## 💾 Dataset Snapshot (نظرة على البيانات)
The source data was initially provided as a single **Flat File** containing detailed transactional information. This file included the following key data points which were later split into a relational model:

* **Financial & Sales:** `Revenue generated`, `Total products sold`, `Costs`.
* **Product & Inventory:** `SKU`, `Product Type`, `Stock levels`, `Order quantities`, `Price`.
* **Logistics & Time:** `Shipping costs`, `Transportation Mode`, `Shipping carrier`, `Lead times`, `Manufacturing lead time`.
* **Quality & Suppliers:** `Supplier name`, `Defect rates`, `Inspection results` (Pass/Fail/Pending).
* **Customer:** `Customer demographics` (Female, Male, Non-binary, Unknown).

## 📈 Key Insights
* **Total Revenue:** $577K with a healthy Profit Margin of ~86%.
* **Defect Rates:** Identified specific suppliers with higher defect rates to improve quality control.
* **Shipping Modes:** Analyzed cost vs. revenue for different transportation modes (Air, Sea, Road, Rail).

## 📂 Project Structure 🔗
Here are the links to the detailed project documentation:
* [⚙️ Data Preparation and Processing](Data_Preparation_and_Processing.md)
* [📊 Analytics and Dashboard Deep Dive](Analytics_and_Dashboard.md)
