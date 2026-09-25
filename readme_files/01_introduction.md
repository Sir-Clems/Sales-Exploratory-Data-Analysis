# Introduction

## Project Overview

This project presents an **Exploratory Data Analysis (EDA)** of a sales dataset using **Microsoft SQL Server**. The analysis explores the database structure, data quality, customer demographics, product performance, sales distribution, and revenue generation.

The dataset follows a **star-schema structure**, consisting of a central sales fact table linked to customer and product dimension tables. Using SQL techniques such as **joins, aggregations, grouping, ranking functions, CTEs, and data-quality checks**, the project transforms raw transactional data into meaningful insights.

The analysis focuses on understanding **where sales are generated, which products drive revenue and sales volume, who the most valuable customers are, and how Customer demographic patterns associated with sales performance**.


## Executive Summary

The analysis revealed that the **United States and Australia are the company's strongest markets**, accounting for the largest customer bases and generating the highest sales values and quantities sold.

Product analysis revealed a significant difference between **sales volume and revenue contribution**. While **Accessories recorded the highest quantity of units sold**, the **Bikes category generated the overwhelming majority of total revenue**. The **Mountain-200 product line** emerged as the strongest group of individual products by revenue.

The analysis also identified highly active and high-value customers who could be targeted through `retention and loyalty initiatives`. Sales were relatively balanced across **gender and marital-status** groups, indicating that the company's revenue is not heavily dependent on a single demographic segment.

In addition, several data-quality issues were identified, including missing or unspecified values in customer and product attributes, as well as potential customer age outliers.

Overall, the findings indicate that the company should **prioritize investment in high-performing markets and products while developing strategies to improve lower-performing segments and strengthen data quality**.


## Business Problem

Businesses generate large volumes of transactional data, but without proper analysis, it can be difficult to understand **what is driving sales performance and where resources should be allocated**.

The company requires a clearer understanding of:

1. Its strongest and weakest geographic markets.
2. The products and categories driving sales volume and revenue.
3. The customers contributing the most value to the business.
4. Customer demographic patterns associated with sales performance.
5. Potential data-quality issues that could affect reporting and decision-making.

Without these insights, decisions relating to inventory allocation, marketing investment, customer retention, and product strategy may be based on assumptions rather than data.

Therefore, this project addresses these challenges by exploring the available sales, customer, and product data to uncover actionable insights that can support more informed and data-driven business decisions.
