# Sales Data Analysis & Visualization Project

## Table of Contents

- [Introduction](#introduction)
- [Steps Taken](#steps-taken)
- [Technologies Used](#technologies-used)
- [Getting Started](#getting-started)
- [Usage](#usage)

## Introduction

Sales Data Analysis & Visualization Project is a comprehensive sales data analysis and visualization project aimed at extracting actionable insights from raw sales data. Leveraging MySQL for data storage and Power BI for visualization, this project provides a robust solution for understanding sales trends, customer behavior, and product performance.

## Steps Taken

### Step 1: Data Acquisition and Preparation

1. Downloaded MySQL file dump containing sales data.
2. Used MySQL commands to perform initial data checks and explore the data structure.

### Step 2: Data Modeling and Cleaning

1. Imported the MySQL file into Power BI.
2. Designed a data model by connecting primary keys to foreign keys and creating facts and dimension tables.
3. Used Power Query Editor for data cleaning tasks, including:
   - Filtering out irrelevant markets.
   - Removing records with negative sales amounts.
   - Standardizing currency values.

### Step 3: Data Analysis and Visualization

1. Developed DAX measures for deriving key performance indicators and trends.
2. Created dynamic dashboards with insightful visualizations, including:
   - Matrix visuals for top-line performance analysis.
   - KPI cards for summarizing key metrics.
   - Map and treemap visuals for geographical analysis.
   - Column chart for visualizing revenue trends.
   - Gauge chart for performance assessment against targets.

### Step 4: Data Validation

1. Conducted data validation through SQL queries to verify analysis results against the original dataset. Example queries include:
   - ```sql
     Select Sum(sales_qty) from transactions inner join date on transactions.order_date = date.date where date.year = 2020 and transactions.currency = "INR\r" or transactions.currency = "USD\r";
     ```
   - ```sql
     Select SUM(sales_amount) FROM transactions inner join date on transactions.order_date = date.date where date.year = 2020 and date.month_name = "January" and (transactions.currency = "INR\r" or transactions.currency = "USD\r");
    

2. Ensured accuracy and consistency of the visualization by validating key metrics through SQL querying.

## Technologies Used

- MySQL
- Power BI - Power Query Editor

## Getting Started

To get started with the project, follow these steps:

1. Clone the repository: `git clone https://github.com/yourusername/project1.git`
2. Install MySQL and Power BI on your system.
3. Import the MySQL dump into your local MySQL database.
4. Open Power BI and import the MySQL data for visualization.

## Usage

Once the project is set up, you can use it to:

- Analyze sales trends by product, region, or time period.
- Identify top-performing products and customers.
- Track revenue and sales quantity over time.
- Validate analysis results through SQL queries.

## Snap of Dashboard

![Sales_Insights_snap](https://github.com/shuja04/Sales-Data-Analysis-Visualization-Project/assets/167103109/1a2a6f39-d224-43f7-a9cf-6466c3f8d591)
