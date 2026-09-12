# Sales Data Exploration Project

This project uses Microsoft SQL Server to perform exploratory analysis of sales, customer, and product data. The objective is to understand sales performance across countries and product categories, identify customer purchasing patterns, evaluate revenue concentration, and uncover areas that can support better commercial decision-making


![Exploratory Data Analysis Workflow](/images/eda_workflow.png)


## Introduction

### Project Overview

This project presents an **Exploratory Data Analysis (EDA)** of a sales dataset using **Microsoft SQL Server**. The analysis examines the database structure, data quality, customer demographics, product performance, sales distribution, and revenue generation.

The dataset follows a **star-schema structure**, consisting of a central sales fact table linked to customer and product dimension tables. Using SQL techniques including **joins, aggregations, grouping, ranking functions, CTEs and data-quality checks**, the project transforms transactional data into meaningful business insights.

The analysis focuses on answering key business questions, including:
* Where are the company's strongest and weakest sales markets?
* Which products and categories drive sales volume and revenue?
* Which customers contribute the most value to the business?
* How are sales distributed across customer demographic groups?
* What data-quality issues could affect analysis and reporting?

The objective is to use these findings to support more informed decisions around **market prioritization, product strategy, customer retention, inventory allocation, and data quality management**.


### Executive Summary

The analysis identified the **United States and Australia as the company's strongest markets**, with the largest customer bases and the highest sales values and quantities sold.

`Product analysis` revealed a significant difference between **sales volume and revenue contribution**. Although **Accessories recorded the highest quantity of units sold**, the **Bikes category generated the overwhelming majority of total revenue**. At the individual product level, the **Mountain-200 product line** emerged as the strongest group by revenue.

`Customer analysis` identified highly active and high-value customers who represent potential targets for **retention, loyalty, and customer-value initiatives**. Sales were also relatively balanced across **gender and marital-status groups**, suggesting that the company's revenue is not heavily concentrated within a single demographic segment.

The analysis also identified several **data-quality issues**, including missing or unspecified values in customer and product attributes, as well as potential customer-age outliers. These issues should be considered when interpreting results and should be addressed before using the data for advanced analytics or predictive modelling.

Overall, the findings suggest that the company should **prioritize investment in high-performing markets and products, strengthen strategies for lower-performing segments, retain high-value customers, and improve data quality to support more reliable reporting and future modelling**.


### Business Problem

Businesses generate large volumes of transactional data, but without systematic analysis, it can be difficult to understand **what is driving sales performance and where resources should be allocated**.

The company requires a clearer understanding of:
1. **Geographic performance** — Which markets generate the highest and lowest sales?
2. **Product performance** — Which products and categories drive sales volume and revenue?
3. **Customer value** — Which customers contribute the most revenue and purchasing activity?
4. **Customer demographics** — What patterns exist between customer characteristics and sales performance?
5. **Data quality** — Are there missing, inconsistent, or potentially anomalous values that could affect reporting and decision-making?

Without these insights, decisions relating to **inventory allocation, marketing investment, customer retention, and product strategy** may be based on assumptions rather than evidence.

Therefore, this project explores the available **sales, customer, and product data** to identify performance patterns, customer and product opportunities, and data-quality concerns. The resulting insights are intended to support **data-driven business decisions** and provide a foundation for subsequent analytical and predictive modelling.


*Click the headings below to explore the detailed analysis, SQL queries, results, and business insights.*


## [Tables Exploration](readme_files/02_explore_database_tables.md) — What data is available and how it is structured?
This section profiles the database tables, columns, data types, nullability, and structural metadata to establish an understanding of the available data.

## [Dimensions Exploration](readme_files/03_dimensions_explorations.md) — What are the important customer and product attributes?
This section examines countries, customer distribution, product categories, subcategories, and dimensional attributes, including the identification of unclassified values.

