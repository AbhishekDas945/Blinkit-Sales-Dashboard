# 🛒 Blinkit Sales Performance Analysis — Power BI Dashboard

![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![Power Query](https://img.shields.io/badge/Power%20Query-Data%20Transformation-217346?style=for-the-badge&logo=microsoftexcel&logoColor=white)
![DAX](https://img.shields.io/badge/DAX-Measures%20%26%20KPIs-0078D4?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Completed-success?style=for-the-badge)

## 📌 Project Overview
This repository contains an interactive **Blinkit Sales Performance Dashboard** built in **Microsoft Power BI**. Designed around Blinkit's brand identity (*"India's Last Minute App"*), the dashboard analyzes sales performance, customer ratings, product categories, and outlet distribution across Tier 1, Tier 2, and Tier 3 cities.

Using **Power Query** for data cleaning and transformation alongside **DAX** for dynamic KPI modeling, this project transforms raw retail transaction records into actionable insights for inventory planning and store expansion.

---

##  Dashboard Preview
> 💡 *Replace `dashboard_preview.png` below with the exact file path of your uploaded screenshot in the repository.*

![Blinkit Power BI Dashboard](dashboard_preview.png)

---

## 🎯 Key KPIs at a Glance
| Metric | Value | Description |
| :--- | :--- | :--- |
| **Total Sales** | **₹1.20M** | Overall revenue generated across all outlets and item categories |
| **Average Sales** | **₹140.99** | Mean revenue per transaction/item record |
| **No. of Items** | **9K (8,523)** | Total distinct product entries analyzed across all stores |
| **Average Rating** | **3.92 / 5.0** | Overall customer satisfaction rating across outlets |

---

## 🛠️ Tools & Technical Implementation
* **Power Query (ETL & Data Cleaning):**
  * Standardized inconsistent categorical values in the **Fat Content** column (e.g., unifying `LF`, `low fat` → `Low Fat` and `reg` → `Regular`).
  * Verified data types across numerical, currency, date/year, and text columns.
  * Handled missing values and removed redundant attributes to optimize data model performance.
* **DAX (Data Analysis Expressions):**
  * Created core aggregation measures: `Total Sales`, `Average Sales`, `Number of Items`, and `Average Rating`.
  * Configured **Field Parameters / Dynamic Metric Switching** allowing users to toggle the entire dashboard view between *Total Sales*, *Average Sales*, *Number of Items*, and *Average Rating* with a single click.
* **Interactive UI/UX Design:**
  * **Left Filter Panel:** Dedicated slicers for **Outlet Location Type**, **Outlet Size**, and **Item Type** for granular drill-downs.
  * **Conditional Formatting:** Applied custom color-coded data bars and background fills on the bottom-right Outlet Type matrix to compare 5 metrics simultaneously.

---

##  Key Business Insights

### 1. Consumer Preference by Fat Content
* **Low Fat** items dominate customer demand, contributing **₹776.32K (64.6%)** of total sales compared to **₹425.36K (35.4%)** for **Regular** items.
* Across every city tier, Low Fat products consistently outsell Regular items:
  * **Tier 3:** ₹0.31M (Low Fat) vs. ₹0.17M (Regular)
  * **Tier 2:** ₹0.25M (Low Fat) vs. ₹0.14M (Regular)
  * **Tier 1:** ₹0.22M (Low Fat) vs. ₹0.12M (Regular)

### 2. Top & Bottom Performing Item Categories
* **Top Revenue Drivers:** **Fruits and Vegetables (₹178.12K)** and **Snack Foods (₹175.43K)** are the two flagship categories, followed by **Household (₹135.98K)**, **Frozen Foods (₹118.56K)**, and **Dairy (₹101.28K)**.
* **Lowest Revenue Categories:** **Seafood (₹9.08K)**, **Breakfast (₹15.60K)**, and **Starchy Foods (₹21.88K)** generate the lowest sales volumes.

### 3. Outlet Establishment Trend (2011–2022)
* Outlets established in **2018** achieved the highest sales peak at **₹204.52K**.
* Establishments from **2012 to 2017** maintained a stable revenue band between **₹130.48K and ₹133.10K**, while post-2020 outlets stabilized at **₹131.48K** in 2022.

### 4. Store Size & Regional Tier Performance
* **By Outlet Size:** **Medium-sized outlets** generate the largest revenue share at **₹507.9K (42.27%)**, followed by **Small outlets at ₹444.8K (37.01%)** and **High-sized outlets at ₹249.0K (20.72%)**.
* **By Location Tier:** **Tier 3 cities** lead overall revenue with **₹472.13K**, outperforming **Tier 2 (₹393.15K)** and **Tier 1 (₹336.40K)**.

### 5. Outlet Type Breakdown
| Outlet Type | Total Sales | Average Sales | Number of Items | Average Rating | Item Visibility |
| :--- | :---: | :---: | :---: | :---: | :---: |
| **Supermarket Type1** | ₹787.55K | ₹141.21 | 5,577 | 3.92 | 6.07% |
| **Grocery Store** | ₹151.94K | ₹140.29 | 1,083 | 3.93 | 10.49% |
| **Supermarket Type2** | ₹131.48K | ₹141.68 | 928 | 3.93 | 6.10% |
| **Supermarket Type3** | ₹130.71K | ₹139.80 | 935 | 3.91 | 5.86% |

* **Supermarket Type1** is the primary revenue engine, accounting for over **65%** of total sales and SKU volume (5,577 items).
* **Grocery Stores** command the highest average **Item Visibility (10.49%)** and tie with Supermarket Type2 for the highest **Average Rating (3.93)**.
