# Coffee_Shop_Sales_(Associated_Anh_Leimer)

A comprehensive, data-driven Power BI dashboard designed to analyze sales performance, understand shopper behavior, and model financial impacts across multiple retail coffee shop locations.

# Coffee Shop Sales Performance Dashboard

A comprehensive, data-driven Power BI dashboard designed to analyze sales performance, understand shopper behavior, and model financial impacts across multiple retail coffee shop locations. 

---

## 📊 Project Overview

This multi-page dashboard provides executive-level overviews and granular data breakdowns for three retail locations: **Lower Manhattan**, **Hell's Kitchen**, and **Astoria**. It tracks key performance indicators (KPIs), transaction volume, operational efficiency, and product price elasticity from January to June.

### 🚀 Key High-Level Metrics
* [cite_start]**Total Sales:** \$698,812 [cite: 3]
* [cite_start]**Total Quantity Sold:** 214,470 units [cite: 4]
* [cite_start]**Total Transactions:** 149,116 [cite: 25]

---

## 🗂️ Dashboard Structure & Features

### Page 1: Executive Overview & Product Analysis
[cite_start]The landing page establishes baseline performance and provides cross-filtering slicers for deep dives by store and product category[cite: 14, 16].

* [cite_start]**Balanced Regional Performance:** Retail revenue is evenly distributed across locations, with Hell's Kitchen leading at **33.84%**, followed by Astoria (**33.23%**) and Lower Manhattan (**32.92%**)[cite: 9, 12, 34].
* [cite_start]**Core Revenue Drivers:** **Coffee** represents the highest grossing category at **\$269,952** (32% of total sales) [cite: 69, 70][cite_start], closely followed by **Tea** at **\$196,406** (31% of total sales)[cite: 108, 109].
* [cite_start]**Premium Unit Breakdown:** While *Coffee beans* and *Branded* items represent lower transaction volumes, they yield the highest margins with Average Prices Per Unit of **\$21.93** [cite: 77, 78] [cite_start]and **\$17.53** respectively[cite: 65, 66].

### Page 2: Shopper Behavior & What-If Analysis
[cite_start]This section focuses on transactional trends and predictive revenue modeling[cite: 114, 121, 126, 143].

* [cite_start]**Transaction KPIs:** Tracks core performance metrics including an **Average Order Value (AOV) of \$4.7** [cite: 145] [cite_start]and an **Average Quantity Per Transaction of 1.44**[cite: 118]. [cite_start]Both cards feature Month-over-Month (MoM) growth context indicators[cite: 146, 148].
* [cite_start]**Dynamic Scenario Projections:** Includes a **Price Change Parameter (What-If Analysis)** slider[cite: 121]. [cite_start]Setting a **+10.0% Price Change** dynamically projects adjusted sales curves across product categories (e.g., Bakery at \$82K, Coffee at \$270K) to preview future revenue trends[cite: 126, 135].

### Page 3: Peak Operations & Granular Product Rankings
[cite_start]Designed for operational efficiency, this page maps performance down to the hour, week, and specific product SKU[cite: 178, 193, 204, 211].

* [cite_start]**Sales Distribution Matrix:** A matrix visualization breaking down **Sales Distribution by Week and Day Name**[cite: 193]. [cite_start]Data reveals sharp late-month momentum, with Week 4 tracking at **\$31,806** in revenue velocity[cite: 181].
* [cite_start]**Price Elasticity Scatter Plot:** A custom scatter chart tracking *How Unit Price Affects Transaction Qty*[cite: 179]. [cite_start]A clear downward trendline validates standard economic elasticity—low-cost items (*Flavours*, *Tea*) drive massive volume [cite: 199][cite_start], while premium tiers (*Coffee beans*) see low-frequency, targeted purchases[cite: 197].
* **Product Performance Extremes:**
  * [cite_start]**Top Grossing Product:** *Sustainably Grown Organic Large Hot Chocolate* (**\$21,152** total sales, **+31.2% MoM growth**)[cite: 205].
  * [cite_start]**Lowest Grossing Product:** *Brazilian Organic Beans* (**\$3,852** total sales)[cite: 213].

---

## 🛠️ Tech Stack & Key DAX Patterns

* **Business Intelligence Tool:** Power BI Desktop
* **Data Modeling:** Star schema architecture featuring localized fact tables linked to dedicated Date and Time dimensions.
* **Key DAX Functionality:**
  * **Time Intelligence:** Month-over-Month (MoM) growth calculations utilizing `CALCULATE`, `DATEADD`, and error-handling variables to verify performance momentum.
  * **What-If Parameters:** Leveraged `GENERATESERIES` and `SELECTEDVALUE` to allow end-users to dynamically adjust unit prices and watch revenue forecasts change in real time.
  * **Conditional Formatting:** UI/UX optimization using custom hex-code indicators for quick positive/negative variance scanning.

---

## 💡 Key Takeaway
By identifying peak transaction velocities, understanding price sensitivity curves, and monitoring margin health via dynamic parameter forecasting, this dashboard transforms raw transactional logs into strategic operational decisions for staff sizing, inventory control, and targeted menu promotions.

## 🤝 Contact & Feedback
Feel free to star this repository if you find the design layout or DAX implementations helpful! If you have any questions or want to discuss retail analytics optimizations, connect with me or open an issue.
