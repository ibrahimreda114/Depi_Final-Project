# ⚙️ Data Preparation & Processing

## 1️⃣ Data Source & Initial State
The project started with a single **Flat File** that contained all transactional and descriptive data in one table. This structure suffered from high **data redundancy** (e.g., repeating product names, supplier names, and demographics for every transaction), which negatively affects query performance and model scalability.

## 2️⃣ Power Query (ETL - Transformation)
The core of the preparation involved normalizing the data by splitting the flat file into specialized tables using Power Query:

* **Normalization:** Identified descriptive columns (Dimensions) and separated them from the measurement columns (Facts).
* **Data Types:** Ensured correct data types (e.g., converting text-based columns like 'Shipping Costs' and 'Defect rates' to Decimal/Currency).
* **Cleaning & Filtering:** Addressed **implicit nulls** and removed any rows where core identifiers were missing.
* **Feature Engineering:** Created a custom column based on the `Inspection results` to categorize defect status as 'Pass', 'Fail', or 'Pending' for clear filtering in the dashboard.

## 3️⃣ Data Modeling (Star Schema)
The data was modeled using the **Star Schema** methodology to ensure optimal performance, simplified DAX calculations, and easy navigation. 

### 🔹 Fact Table (Fact_Transactions)
The central table containing the metrics and foreign keys:
* **Metrics:** `Revenue generated`, `Costs`, `Total products sold`, `Order quantities`, `Defect rates`.
* **Keys:** Keys linking to Dim_Product, Dim_Supplier, Dim_Customer, and Dim_Shipping.

### 🔹 Dimension Tables (Dimensions)
Descriptive tables used for slicing and filtering the Fact table:
* **Dim_Products:** Derived from `SKU`, `Product Type`, and `Price`.
* **Dim_Suppliers:** Derived from `Supplier name`, `Manufacturing lead time`, and `Location`.
* **Dim_Shipping:** Derived from `Shipping carrier`, `Transportation Mode`, and `Shipping costs`.
* **Dim_Customers:** Derived from `Customer demographics`.

## 4️⃣ DAX Measures
Several measures were created to calculate key financial and performance indicators used across the report:
* **Profit Margin %:** Calculates the percentage profit on sales.
    $$\text{Profit Margin} = \frac{\text{Total Revenue} - \text{Total Costs}}{\text{Total Revenue}}$$
* **Defect Rate %:** Calculated as the average defect rate weighted by volume.
* **Availability %:** Measures the percentage of available inventory against total stock.

---

## Data Model (Star Schema Diagram)
To illustrate the relationships and connections between the tables:

![Diagram showing the Star Schema Data Model with Fact and Dimension tables connected by primary and foreign keys.](https://github.com/ibrahimreda114/Depi_Final-Project/blob/main/images/Data%20model.png)

