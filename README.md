# Pyspark_Sales_Project
# Sales Data Engineering with PySpark - Jan to Mar 2019
This project demonstrates data engineering and analytics on online product sales data for the first quarter of 2019 (January, February, and March) using PySpark.

# Problem Statement:
Given three datasets containing monthly sales data of an online store for Jan, Feb, and Mar 2019, perform the following data processing and analysis tasks:

Cleanse the data by removing blank or null rows.

Identify the date on which maximum sales occurred for each product across the three months.

Find the date on which the maximum sales happened for all products combined in the three months.

Calculate the average sales value for each product over the period.

Merge the three datasets into a combined dataset ordered by date in descending order and add a column salesdiff that shows the difference in sales between the current row and the next row (based on date descending) for each product. For the last row, treat the next row sales as zero.

Retrieve orderId and purchase address for the order with maximum sales across the three months.

Extract city information from the purchase address (second element in a comma-separated string) and identify the city with the highest number of orders.

Calculate total order counts for each city across the three months.

Partition the data by bi-weekly order dates and save the result in physical storage (DBFS, ADLS, local storage, Delta table, S3, or HDFS).

# Dataset Details:
Sales data files for January, February, and March 2019

Each dataset contains columns such as orderId, product, orderDate, qty, price, and purchaseAddress.

Sales value is computed as qty * price.

Order counts are based on unique orderIds.

# Technologies Used:
PySpark (Apache Spark with Python)

Databricks

Data engineering and transformation

Partitioning and storage optimization

# How to Run:
Clone the repo

Load datasets in PySpark environment (I.e Databricks)

Execute the data processing notebook/script (in Databricks)

Results include cleaned data, analytical summaries, and partitioned output datasets