## [Date Exploration](readme_files/04_date_exploration.md) — What period does the dataset cover and what does the customer age data reveal?
This section examines the earliest and latest sales dates and explores customer birthdate and age characteristics, including potential age outliers.

## [Magnitude Analysis](readme_files/05_magnitude_analysis.md) — How large is the business in terms of sales, volume, cost, and purchasing activity?
This section examines macro-level measures such as sales by country, product quantities, product costs, and customer purchasing frequency.

## [Customer Analysis](readme_files/06_customer_analysis.md) — Who are the most valuable and active customers?
This section analyses customer revenue, order activity, average order value, purchase frequency, and customer-level purchasing behaviour.

## [Product Category Analysis](readme_files/07_product_category_analysis.md) — Which categories drive volume and sales?
This section examines product costs, sales volume, revenue contribution, and differences between high-volume and high-revenue product categories.

## [Revenue Analysis](readme_files/08_revenue_analysis.md) — Where is revenue concentrated?
This section evaluates revenue contribution across product categories and customers to identify the products and customers associated with the highest sales revenue.

## [Distribution Analysis](readme_files/09_distribution_analysis.md) — How is customer and sales performance distributed?
This section examines sales-volume distribution across countries and the distribution of customer revenue using measures such as minimum, maximum, average, and median revenue.

## [Ranking Analysis](readme_files/10_ranking_analysis.md) — Which products and categories rank highest by revenue?
This section identifies the top revenue-generating products and product categories to highlight areas of strong commercial performance and revenue concentration.

## [Conclusion & Recommendation](readme_files/11_conclusion_&_recommendation.md)
This section summarizes the major findings, translates them into actionable business recommendations, and identifies opportunities for advanced analytics and predictive modelling.


## Key Metrics

| Metric        | Definition                                 |
| ------------- | ------------------------------------------- |
| Revenue       | Total monetary value generated from sales   |
| Quantity Sold | Total units sold                            |
| Orders        | Number of sales/order transactions          |
| Customers     | Unique customers represented in the dataset |
| Product Cost  | Cost associated with the product            |


## Repository Structure

```text
Exploratory_Data_Analysis/
|
│───README.md
│   
├───images/
│       avg_cost_by_category.png
│       customers_table_exploration.png
│       customer_base_per_country.png
│       customer_purchase_frequency.png
│       customer_revenue_distribution.png
│       ealiest_latest_dates.png
│       eda_workflow.png
│       explore_database_tables.png
│       max_min_avg_prod_price.png
│       oldest_youngest_customer_birthday.png
│       products_table_exploration.png
│       product_categories.png
│       product_cat_count.png
│       product_cat_subcategory.png
│       sales_table_exploration.png
│       sales_volume_revenue-category.png
│       time_range.png
│       top_prod_categories.png
│       top_revenue_gen_products.png
│       total_customer_by_marital_status.png
│       total_orders_by_customer.png
│       total_quantity_sold-by_country.png
│       total_revenue_by_customers.png
│       total_revenue_by_product_category.png
│       total_sales_by_category.png
│       total_sales_by_country.png
│       total_sales_by_gender.png
│       unique_countries.png
│       
└───readme_files/
        01_introduction.md
        02_explore_database_tables.md
        03_dimensions_explorations.md
        04_date_exploration.md
        05_magnitude_analysis.md
        06_customer_analysis.md
        07_product_category_analysis.md
        08_revenue_analysis.md
        09_distribution_analysis.md
        10_ranking_analysis.md
        11_conclusion_&_Recommendation.md
 ```       

## Tools Used
1. **Database Engine:** Microsoft SQL Server (MSSQL)

2. **Development Environment:** Visual Studio Code (VS Code)

4. **Key Techniques:** Aggregations, Joins, Window Functions, CTEs and Data Filtering# Sales Data Exploration Portfolio

An exploratory data analysis (EDA) project focused on identifying key trends, customer behaviors, and performance metrics.
