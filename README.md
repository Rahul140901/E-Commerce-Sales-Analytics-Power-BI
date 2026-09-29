# 🛒 E-Commerce Sales Analytics — Power BI

An interactive **Power BI dashboard** designed to analyze e-commerce sales, customer behavior, product performance, and delivery operations using the **Brazilian Olist E-Commerce dataset**.

This project transforms raw transactional data into a **4-page analytical dashboard**, providing insights into revenue, orders, customers, product categories, repeat purchasing behavior, and delivery performance.

---

## 📊 Dashboard Preview

### 1. Executive Overview

![Executive Overview](Dashboard%20Images/Executive%20Overview.png)

Provides a high-level view of overall business performance, including revenue, orders, customers, product sales, delivery performance, and order status.

---

### 2. Customer Analysis

![Customer Analysis](Dashboard%20Images/Customer%20Analysis.png)

Analyzes customer acquisition, returning customers, repeat purchase behavior, geographic distribution, and customer segmentation.

---

### 3. Product & Category Analysis

![Product & Category](Dashboard%20Images/Product%20%26%20Category.png)

Examines product and category performance using revenue, order volume, pricing, freight costs, and category-level trends.

---

### 4. Delivery & Operations

![Delivery & Operations](Dashboard%20Images/Delivery%20%26%20Operations.png)

Analyzes order fulfillment and delivery performance, including delivery time, late deliveries, order status, and geographic operational performance.

---

## 📌 Project Overview

The objective of this project is to build an end-to-end **e-commerce analytics solution in Power BI** that converts raw Olist transactional data into meaningful business insights.

The dashboard is organized into four analytical areas:

- **Executive Overview** — overall business performance
- **Customer Analysis** — acquisition, retention, and customer behavior
- **Product & Category Analysis** — product and category performance
- **Delivery & Operations** — fulfillment and delivery efficiency

The report includes synchronized **Year** and **Month** filters, interactive visuals, cross-filtering, and page navigation for easier exploration.

---

## 🎯 Business Objectives

The analysis focuses on answering questions such as:

- How much revenue is being generated?
- How are orders and revenue changing over time?
- How many unique customers are purchasing?
- How many customers are new, returning, or repeat buyers?
- Which product categories generate the most revenue and orders?
- Which states and cities contribute the most customers and orders?
- What is the average delivery time?
- What percentage of deliveries arrive late?
- What percentage of orders are delivered or canceled?
- How does delivery performance vary geographically?

---

## 📈 Key KPIs

### Executive Overview

- Total Revenue
- Total Orders
- Total Customers
- Average Order Value
- Total Items Sold
- Average Rating
- Average Delivery Days
- Repeat Customer Rate
- On-Time Delivery %

### Customer Analysis

- Total Customers
- New Customers
- Returning Customers
- Repeat Customer Rate
- Orders per Customer

### Product & Category Analysis

- Total Revenue
- Total Products
- Total Categories
- Average Product Price
- Average Freight per Order

### Delivery & Operations

- Total Orders
- Average Delivery Days
- Late Delivery %
- Delivered Order %
- Canceled Order %

---

## 📊 Key Dashboard Metrics

For the complete dataset, the dashboard reports approximately:

| Metric | Value |
|---|---:|
| Total Revenue | R$13.59M |
| Total Orders | 99K |
| Total Customers | 96,096 |
| Total Items Sold | 113K |
| Average Order Value | R$137.75 |
| Average Delivery Days | 12.50 |
| Repeat Customer Rate | 3.12% |
| On-Time Delivery Rate | 91.89% |
| Total Products | 32,951 |
| Total Categories | 74 |
| Average Product Price | R$120.65 |
| Average Freight per Order | R$22.82 |

> Values may change depending on the Year and Month filters selected in the report.

---

## 🗂️ Dataset

This project uses the **Brazilian E-Commerce Public Dataset by Olist**.

The repository contains the following source files:

```text
olist_customers_dataset.csv
olist_geolocation_dataset.csv
olist_order_items_dataset.csv
olist_order_payments_dataset.csv
olist_order_reviews_dataset.csv
olist_orders_dataset.csv
olist_products_dataset.csv
olist_sellers_dataset.csv
product_category_name_translation.csv
```

These datasets contain information related to:

- Customers
- Orders
- Order items
- Products
- Sellers
- Payments
- Reviews
- Geographic locations
- Product category translations

---

## 🗺️ Geospatial Data

The project also includes:

```text
Brazil_States_Olist.geojson
```

This geographic file supports **Brazilian state-level map visualizations** used in the Power BI dashboard.

Geographic analysis is used to visualize metrics such as customer distribution, revenue, orders, and delivery performance across Brazilian states.

---

## 🧹 Data Preparation

Data preparation and transformation included:

