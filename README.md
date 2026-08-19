# 📊 Sales & Customer Performance Dashboard – Tableau

*Analyzing sales, profitability, customer behavior, order trends, and product performance using Tableau to generate actionable business insights.*

---

## 📌 Table of Contents

- <a href="#overview">Overview</a>
- <a href="#business-problem">Business Problem</a>
- <a href="#dataset">Dataset</a>
- <a href="#tools--technologies">Tools & Technologies</a>
- <a href="#project-structure">Project Structure</a>
- <a href="#data-cleaning--preparation">Data Preparation</a>
- <a href="#research-questions--key-findings">Research Questions & Key Findings</a>
- <a href="#dashboard">Dashboard</a>
- <a href="#how-to-run-this-project">How to Run This Project</a>
- <a href="#author--contact">Author & Contact</a>

---

<h2><a class="anchor" id="overview"></a>Overview</h2>

This project presents an **Interactive Sales & Customer Performance Dashboard built using Tableau**.

The dashboard analyzes business performance for **2020-23 compared with the previous years** across sales, profit, quantity, customers, orders, products, sub-categories, and customer purchasing behavior.
The project contains two major dashboard views:
- **Sales Dashboard** – Provides an overview of sales, profit, quantity, sub-category performance, and sales/profit trends.
- **Customer Dashboard** – Analyzes customer growth, sales per customer, order volume, customer order distribution, and top-performing customers.
- **Interactive filters** allow users to analyze performance by **Year, Category, Sub-Category, Region, State, and City**.

---

<h2><a class="anchor" id="business-problem"></a>Business Problem</h2>

Businesses need to continuously monitor sales and customer performance to identify growth opportunities, profitable products, and areas requiring improvement.This project aims to answer questions such as:

- How did sales and profit perform compared with the previous year?
- Which products and sub-categories generate the highest sales?
- Which sub-categories generate losses?
- How are sales and profit changing over time?
- How many customers and orders were generated?
- What is the average sales generated per customer?
- Which customers contribute the most to overall sales and profit?
- How frequently do customers place orders?
- Which regions and locations require further investigation?

---

<h2><a class="anchor" id="dataset"></a>Dataset</h2>

- Multiple CSV files located in the `/Database/` folder. (**Customer, Location, Orders, Products**)
**Orders** acts as the primary transactional table and is connected with **Customers, Location, and Products tables**.
---

<h2><a class="anchor" id="tools--technologies"></a>Tools & Technologies</h2>

- Tableau (Interactive Visualizations)
- Excel (Data Cleaning)
- Github

---

<h2><a class="anchor" id="project-structure"></a>Project Structure</h2>

```text
sales-customer-dashboard/
│
├── README.md
│
├── Database/
│   ├── Customers.csv
│   ├── Location.csv
│   ├── Orders.csv
│   └── Products.csv
│
├── Images/
│   ├── Icon - Customer Dashboard (active).png
│   ├── Icon - Customer Dashboard.png
│   ├── Icon - Filter Hidden.png
│   ├── Icon - Filter Shown.png
│   ├── Icon - Logo.png
│   ├── Icon - Sales Dashboard.png
│   └── Icon - Sales Dashboard(active).png
|
├── README.md
└── sales-dashboard-project.twbx
```

---

<h2><a class="anchor" id="data-cleaning--preparation"></a>Data Preparation</h2>

The dataset was prepared for Tableau analysis by:

- Checking the available sales and customer fields
- Ensuring appropriate data types for dates, numerical fields, and categorical dimensions
- Using order and customer information to create customer-level metrics
- Aggregating sales, profit, quantity, and order metrics
- Creating year-over-year performance comparisons
- Creating calculated fields for KPI growth percentages
- Preparing monthly sales and profit trends
- Creating sub-category level sales and profit comparisons
- Creating customer ranking and order-frequency analysis

---

## Research Questions & Key Findings

### 1. Is overall business performance improving?

Yes. 2023 shows positive year-over-year growth across the primary sales KPIs:

- Sales increased by **20.4%**
- Profit increased by **14.2%**
- Quantity increased by **26.8%**

However, the lower profit growth compared with sales growth suggests that revenue growth should also be evaluated alongside margins and product-level profitability.

### 2. Is the customer base growing?

The total customer count increased by **8.6%**, reaching **693 customers** in 2023.

At the same time, sales per customer increased by **10.8%**, indicating that the business generated more revenue per customer on average.

### 3. Are order volumes increasing?

