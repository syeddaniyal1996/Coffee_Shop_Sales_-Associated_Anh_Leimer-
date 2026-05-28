# Coffee_Shop_Sales_(Associated_Anh_Leimer)

A comprehensive, data-driven Power BI dashboard designed to analyze sales performance, understand shopper behavior, and model financial impacts across multiple retail coffee shop locations.

# Coffee Shop Sales Performance Dashboard

A comprehensive, data-driven Power BI dashboard designed to analyze sales performance, understand shopper behavior, and model financial impacts across multiple retail coffee shop locations. 

---

## 📊 Project Overview

This multi-page dashboard provides executive-level overviews and granular data breakdowns for three retail locations: **Lower Manhattan**, **Hell's Kitchen**, and **Astoria**. It tracks key performance indicators (KPIs), transaction volume, operational efficiency, and product price elasticity from January to June.

### 🚀 Key High-Level Metrics
* **Total Sales:** \$698,812 [cite: 3]
* **Total Quantity Sold:** 214,470 units [cite: 4]
* **Total Transactions:** 149,116 [cite: 25]

---

## 🗂️ Dashboard Structure & Features

### Page 1: Executive Overview & Product Analysis

The landing page establishes baseline performance and provides cross-filtering slicers for deep dives by store and product category[cite: 14, 16].

* **Balanced Regional Performance:**
* Retail revenue is evenly distributed across locations, with Hell's Kitchen leading at **33.84%**, followed by Astoria (**33.23%**) and Lower Manhattan (**32.92%**).
* **Core Revenue Drivers:** **Coffee** represents the highest grossing category at **\$269,952** (32% of total sales) [cite: 69, 70][cite_start], closely followed by **Tea** at **\$196,406** (31% of total sales).
* **Premium Unit Breakdown:** While *Coffee beans* and *Branded* items represent lower transaction volumes, they yield the highest margins with Average Prices Per Unit of **\$21.93** and **\$17.53** respectively.

<img width="1452" height="822" alt="01" src="https://github.com/user-attachments/assets/02209de7-fd1c-4271-99b0-6e2dca1f0761" />

### Page 2: Shopper Behavior & What-If Analysis
This section focuses on transactional trends and predictive revenue modeling.

* **Transaction KPIs:** Tracks core performance metrics including an **Average Order Value (AOV) of \$4.7** and an **Average Quantity Per Transaction of 1.44**. Both cards feature Month-over-Month (MoM) growth context indicators.
* **Dynamic Scenario Projections:** Includes a **Price Change Parameter (What-If Analysis)**. Setting a **+10.0% Price Change** dynamically projects adjusted sales curves across product categories (e.g., Bakery at \$82K, Coffee at \$270K) to preview future revenue trends.

<img width="1459" height="820" alt="02" src="https://github.com/user-attachments/assets/77a6842e-0851-4f0a-956f-cfa3650f4e59" />

### Page 3: Peak Operations & Granular Product Rankings
Designed for operational efficiency, this page maps performance down to the hour, week, and specific product SKU.

* **Sales Distribution Matrix:** A matrix visualization breaking down **Sales Distribution by Week and Day Name**. Data reveals sharp late-month momentum, with Week 4 tracking at **\$31,806** in revenue velocity.
* **Price Elasticity Scatter Plot:** A custom scatter chart tracking *How Unit Price Affects Transaction Qty*. A clear downward trendline validates standard economic elasticity—low-cost items (*Flavours*, *Tea*) drive massive volume, while premium tiers (*Coffee beans*) see low-frequency, targeted purchases.
* **Product Performance Extremes:**
  * **Top Grossing Product:** *Sustainably Grown Organic Large Hot Chocolate* (**\$21,152** total sales, **+31.2% MoM growth**).
  * **Lowest Grossing Product:** *Brazilian Organic Beans* (**\$3,852** total sales).

<img width="1454" height="820" alt="03" src="https://github.com/user-attachments/assets/12be1801-cede-4dc1-aa58-7c92fe845472" />

---

## 🛠️ Tech Stack & Key DAX Patterns

* **Business Intelligence Tool:** Power BI Desktop
* **Data Modeling:** Star schema architecture featuring localized fact tables linked to dedicated Date and Time dimensions.
* **Key DAX Functionality:**
  * **Time Intelligence:** Month-over-Month (MoM) growth calculations utilizing `CALCULATE`, `DATEADD`, and error-handling variables to verify performance momentum.
  * **What-If Parameters:** Leveraged `GENERATESERIES` and `SELECTEDVALUE` to allow end-users to dynamically adjust unit prices and watch revenue forecasts change in real time.
  * **Conditional Formatting:** UI/UX optimization using custom hex-code indicators for quick positive/negative variance scanning.
