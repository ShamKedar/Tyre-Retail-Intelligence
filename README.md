# 🚗 Tyre Retail Intelligence

**MySQL | Power BI | DAX | SQL | Google Colab | Python**

An end-to-end retail analytics project focused on analyzing **sales performance, product demand, pricing, returns, inventory levels, supplier lead times, and replenishment risk** for a tyre retailer.

The project uses two years of transaction data from **April 2024 to March 2026** and combines sales, current inventory, and supplier information to answer practical business questions and support data-driven decisions.

---

## 📌 Project Overview

A tyre retailer needs to understand:

* Which products and brands generate the most revenue?
* Which products are selling the fastest?
* Which products may be overstocked or at risk of stockout?
* ...

This project addresses these questions using **MySQL for data analysis and Power BI for interactive business reporting**.

> **Note:** The dataset is derived from a real tyre retailer's transaction records. Brands, suppliers, and product identifiers have been anonymised, and monetary values have been scaled by a constant factor. Therefore, the absolute monetary values should not be interpreted as actual market prices or revenue. Relative patterns, demand behaviour, seasonality, and price relationships are preserved.

---

# 🎯 Business Objectives

The main objectives of this project are to:

- Analyse overall sales and revenue performance.
- Identify high-performing brands and products.
- Analyse pricing and price-tier performance.
- Understand product return patterns.
- Evaluate current inventory levels.
- Identify potentially overstocked and low-stock products.
- Analyse supplier lead-time performance.
- Identify brands that may face stockout risk before replenishment.
- Prioritise brands for inventory replenishment.
- Build an interactive Power BI dashboard for business decision-making.

---

# 📊 Dataset

* [About Dataset]()
* Original Dataset is available on kaggle [Tyre Retail Sales & Inventory Dataset (2024–2026)](https://www.kaggle.com/datasets/samauto/tyre-retail-sales-and-inventory-dataset-20242026?select=DS+Data+Set+-+Current+Stock.csv)

---

# 🛠️ Tools & Technologies

| Tool         | Purpose                                                                |
| ------------ | ---------------------------------------------------------------------- |
| **MySQL**    | Data querying, transformation and business analysis                    |
| **SQL**      | Aggregation, joins, CTEs, window functions and analytical calculations |
| **Power BI** | Interactive dashboards and data visualization                          |
| **DAX**      | Dynamic business measures and KPIs                                     |
| **GitHub**   | Project documentation and version control                              |
| **Python**   | Data cleaning and structural analysis.                                 |
| **Notion**   | Project task management and planning.                                  |

---

# 📈 Power BI Dashboard

The Power BI report is divided into four pages.

## Page 1 — Executive Overview

![Page 1]()

### Purpose

Provides management with a high-level overview of overall retail performance.

---

# Page 2 — Sales & Product Performance

![Page 2]()

### Purpose

Identifies the products, brands, and pricing segments driving sales performance.

---

# Page 3 — Inventory Analysis

![Page 3]()

### Purpose

Identifies products where inventory levels may not align with demand.

---

# Page 4 — Supplier & Inventory Risk

![Page 4]()

### Purpose

Combines sales demand, inventory levels, and supplier lead-time information to identify potential replenishment risks.

---

# 🔍 Analytical Assumptions

Some inventory classifications in this project are **analytical assumptions rather than values explicitly provided by the dataset**.

For example:

```text
Days of Inventory < 50     → Critical
< 70 days                  → Low
< 90 days                  → Healthy
```

Similarly, replenishment-risk thresholds are defined for analytical purposes.

These thresholds should be reviewed and adjusted according to actual business policies if real operational data becomes available.

The project therefore presents these classifications as **analytical indicators**, not official inventory policies.

---

# 📁 Project Structure

```text
Tyre-Retail-Analytics/
├── 📁 dashboards
│   ├── 📁 power-bi dashboard
│   │   ├── 📄 DAX Measures
│   │   └── 📄 Tyre Retail Intelligence Dashboard.pbix
│   ├── 📁 screenshots of dashboard
│   │   ├── 🖼️ Page_1.png
│   │   ├── 🖼️ Page_2.png
│   │   ├── 🖼️ Page_3.png
│   │   ├── 🖼️ Page_4.png
│   │   └── 📕 SS of Tyre Retail Intelligence Dashboard.pdf
│   └── 📄 Data Terms Used
├── 📁 data
│   ├── 📄 About Dataset
│   ├── 📄 current_stocks.csv
│   ├── 📄 sales.csv
│   └── 📄 supplier.csv
├── 📁 sql
│   ├── 📄 business questions list
│   └── 📄 sql_15_business_questions
├── 📄 Cleaning_Tyre_Retail_Dataset.ipynb
├── 📄 Insights
└── 📝 README.md
```

---

# 🎯 Key Learning Outcomes

Through this project, I practiced:

* Designing SQL queries around business requirements.
* Joining multiple relational tables.
* Working with sales and return transactions.
* Using CTEs and window functions.
* Performing time-based sales analysis.
* Developing inventory metrics.
* Understanding lead-time and replenishment concepts.
* Creating DAX measures.
* Building an interactive Power BI dashboard.
* Communicating analytical findings as business recommendations.

---

# 📌 Conclusion

**Tyre Retail Intelligence** demonstrates an end-to-end data analytics workflow using Colab, MySQL and Power BI.

Rather than focusing only on individual SQL queries or visualizations, the project follows a business-oriented approach:

> **Business Question → Data → Data Cleaning → SQL Analysis → Metrics → Power BI → Insights → Recommendations**

The goal is to demonstrate how retail transaction, inventory, and supplier data can be transformed into actionable information for **sales performance, inventory management, and replenishment decision-making**.

---

## 👤 Author

**Sham Kedar**

**Data Analyst**

This project is part of my data analytics portfolio, demonstrating practical Pandas, SQL, Power BI and business analysis skills.
