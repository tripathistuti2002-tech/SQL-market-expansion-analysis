
#  Monday Coffee Expansion — MySQL Data Analysis Project

---

##  Project Overview
**Monday Coffee** is an online coffee company that has been selling its products across major Indian cities. As part of its strategic expansion plan, the business aims to move offline and open physical coffee shop locations. 

The goal of this project is to analyze historical sales data, customer segmentation, city populations, and rental costs using **MySQL** to recommend the **top 3 cities in India** for opening new physical storefronts.

---

##  Data Architecture & Schema
The project utilizes four primary tables:

* **`city`**: Contains city details, population figures, and estimated coffee consumers.
* **`customers`**: Stores unique customer information and city associations.
* **`products`**: Holds product details and pricing information.
* **`sales`**: Contains transactional data including purchase dates, quantities, and totals.

---

##  Key Questions & SQL Business Analysis

### 1. Coffee Consumers Count
* **Question:** How many people in each city are estimated to consume coffee, given that 25% of the population does?
* **Objective:** Determine market size based on city population data.

### 2. Total Revenue from Coffee Sales
* **Question:** What is the total revenue generated from coffee sales across all cities in the last quarter (Q4)?
* **Objective:** Evaluate recent quarterly financial performance.

### 3. Sales Volume per Product
* **Question:** How many units of each coffee product have been sold?
* **Objective:** Identify top-performing individual products.

### 4. Average Sales Amount per City
* **Question:** What is the average sales amount per customer in each city?
* **Objective:** Measure customer spending habits by region.

### 5. City Population vs. Coffee Consumers
* **Question:** Provide a comprehensive list of cities along with their populations and estimated coffee consumers.
* **Objective:** Benchmark overall city demographics.

### 6. Top Selling Products by City
* **Question:** What are the top 3 selling products in each city based on sales volume?
* **Objective:** Inform regional menu planning and inventory stock.

### 7. Customer Segmentation by City
* **Question:** How many unique customers are there in each city who have purchased coffee products?
* **Objective:** Assess current online market penetration per city.

### 8. Average Sale vs. Average Rent
* **Question:** Calculate each city's average sale per customer against its average rent per customer.
* **Objective:** Evaluate profitability potential vs. operational overhead.

### 9. Monthly Sales Growth Rate
* **Question:** Calculate the percentage growth (or decline) in sales over monthly time periods.
* **Objective:** Track revenue momentum and seasonality.

### 10. Market Potential Analysis
* **Question:** Identify the top cities based on total sales, total rent, total unique customers, and estimated coffee consumers.
* **Objective:** Holistic scoring for expansion selection.

---

##  Final Recommendations

Based on multi-variable SQL analysis balancing revenue, customer volume, and rental overhead, the top three recommended cities for new store openings are:

###  1. Pune
* **Low Overhead:** Exceptionally low average rent per customer.
* **High Revenue:** Generated the highest total sales performance across all analyzed regions.
* **High Value:** High average sales per customer ratio.

###  2. Delhi
* **Massive Market:** Highest estimated coffee-consuming population (**7.7 Million**).
* **Strong Base:** Top-tier total customer count (**68 unique buyers**).
* **Manageable Overhead:** Average rent per customer remains reasonable at **330**.

###  3. Jaipur
* **Highest Engagement:** Highest number of unique purchasing customers (**69 buyers**).
* **Ultra-Low Rent:** Very low average rent per customer at **156**.
* **Solid Profit Margin:** Strong average sales per customer at **~11.6k**.

---

## Tech Stack & MySQL Techniques Used
* **Database Management System:** MySQL
* **Tools & Concepts:**
  * **Data Aggregations:** SUM(), AVG(), COUNT(DISTINCT )
  * **Window Functions:** RANK(), DENSE_RANK(), LAG()
  * **Common Table Expressions (CTEs)** for complex multi-step queries
  * **Multi-Table Joins:** INNER JOIN, LEFT JOIN
  * **Date Filtering & Functions:** DATE_FORMAT(), YEAR(), QUARTER()
