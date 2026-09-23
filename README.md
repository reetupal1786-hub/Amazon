# 📊 Global E-Commerce Sales Pipeline & Analytics Portfolio

Welcome to my data analytics project repository. This project focuses on the comprehensive end-to-end data pipelines, exploratory analysis, and business intelligence reporting built strictly around a large-scale global e-commerce transactional dataset.

The underlying dataset tracks complex multidimensional order logs—including structured identifiers (`OrderID`, `CustomerID`, `ProductID`, `SellerID`), key timestamps (`OrderDate`), multi-currency financials, regional demographics, dynamic shipping mechanics, and live execution updates (`OrderStatus`).

---

## 🛠️ Data Analytics Tools & Architecture Breakdown

To extract business value, clean anomalies, and scale reporting metrics from this dataset, the following tools are deployed across the data lifecycle:

### 1. 🛢️ SQL & Relational Databases (Data Modeling, Querying & Schema Design)
* **Core Application:** SQL is used as the foundational tier to ingest, aggregate, and structure raw multi-channel logs into data marts.
* **Key Implementations:**
  * **Dynamic Partitioning:** Segmenting records by global geographics (`Country`, `State`, `City`) to profile cluster variance.
  * **Financial Metrics Engineering:** Writing mathematical aggregation strings to calculate exact Net Revenue on the fly:  
    `Net Revenue = (Quantity * UnitPrice) - Discount + Tax + ShippingCost`
  * **Window Functions:** Leveraging functions like `DENSE_RANK() OVER (PARTITION BY Category ORDER BY Quantity DESC)` to uncover product demand and isolate velocity metrics for high-volume items like *Drone Mini, Microphones, and 4K Monitors*.
  * **Logistical Isolation:** Querying granular tracking vectors via categorical logical breaks (`OrderStatus = 'Delivered'`, `'Shipped'`, `'Pending'`, `'Cancelled'`, or `'Returned'`).

### 2. 🐍 Python (Exploratory Data Analysis, Cleaning & Anomaly Detection)
* **Primary Frameworks:** Pandas, NumPy, Matplotlib, Seaborn
* **Core Application:** Deployed inside computational notebooks to implement automatic Extract-Transform-Load (ETL) flows and clean data format discrepancies.
* **Key Implementations:**
  * **Dtype Standardization & Parsing:** Converting unstructured strings into absolute datetimes (`OrderDate`) to compute time-series velocity and month-over-month sales trends.
  * **Transactional Profiling:** Utilizing **Pandas** to isolate payment channel preferences across dynamic execution groups—profiling consumer demand loops via *UPI, Debit Card, Amazon Pay, Credit Card, Cash on Delivery, and Net Banking*.
  * **Statistical EDA Graphs:** Deploying **Seaborn** distribution scatter matrices and correlation heatmaps to spot pricing anomalies, average unit discount trends, and systemic charge boundaries across different shipping lanes.

### 3. 📊 Power BI Desktop (Enterprise BI Dashboarding & Data Warehousing)
* **Architecture Models:** Power Query M-Engine, DAX Computations, Star Schema Relations
* **Core Application:** Transforming normalized transactional matrices into a highly responsive visual intelligence command center for stakeholders.
* **Key Implementations:**
  * **Star Schema Data Modeling:** Creating relationships between core transactional facts and disconnected dimension branches like consumer matrices, regional maps, and product logs.
  * **Time Intelligence DAX Infrastructure:** Developing complex custom metrics using **DAX** to measure global rolling sales averages and calculate loss ratios caused by order cancellation patterns.
  * **Interactive Cloud Visualization:** Creating high-level maps and product category matrices with dynamic slicers to evaluate cross-border performance (*India, United States, United Kingdom, Canada, Australia*).

### 4. 📈 Microsoft Excel (Spreadsheet Optimization & Matrix Prototyping)
* **Toolkit Deployed:** Pivot Cache Architecture, Dynamic Array Syntax, XLOOKUP Mapping
* **Core Application:** Deployed for targeted localized data testing, validation audits, and quick ad-hoc summaries.
* **Key Implementations:**
  * Building detailed dynamic tables to audit product pricing margins across separate supply chains.
  * Writing conditional lookups (`XLOOKUP`) to map product logs (`ProductID`) directly to supply routes, identifying pricing errors before loading data into major server systems.

---

## 📂 Structural Database File Architecture Schema
* **File System Type:** Structured Tabular Dimension Matrix
* **Primary Key Field:** `OrderID` (Unique Transaction Serial Sequence)
* **Foreign Dimension Relational Hooks:** `CustomerID`, `ProductID`, `SellerID`
* **Core Computational Variables:** `Quantity`, `UnitPrice`, `Discount`, `Tax`, `ShippingCost`
* **Descriptive Dimension Headers:** `Category`, `Brand`, `PaymentMethod`, `OrderStatus`, `City`, `State`, `Country`

---

## 📬 Contact & Analytics Connect
* **Location:** Noida, Uttar Pradesh, India
* **Email:** [reetu659544@gmail.com](mailto:reetu659544@gmail.com)
* **LinkedIn:** [://linkedin.com](https://linkedin.com)
* **GitHub:** [://github.com](https://github.com)
