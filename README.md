🛒 Store Sales Exploratory Data Analysis

📌 Project Overview

This project performs exploratory data analysis (EDA) on a store sales dataset. The goal is to explore sales patterns, customer behavior, product performance, and revenue distribution across regions in Nigeria.

The project is implemented in Python using Pandas, Matplotlib, and Seaborn for data manipulation and visualization.


📂 Dataset

The dataset contains store sales records with the following key columns:

order_id – Unique identifier for each order

order_date – Date of the order

customer – Customer name

state – State where the order was made

product – Product purchased

quantity – Number of items purchased

price – Price per unit

discount – Discount applied

total – Final amount after discount

payment_method – Payment channel used



---

🔍 Analysis Steps

Part 1 – Basic Exploration

Load dataset and inspect structure (.head(), .shape, .info())

Check for missing values


Part 2 – Data Creation & Transformation

Created new columns:

vat_7_5 (7.5% VAT)

grand_total (total + vat_7_5)

month (extracted from order_date)


Transformed product names to uppercase

Replaced "POS" in payment_method with "Card (POS)"


Part 3 – Selection & Loops

Selected specific columns using iloc

Used for loop to print first 5 customers

Used while loop to print first 5 products


Part 4 – Sorting, Grouping & Aggregation

Sorted top 10 biggest orders by total

Grouped revenue by state and product

Identified top 3 customers by total spend


Part 5 – Missing Values & Data Types

Filled missing discount values with 0.0

Converted quantity column to integer


Part 6 – Merging Data

Created state → region mapping (Nigeria geopolitical zones)

Merged with sales dataset to analyze revenue by region



---

📊 Visualizations

Bar charts for top products and states by revenue

Line chart for monthly sales trend

Histogram for total sales distribution




🛠️ Tech Stack

Python 🐍

Pandas

Matplotlib

Seaborn

Google Colab / Jupyter Notebook



