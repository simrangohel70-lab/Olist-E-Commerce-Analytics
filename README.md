# 🛒 Olist E-Commerce Analytics Dashboard | Power BI

## 📥 Download Power BI Project

🔗 [Download Olist E-Commerce Analytics Dashboard] https://drive.google.com/file/d/1FEQZgBH2CFoT1u1tLkTNJMkc31NfUoha/view?usp=drive_link


**File Format:** `.pbix`  
**Tool Required:** Microsoft Power BI Desktop

## 🎥 Project Demo Video

Watch the complete project walkthrough to see the data preparation, data modeling, DAX measures, and interactive Power BI dashboard.

▶️ https://drive.google.com/file/d/11BOgmLcHkZyWxM1o8QD6mkqhG1gO_XCX/view?usp=drive_link
---

## 📌 Table of Contents

- [📖 Project Overview](#-project-overview)
- [🎯 Project Objectives](#-project-objectives)
- [📂 Dataset Information](#-dataset-information)
- [🛠️ Tools and Technologies](#️-tools-and-technologies)
- [⚙️ Project Tasks: 1–12](#️-project-tasks-112)
- [📊 Dashboard Pages](#-dashboard-pages)
- [🧩 Data Model](#-data-model)
- [📐 DAX Measures](#-dax-measures)
- [🔍 Key Business Questions](#-key-business-questions)
- [💡 Key Insights](#-key-insights)
- [🚀 How to Run the Project](#-how-to-run-the-project)
- [📁 Project Structure](#-project-structure)
- [📸 Screenshots](#-screenshots)
- [📚 Data Source](#-data-source)
- [👩‍💻 Author](#-author)

---

## 📖 Project Overview

The **Olist E-Commerce Analytics Dashboard** is an interactive Power BI project built using the Brazilian E-Commerce Public Dataset by Olist.

The project analyzes order activity, product revenue, customer and seller locations, payment methods, and customer reviews. It combines data preparation, data modeling, DAX calculations, and interactive visualizations to create a multi-page business intelligence report.

📅 **Dataset period:** 2016–2018
🌎 **Geographic coverage:** Brazil
📊 **Platform:** Microsoft Power BI

## 🎯 Project Objectives

- 📦 Monitor total orders and revenue.
- 💰 Analyze product category performance.
- 📈 Explore order trends over time.
- 🗺️ Compare customer and seller locations.
- 💳 Understand payment method distribution.
- ⭐ Analyze customer review scores.
- 🧩 Build a structured data model with relationships.
- 🎨 Create a consistent and professional report layout.

## 📂 Dataset Information

The project uses the public Olist dataset available on Kaggle. It contains approximately 100,000 orders and multiple related datasets covering orders, order items, customers, products, sellers, payments, reviews, and geolocation.

| Dataset              | Purpose                                        |
| -------------------- | ---------------------------------------------- |
| Orders               | Order status and purchase/delivery dates       |
| Order Items          | Product items, prices, freight, and sellers    |
| Customers            | Customer identifiers and locations             |
| Products             | Product attributes and categories              |
| Sellers              | Seller identifiers and locations               |
| Payments             | Payment types, installments, and values        |
| Reviews              | Customer review scores and feedback            |
| Geolocation          | Brazilian ZIP code and geographic information  |
| Category Translation | Translates product category names into English |

## 🛠️ Tools and Technologies

| Tool                  | Usage                                                         |
| --------------------- | ------------------------------------------------------------- |
| 🟡 Microsoft Power BI | Report development and visualization                          |
| 🔄 Power Query        | Data cleaning and transformation                              |
| 📐 DAX                | Measures and analytical calculations                          |
| 🧩 Data Modeling      | Relationships, dimensions, and fact tables                    |
| 📊 Power BI Visuals   | Cards, bar charts, line charts, maps, matrix, and donut chart |
| 📁 CSV                | Source data format                                            |

---

## ⚙️ Project Tasks: 1–12

### 🟢 Task 1: Data Import and Initial Setup

- Imported the Olist CSV datasets into Power BI.
- Reviewed the available tables and columns.
- Prepared the source data for transformation and analysis.

### 🧹 Task 2: Data Cleaning and Power Query

- Reviewed column names, data types, and missing values.
- Prepared date, numeric, and text columns for analysis.
- Checked the consistency of important fields used in visuals and relationships.

### 🔄 Task 3: Data Transformation

- Used Power Query transformations where required.
- Merged product category translation data with the product table.
- Created the English product category field, `Product_Category_EN`.

### 🧩 Task 4: Data Modeling Principles

- Organized the data into related tables.
- Identified primary and foreign key fields.
- Used relationships instead of unnecessarily combining every dataset into one large table.

### 🔗 Task 5: Relationships and Model Structure

- Connected order items to orders, products, and sellers.
- Connected payments and reviews to orders.
- Connected customers to orders and dates to the order date fields.
- Reviewed relationship cardinality, active/inactive relationships, and cross-filter direction.

### 📅 Task 6: Date Table and Calendar Setup

- Created and used a dedicated `DimDate` calendar table.
- Added calendar attributes such as Year, Quarter, Month Name, and Month Number.
- Sorted `Month_Name` by `Month_Num`.
- Marked the calendar as a Date Table using its date column.

### 🧮 Task 7: DAX Calculations

- Created analytical measures for order and revenue reporting.
- Used aggregation functions such as `SUM`, `AVERAGE`, and `DISTINCTCOUNT` where appropriate.
- Created an average order value calculation for KPI reporting.

### 🏗️ Task 8: Hierarchies

Created hierarchies to support drill-down analysis:

- 📅 **Date Hierarchy:** Year → Quarter → Month Name
- 🛍️ **Product Hierarchy:** Product Category → Product ID
- 🏪 **Seller Location:** Seller State → Seller City
- 👥 **Customer Location:** Customer State → Customer City

### 📊 Task 9: KPI Cards and Visualizations

Developed the main analytical visuals:

- Total Orders
- Total Revenue
- Average Order Value
- Average Customer Rating
- Top 10 Product Categories by Revenue
- Monthly Order Volume
- Order Distribution by Brazilian State

### 🎨 Task 10: Formatting and Visual Design

- Applied a consistent red, white, and grey theme.
- Added clear report titles and visual headings.
- Adjusted chart labels, card formatting, and page backgrounds.
- Used consistent colors to maintain a professional dashboard appearance.

### 🖥️ Task 11: Multi-Page Dashboard Development

Created three analytical report pages:

1. **Sales Overview**
2. **Geographic Analysis**
3. **Payments & Reviews**

Added year, order status, and product category slicers where appropriate to support interactive exploration.

### ✅ Task 12: Model Validation and Final Polish

- Reviewed model relationships and relationship status.
- Checked visual titles, formatting, and KPI card consistency.
- Applied a consistent report theme.
- Prepared a model description for the Sales Overview page.
- Reviewed measures and visuals for accuracy and completeness.

---

## 📊 Dashboard Pages

### 1️⃣ Sales Overview

**Purpose:** Understand order activity, revenue, category performance, and order trends.

**Includes:**

- 📦 Total Orders KPI
- 💰 Total Revenue KPI
- 🧾 Average Order Value KPI
- ⭐ Average Customer Rating KPI
- 📊 Top 10 Product Categories by Revenue
- 📈 Monthly Order Volume (2016–2018)
- 🎛️ Year, Order Status, and Product Category slicers

### 2️⃣ Geographic Analysis

**Purpose:** Explore the geographic distribution of customers and sellers across Brazil.

**Includes:**

- 🗺️ Order distribution by customer state
- 🏪 Revenue by seller state
- 📍 Top seller cities by revenue
- 🎛️ Year slicer

### 3️⃣ Payments & Reviews

**Purpose:** Explore payment preferences, transaction values, and customer satisfaction.

**Includes:**

- 📋 Payment value by payment type and year
- 🍩 Payment method distribution
- ⭐ Review score analysis by product category
- 🎛️ Year slicer

---

## 🧩 Data Model

<img width="1146" height="723" alt="Screenshot 2026-10-23 171141" src="https://github.com/user-attachments/assets/8548ac33-222d-445b-b2e5-fb0d136e9fff" />


The model uses related tables organized for analytical reporting.

### Fact Tables

- `FactOrderItems`
- `FactPayments`
- `FactReviews`

### Dimension and Supporting Tables

- `DimOrders`
- `DimCustomers`
- `DimProducts`
- `DimSellers`
- `DimDate`

The `CategoryTranslation` query is used to prepare English category labels for products.

### 🔗 Main Relationships

| Table          | Related Table | Key           |
| -------------- | ------------- | ------------- |
| FactOrderItems | DimOrders     | `order_id`    |
| FactOrderItems | DimProducts   | `product_id`  |
| FactOrderItems | DimSellers    | `seller_id`   |
| DimOrders      | DimCustomers  | `customer_id` |
| DimOrders      | DimDate       | Purchase date |
| FactPayments   | DimOrders     | `order_id`    |
| FactReviews    | DimOrders     | `order_id`    |

An additional inactive relationship connects the order delivery date to the calendar date. This can support delivery-date analysis when activated appropriately in a measure.

**Model note:** The final relationship cardinality and active status should match the actual Power BI model and the uniqueness of the relevant key columns.

## 📐 DAX Measures

Examples of calculations used or relevant to the report:

**Total Revenue**

```DAX
Total Revenue =
SUM(FactOrderItems[price])
```

**Total Orders**

```DAX
Total Orders =
DISTINCTCOUNT(DimOrders[order_id])
```

**Average Customer Rating**

```DAX
Avg Customer Rating =
AVERAGE(FactReviews[review_score])
```

**Average Order Value**

```DAX
Avg Order Value =
DIVIDE(
    [Total Revenue],
    [Total Orders]
)
```

*Note:* These are reference versions of the measures. Confirm that the measures used in the final `.pbix` file match the intended business definitions. Item revenue and payment value are different metrics and should not be treated as interchangeable.

---

## 🔍 Key Business Questions

This dashboard helps investigate questions such as:

- 📦 How many distinct orders were placed?
- 💰 Which product categories generated the most item revenue?
- 📈 How did order volume change from 2016 to 2018?
- 🗺️ Which Brazilian states and cities account for the observed order and seller activity?
- 💳 Which payment methods contributed the most payment value?
- ⭐ What average review score did customers give?
- 🎛️ How do the results change when filtering by year, status, or product category?

## 💡 Key Insights

The report is designed to help users identify:

- 🛍️ High-performing product categories.
- 📈 Changes in order volume across the reporting period.
- 🏪 Geographic concentrations of seller revenue.
- 💳 Differences in payment method usage.
- ⭐ Customer review patterns that may require further investigation.

**Important:** Final numerical findings should be documented only after validating the measures, chart aggregations, and filter behavior in Power BI.

## 🚀 How to Run the Project

1. 📥 Download the dataset from Kaggle using the link below.
2. 📦 Extract the downloaded ZIP archive.
3. 🟡 Open the project `.pbix` file in Power BI Desktop.
4. 🔄 If prompted, update the data source paths to the extracted CSV files.
5. 🔃 Refresh the data.
6. 🧩 Check that the relationships and measures are working correctly.
7. 🎛️ Explore the report pages using the slicers and visual interactions.

## 📁 Project Structure

Example structure for the GitHub repository:

```text
Olist-Ecommerce-Analytics/
│
├── Dataset/
│   └── README.md
│
├── Screenshots/
│   ├── Sales-Overview.png
│   ├── Geographic-Analysis.png
│   └── Payments-and-Reviews.png
│
├── Olist-Ecommerce-Analytics.pbix
└── README.md
```

*Update the filenames to match the files actually present in your repository. Large source datasets do not need to be committed to GitHub.*

## 📸 Screenshots

### 🏠 Sales Overview

<img width="1200" height="672" alt="Screenshot 2026-10-23 170826" src="https://github.com/user-attachments/assets/3574bbb0-0865-4a51-bcb8-ff4a68abf86b" />


### 🗺️ Geographic Analysis

<img width="1197" height="676" alt="Screenshot 2026-10-23 170939" src="https://github.com/user-attachments/assets/9e608da4-ed6b-4681-9149-d58b373f0807" />


### 💳 Payments & Reviews

<img width="1198" height="676" alt="Screenshot 2026-10-23 171039" src="https://github.com/user-attachments/assets/e5d28097-ba11-402c-b36b-f3f195a887c2" />


---

## 📚 Data Source

**Brazilian E-Commerce Public Dataset by Olist**

🔗 [View and download the dataset on Kaggle](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce)

The dataset is provided for public analysis and is subject to the dataset's stated license and terms.

## 👩‍💻 Author

**Simran Gohel**

📊 Aspiring Data Analyst | Power BI | SQL | Python | Excel

🔗 [GitHub Profile](https://github.com/simrangohel70-lab)

---

\<p align="center">   ⭐ If you find this project useful, consider giving the repository a star!\<br>   \<strong>Thank you for visiting! 🚀\</strong> \</p>