Yes. Total orders increased by **28.3%**, reaching **1,687 orders**.

The growth in orders is considerably higher than customer growth, indicating increased purchasing activity among existing customers.

### 4. Which sub-categories require attention?

The sub-category profitability visualization identifies several areas where the business generated losses.

Loss-making categories visible in the dashboard include:

- Tables
- Machines
- Envelopes
- Fasteners

These categories should be investigated further for pricing, discounting, procurement costs, and product-level profitability.

### 5. Which customers are high-value?

The Customer Dashboard provides a ranked **Top 10 Customers** table based on customer performance.

The top-ranked customer in the dashboard is **Raymond Buch**, followed by customers such as Hunter Lopez and Tom Ashbrook.

The table provides:

- Customer name
- Last order date
- 2023 profit
- 2023 sales
- Number of orders

This makes it possible to identify customers who contribute significantly to revenue and profitability.

---

## Dashboard

### 📊 Sales Dashboard

![Sales Dashboard](screenshots/sales-dashboard.png)

The Sales Dashboard provides:

- Total Sales KPI
- Total Profit KPI
- Total Quantity KPI
- Monthly sales trend
- Monthly profit trend
- Sales comparison by sub-category
- Profit/loss by sub-category
- Average sales benchmark
- Average profit benchmark
- Year-over-year comparison

---

### 👥 Customer Dashboard

![Customer Dashboard](screenshots/customer-dashboard.png)

The Customer Dashboard provides:

- Total Customers
- Sales per Customer
- Total Orders
- Monthly customer trends
- Monthly sales/customer trends
- Monthly order trends
- Customer order-frequency distribution
- Top 10 Customers
- Customer sales and profit performance

---

### 🔎 Interactive Filters

![Customer Dashboard Filters](screenshots/customer-dashboard-filters.png)

The dashboard includes interactive filters for:

- **Year**
- **Category**
- **Sub-Category**
- **Region**
- **State**
- **City**

These filters allow users to drill down from overall business performance into specific products and geographic locations.

---

## Dashboard Features

### KPI Cards

High-level KPI cards provide an immediate overview of business performance and year-over-year growth.

### Monthly Trend Analysis

Line charts compare 2023 performance with the previous year and highlight:

- Highest-performing month
- Lowest-performing month
- Monthly sales movement
- Monthly profit movement

### Sub-Category Analysis

The dashboard compares sales and profitability across product sub-categories to identify:

- High-sales products
- High-profit products
- Loss-making products
- Areas requiring optimization

### Customer Analysis

The Customer Dashboard provides insight into:

- Customer growth
- Customer value
- Order frequency
- Top customers
- Customer sales
- Customer profitability

### Interactive Filtering

Users can dynamically filter the dashboard by time, product category, and geographic location to perform detailed analysis.

---

## How to Run This Project

### 1. Clone the repository

```bash
git clone https://github.com/yourusername/sales-customer-dashboard-tableau.git
```

### 2. Navigate to the project directory

```bash
cd sales-customer-dashboard-tableau
```

### 3. Open the Tableau workbook

Open:

```text
dashboard/sales_customer_dashboard.twbx
```

using **Tableau Desktop** or a compatible Tableau environment.

### 4. Connect the dataset

If the workbook uses an external CSV/Excel data source, update the data connection path to:

```text
data/sales_data.csv
```

### 5. Explore the dashboards

Use the available filters to analyze performance by:

- Year
- Category
- Sub-Category
- Region
- State
- City

---

## Business Recommendations

Based on the dashboard analysis:

- **Focus on profitable sub-categories** while maintaining strong sales growth.
- **Investigate loss-making sub-categories** such as Tables, Machines, Envelopes, and Fasteners.
- **Improve customer retention** by converting one-time customers into repeat buyers.
- **Develop targeted strategies for high-value customers** based on their sales and profit contribution.
- **Analyze periods of high sales but relatively lower profit** to identify discounting or cost-related issues.
- **Use geographic filtering** to identify high-performing and underperforming regions and cities.
- **Monitor monthly trends** to optimize inventory, promotions, and sales strategies during high-demand periods.

---

## Author & Contact

**Anubrata Guchhait**  
Data Analyst | B.Sc. Mathematics Graduate

📧 Email: `your-email@example.com`  
🔗 LinkedIn: `https://www.linkedin.com/in/your-profile/`  
🔗 GitHub: `https://github.com/yourusername`

---

⭐ **If you found this project useful, consider giving the repository a star!**