- Handling missing and blank values
- Correcting data types
- Preparing date fields
- Creating a dedicated Date Table
- Translating product category names
- Establishing relationships between fact and dimension tables
- Creating calculated columns where required
- Preparing geographic fields for state-level analysis
- Creating customer-level analytical logic
- Building reusable DAX measures for KPIs and trends

---

## 🔗 Data Model

The Power BI model connects multiple Olist datasets to analyze the complete order lifecycle.

Major model relationships include:

```text
Customers
    ↓
Orders
    ↓
Order Items
   ↙     ↘
Products  Sellers

Orders
 ├── Payments
 ├── Reviews
 └── Date Table
```

Additional supporting tables are used for category translation, customer segmentation, geography, and state-level visualization.

---

## 🧮 Analysis & DAX

DAX measures were developed for business metrics including:

- Total Revenue
- Total Orders
- Total Customers
- Average Order Value
- Total Items Sold
- Average Delivery Days
- New Customers
- Returning Customers
- Repeat Customers
- Repeat Customer Rate
- Orders per Customer
- Previous-period comparisons
- Customer change indicators
- Delivered Orders
- Canceled Orders
- Delivered Order %
- Canceled Order %
- Late Delivery %
- On-Time Delivery %
- Average Product Price
- Average Freight per Order

Time-based measures use the Date Table to support dynamic analysis across **Year** and **Month**.

---

## 📑 Dashboard Pages

### 🏠 Executive Overview

Provides a consolidated view of business performance through:

- Revenue trend
- Top categories by revenue
- Revenue by customer state
- Order status distribution
- Business insight KPIs
- Year and Month filtering

### 👥 Customer Analysis

Focuses on customer behavior through:

- New vs Returning Customers Trend
- Top cities by customers
- Customers by state
- Customer segmentation
- Repeat Customer Rate
- Orders per Customer

### 📦 Product & Category Analysis

Analyzes merchandise performance through:

- Top categories by revenue
- Category revenue share
- Top categories by orders
- Category revenue trends
- Price vs order volume analysis
- Top category performance table

### 🚚 Delivery & Operations

Evaluates fulfillment performance through:

- Orders and Average Delivery Days Trend
- Order Status Distribution
- On-Time vs Late Delivery analysis
- Delivery Days by State
- Orders by State
- Top Cities by Orders
- State-level delivery performance

---

## 💡 Key Business Insights

The dashboard enables users to identify:

- Revenue and order trends across the available data period
- High-performing product categories
- Geographic concentration of customers and orders
- New and returning customer behavior
- Repeat purchasing patterns
- Average delivery performance
- Late-delivery patterns
- Order fulfillment and cancellation performance
- Differences in operational performance across Brazilian states

These insights can support decisions related to **sales strategy, customer retention, product planning, logistics, and operational performance**.

---

## 🛠️ Tools & Technologies

- **Power BI Desktop** — dashboard development and visualization
- **Power Query** — data cleaning and transformation
- **DAX** — calculated measures and analytical logic
- **CSV** — source datasets
- **GeoJSON** — Brazilian state geographic boundaries
- **Git & GitHub** — version control and project hosting

---

## 📁 Repository Structure

```text
E-Commerce-Sales-Analytics-Power-BI/
│
├── Dashboard Images/
│   ├── Executive Overview.png
│   ├── Customer Analysis.png
│   ├── Product & Category.png
│   └── Delivery & Operations.png
│
├── Dataset/
│   ├── olist_customers_dataset.csv
│   ├── olist_geolocation_dataset.csv
│   ├── olist_order_items_dataset.csv
│   ├── olist_order_payments_dataset.csv
│   ├── olist_order_reviews_dataset.csv
│   ├── olist_orders_dataset.csv
│   ├── olist_products_dataset.csv
│   ├── olist_sellers_dataset.csv
│   └── product_category_name_translation.csv
│
├── Brazil_States_Olist.geojson
├── E-Commerce Sales Analytics.pbix
├── .gitignore
└── README.md
```

---

## 🚀 How to Use the Project

1. Clone or download this repository.
2. Open `E-Commerce Sales Analytics.pbix` using **Power BI Desktop**.
3. Use the **Year** and **Month Name** slicers to explore different periods.
4. Navigate between the four dashboard pages using the report navigation.
5. Interact with charts, maps, categories, states, and cities to explore the data.

---

## 📅 Data Period

The dashboard analyzes Olist e-commerce data covering:

**2016 – 2018**

---

## 👤 Author

**Rahul Shewale**

Data Analyst | Power BI | SQL | Excel | Tableau

GitHub: **Rahul140901**

---

## ⭐ Project Purpose

This project was developed as a **Data Analytics portfolio project** to demonstrate practical skills in:

**Data Cleaning → Data Modeling → DAX → Business Analysis → Data Visualization → Dashboard Design → Business Insights**

If you find this project useful, consider giving the repository a ⭐.