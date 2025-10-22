# Customer Trends & Shopping Behavior Analysis

## Project Overview

This project performs a **comprehensive analysis of a retail company's customer shopping behavior** to identify key trends, understand purchase drivers, and provide **actionable insights**.  

The primary goal is to help the company **leverage consumer data to improve sales, customer satisfaction, and long-term loyalty**.

**Business Problem:**  
> How can the company leverage consumer shopping data to identify trends, improve customer engagement, and optimize marketing and product strategies?

---

## Project Workflow

The project was executed in **three major stages**:

### 1. Data Preparation (Python)
- Loaded the 3,900-row dataset using `pandas`.
- Cleaned the data by handling missing values (imputed median for *Review Rating*).
- Standardized column names (to `snake_case` format).
- Created a derived feature `age_group`.
- Loaded the cleaned DataFrame into a **PostgreSQL database** for structured querying.

### 2. Data Analysis (SQL)
- Executed **10 SQL queries** in PostgreSQL to extract actionable business insights.
- Focus areas: revenue, product performance, customer segmentation, discounts, and subscription impact.

### 3. Visualization & Insights (Power BI)
- Connected Power BI directly to the PostgreSQL database.
- Built an **interactive dashboard** summarizing KPIs, with filters for Subscription Status, Gender, Category, and Shipping Type.

---

## Key Business Questions & Findings

| # | Business Question | Key Finding |
|---|-------------------|-------------|
| 1 | **Revenue by Gender** | Males generated **$157,890**, Females **$75,191** |
| 2 | **High-Spending Discount Users** | **839** high-value customers use discounts but spend above average |
| 3 | **Top 5 Products by Rating** | Gloves (3.86), Sandals (3.84), Boots (3.82), Hat (3.80), Skirt (3.78) |
| 4 | **Shipping Type Comparison** | Express users spend **$60.48** vs. Standard users **$58.46** |
| 5 | **Subscribers vs. Non-Subscribers** | Non-subscribers drive **73%** of total revenue ($170,436 vs $62,645) |
| 6 | **Discount-Dependent Products** | Hats (50%), Sneakers (49.7%), Coats (49.1%) heavily discount-reliant |
| 7 | **Customer Segmentation** | Loyal: 3,116 · Returning: 701 · New: 83 |
| 8 | **Top 3 Products per Category** | Accessories: Jewelry · Clothing: Blouse, Pants · Footwear: Sandals |
| 9 | **Repeat Buyers & Subscriptions** | Most repeat buyers (2,518) are **not subscribers** |
| 10 | **Revenue by Age Group** | Young Adult ($62,143) and Middle-aged ($59,197) lead revenue |

---

## Power BI Dashboard

The **interactive Power BI dashboard** presents:
- Key performance indicators (KPIs):  
  - Total Customers  
  - Average Purchase Amount  
  - Average Rating  
- Dynamic filtering by:
  - Subscription Status
  - Gender
  - Category
  - Shipping Type  

📁 **File:** `customer_behavior_dashboard.pbix`

---

## 💡 Business Recommendations

1. **Boost Subscriptions:**  
   Subscription performance is weak. Promote exclusive benefits to convert loyal non-subscribers.

2. **Implement Loyalty Programs:**  
   Introduce a tiered reward system to encourage repeat purchases.

3. **Review Discount Strategy:**  
   Re-evaluate products (e.g., Hats, Sneakers) overly dependent on discounts to improve margins.

4. **Highlight High-Performing Products:**  
   Promote top-rated (Gloves, Sandals) and best-selling (Jewelry, Blouse) products.

5. **Target Key Demographics:**  
   Focus marketing on **Young Adult** and **Middle-aged** groups and promote **Express Shipping** users with tailored offers.

---

## 7. How to Use

### Step 1: Database Setup
- Install and configure **PostgreSQL** on your system.
- Create a new database dedicated to this project.

### Step 2: Data Loading
- Open the Jupyter Notebook file: `Customer_Shopping_Behavior_Analysis.ipynb`.
- Update the database connection string to match your local PostgreSQL configuration.
- Execute the notebook cells to load the dataset `customer_shopping_behavior.csv` into the PostgreSQL database.

### Step 3: Run SQL Analysis
- Open `customer_behavior_sql_queries.sql` in your preferred SQL client (e.g., pgAdmin or DBeaver).
- Execute the queries to reproduce the business insights and analytical results.

### Step 4: Visualize in Power BI
- Open the Power BI report file: `customer_behavior_dashboard.pbix` in **Power BI Desktop**.
- Connect it to your PostgreSQL database to refresh and explore the interactive dashboards.

---

## 8. Technology Stack

- **Programming Language:** Python  
- **Libraries:** Pandas, Psycopg2, SQLAlchemy  
- **Database:** PostgreSQL  
- **Visualization Tool:** Power BI  
- **Supporting Tools:** Jupyter Notebook, DBeaver/pgAdmin, Excel  

---

## 9. Project Outcomes

This project provides a data-driven foundation for enhancing multiple business areas, including:

- Customer engagement and retention  
- Marketing and promotional strategy efficiency  
- Product performance and category management  
- Loyalty and subscription program optimization  

---

## 10. Author

**Nikhil Gupta**  
Email: [23ucs752@lnmiit.ac.in]  
LinkedIn / GitHub: [https://github.com/Nikhilg27425]

---


