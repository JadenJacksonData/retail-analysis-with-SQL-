# Retail Sales SQL Analysis

## Project Overview

This project analyzes a retail sales dataset containing more than 20,000 transaction records using SQL and SQLite. The goal is to clean the data, evaluate sales and profitability, identify product and discount trends, and generate business insights that can support decision-making.

The project is being completed using **DB Browser for SQLite**.

---

## Dataset

* **Raw records:** 20,012
* **Clean records:** 20,000
* **Database:** SQLite
* **Tool:** DB Browser for SQLite
* **Primary analysis language:** SQL

The dataset contains retail transaction information including customer details, products, transaction dates, sales, costs, profits, quantities, discounts, payment methods, and geographic information.

---

# Data Quality & Cleaning

Before beginning the analysis, the dataset was evaluated for missing values, duplicate records, invalid quantities, negative sales amounts, and missing dates.

### Findings

* Identified **12 duplicate transaction records**
* Found **12 duplicated transaction IDs**
* Removed the 12 confirmed duplicate rows
* Final dataset contains **20,000 unique transactions**
* `customer_name`: 10 missing values
* `payment_method`: 10 missing values
* `state`: 10 missing values
* `product_name`: 0 missing values
* Transaction dates: 0 missing values
* Invalid quantities: 0
* Negative sales amounts: 0

### Data Cleaning Approach

Duplicate transaction IDs were investigated before removal. After confirming that the duplicated records were true duplicates, the extra records were removed while retaining one valid record for each transaction ID.

---

# Retail Sales Analysis

### Key Results

* **Total transactions:** 20,000
* **Total sales:** $3,081,718.11
* **Average sale:** $154.09
* **Maximum sale:** $1,149.95
* **Minimum sale:** $18.74
* **Net profit:** $1,330,123.61
* **Net profit margin:** 43.2%

### Monthly Performance

* **Highest sales volume:** January 2026 — 1,202 transactions
* **Highest monthly profit:** January 2026 — $186,914.11

January 2026 was the strongest month based on both transaction volume and total profit.

---

# Cost Analysis

* **Total cost:** $1,751,594.50
* **Average cost:** $87.58
* **Highest monthly cost:** July 2026 — $106,864.50
* **Lowest monthly cost:** February 2026 — $85,778.50

July represented approximately **6.1% of total costs**, while February represented approximately **4.8%**.

---

# Product Analysis

### Order Volume

* **Highest order volume:** Portable Charger — 961 orders
* **Lowest order volume:** Yoga Mat — 579 orders

### Profitability

* **Highest total profit:** Office Chair — $123,747.89
* **Lowest total profit:** Water Bottle — $15,740.26

An important finding is that the product with the highest number of orders was not the product generating the highest total profit. Portable Charger led in order volume, while Office Chair generated the most profit.

This demonstrates that **sales volume and profitability are not necessarily the same thing**.

---

# Discount Analysis

Average discount per order was calculated for each product to determine whether larger discounts were associated with higher order volumes.

### Findings

* Average discount per order ranged from approximately **$0.069 to $0.081**
* **T-Shirt** had the highest average discount per order at approximately **$0.081**
* **Desk Lamp** had the lowest average discount per order at approximately **$0.069**
* **Portable Charger** had the highest total discount amount at **$73.85**
* Portable Charger also had the highest order volume at **961 orders**
* Higher average discounts did not consistently correspond with higher order volume

### Business Insight

Discount size alone does not appear to explain differences in product demand. Other factors may influence product performance, including product type, customer preferences, pricing, and purchasing behavior.

---

# Business Insights So Far

The analysis has identified several preliminary findings:

1. The business generated more than **$3.08 million in sales** and approximately **$1.33 million in profit**.
2. The overall profit margin was approximately **43.2%**.
3. January 2026 was the strongest month for both transaction volume and monthly profit.
4. Portable Charger generated the highest number of orders, while Office Chair generated the highest total profit.
5. Higher order volume does not necessarily translate into higher total profit.
6. Discount levels were relatively consistent across products and did not consistently correspond with higher order volume.
7. The dataset required limited cleaning after removing 12 confirmed duplicate transactions.

---

# SQL Skills Demonstrated

* `SELECT`
* `COUNT()`
* `COUNT(DISTINCT)`
* `SUM()`
* `AVG()`
* `MIN()`
* `MAX()`
* `GROUP BY`
* `HAVING`
* `ORDER BY`
* `LIMIT`
* `WHERE`
* `IS NULL`
* `DELETE`
* SQLite `rowid`
* Date manipulation using `SUBSTR()`
* Number formatting using `printf()`
* Duplicate identification and removal
* Data-quality validation
* Business-focused SQL analysis

---

# Project Roadmap

The project is currently in the **exploratory analysis phase**.

### Completed

* [x] Import retail sales CSV
* [x] Verify dataset size
* [x] Perform data-quality checks
* [x] Identify duplicate transaction IDs
* [x] Remove confirmed duplicate records
* [x] Analyze overall sales
* [x] Analyze costs
* [x] Analyze product performance
* [x] Analyze discounts
* [x] Calculate profitability

### Coming Next

* [ ] Customer analysis
* [ ] Identify top 10 customers by revenue
* [ ] Analyze customer purchase frequency
* [ ] Calculate average customer spending
* [ ] State-level sales analysis
* [ ] State-level profit analysis
* [ ] Payment method analysis
* [ ] Monthly sales and profit trends
* [ ] Additional profitability analysis
* [ ] Identify business opportunities and risks
* [ ] Develop final recommendations
* [ ] Create final project conclusions
* [ ] Prepare SQL queries for GitHub
* [ ] Build polished GitHub README
* [ ] Create resume-ready project description
* [ ] Create LinkedIn project post

---

# Expected Final Deliverables

By the end of the project, the analysis will include:

* Cleaned SQLite database
* SQL analysis queries
* Data-quality documentation
* Sales and profitability analysis
* Product analysis
* Customer analysis
* Geographic analysis
* Discount analysis
* Business recommendations
* Final README
* GitHub portfolio project
* Resume-ready project entry
* LinkedIn-ready project summary

---

## Conclusion

This project demonstrates the use of SQL to transform a large retail transaction dataset into actionable business insights. The analysis began with data-quality validation and progressed into sales, cost, profitability, product, and discount analysis.

The next phase will focus on **customers, geography, payment methods, and deeper trends** to develop a more complete understanding of retail performance.

