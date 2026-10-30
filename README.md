# ☁️ AWS End-to-End Data Engineering Pipeline

## 📌 Project Overview

This project focuses on building an end-to-end ETL (Extract, Transform, Load) pipeline using **Amazon Web Services (AWS)**. The pipeline reads raw CSV data from Amazon S3, processes and transforms the data using AWS Glue, removes duplicate and invalid records, calculates total order amounts, and stores the processed data back in Amazon S3.

The project demonstrates practical experience with AWS cloud services, data processing, ETL workflows, and foundational data engineering concepts.

## 🎯 Project Objectives

- Create an Amazon S3 bucket for storing raw and processed data.
- Prepare and upload sample CSV order data.
- Organize data using separate S3 folders.
- Create an AWS Glue database.
- Configure an AWS Glue crawler to discover the data.
- Develop an ETL script using PySpark.
- Remove duplicate and invalid records.
- Calculate total order amounts.
- Store transformed data in the processed S3 folder.

## 🛠️ Technologies Used

- **Amazon S3** – Cloud storage for raw and processed data.
- **AWS Glue** – Serverless ETL service for data processing.
- **AWS Glue Data Catalog** – Metadata management.
- **AWS Glue Crawler** – Schema discovery and catalog creation.
- **PySpark** – Distributed data processing.
- **Python** – ETL scripting.
- **CSV** – Input data format.

## 🏗️ Project Architecture

```text
       Raw CSV Data
             |
             v
       Amazon S3
       (raw folder)
             |
             v
       AWS Glue Crawler
             |
             v
       AWS Glue Data Catalog
             |
             v
       AWS Glue ETL Job
          (PySpark)
             |
             v
       Data Cleaning
       - Remove duplicates
       - Remove invalid records
       - Calculate order amount
             |
             v
       Amazon S3
     (processed folder)
```

## 📂 Dataset Structure

The project uses sample e-commerce order data with the following columns:

| Column | Description |
|---|---|
| order_id | Unique order identifier |
| customer_id | Customer identifier |
| product | Product name |
| quantity | Number of items ordered |
| price | Price per item |
| city | Customer city |

## ⚙️ Implementation Steps

### Step 1: Create an Amazon S3 Bucket
Created an S3 bucket to store the raw input data and transformed output data.

### Step 2: Prepare Sample CSV Data
Created a sample CSV file containing order details such as order ID, customer ID, product, quantity, price, and city.

### Step 3: Create Folders and Upload CSV
Created separate folders inside the S3 bucket:
- `raw/` – Stores original CSV data.
- `processed/` – Stores transformed data.

Uploaded the sample CSV file into the raw folder.

### Step 4: Create AWS Glue Database
Created an AWS Glue database to organize and manage the metadata associated with the dataset.

### Step 5: Create an AWS Glue Crawler
Configured an AWS Glue crawler to identify the CSV dataset and discover its schema for the Data Catalog.

### Step 6: Develop the ETL Script
Created an AWS Glue ETL job using PySpark to:
- Read CSV data from Amazon S3.
- Load data into a Spark DataFrame.
- Remove duplicate records.
- Filter invalid records.
- Calculate total order amounts.

### Step 7: Transform and Process Data
Applied data-cleaning and transformation operations to prepare the dataset for further analysis.

### Step 8: Configure AWS Glue Job
Configured the Glue job parameters and IAM role required for accessing AWS resources.

The processed output is stored in the S3 `processed/` folder.

## 📊 Key Learning Outcomes

- Understanding end-to-end ETL pipeline architecture.
- Hands-on experience with Amazon S3.
- Working with AWS Glue and Glue Crawlers.
- Understanding AWS Glue Data Catalog.
- Writing PySpark scripts for data transformation.
- Performing data cleaning and duplicate removal.
- Working with IAM roles and AWS permissions.
- Understanding cloud-based data processing workflows.
- Storing raw and transformed data in Amazon S3.

## 🚀 Final Result

Successfully developed an AWS-based ETL pipeline using Amazon S3 and AWS Glue.

The pipeline reads raw CSV data from S3, removes duplicate and invalid records, calculates total order amounts, and saves the transformed data into the S3 `processed/` folder.

This project provided practical exposure to cloud-based ETL development and strengthened my understanding of AWS services and data engineering workflows.

## 👨‍💻 Author

**M. Lokeshwar Reddy**

- 🎓 B.Tech – Artificial Intelligence & Machine Learning
- 🏫 Jain University
- 💻 Aspiring Data Engineer | AI & ML Enthusiast
- ☁️ Interests: AWS, GCP, Azure, SQL, Python, PySpark, ETL Pipelines and Big Data

### 🔗 Connect With Me

- GitHub: [Lokeshwar9704](https://github.com/Lokeshwar9704)

---

⭐ If you find this project interesting, feel free to explore my GitHub repositories!
